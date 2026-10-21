# Top_Models: Backlog, Deferred Work & Forward-Looking Roadmap
*(Formerly 0C6D_plan.md — Milestone 0C-6D Implemented in Commit 942bb06)*

**Target File:** `~/storage/downloads/0C6D_plan.md`  
**Status:** ACTIVE BACKLOG & MASTER ROADMAP SPECIFICATION  
**Author:** AI Agent (Antigravity)  
**Date:** October 2026  
**Reference Document:** `~/storage/downloads/codebase_1.md` (Canonical Factual Architecture)

---

## 1. IMPLEMENTATION ARCHIVE REFERENCE

Milestone 0C-6D has been fully implemented, verified, and committed to git:
- **Verified Commit:** `942bb06` (`Milestone 0C-6D: Implement in-memory filter UI, model-bound extended rows, and event delegation`).
- **Canonical Architecture:** All factual specifications, schemas, DOM layouts, and Service Worker configurations have been consolidated into `~/storage/downloads/codebase_1.md`.
- **Implemented Capabilities Summary:**
  - `adapters/_filter.js`: Declarative `FILTER_DEFINITIONS`, `DEFAULT_FILTER_STATE`, and pure `applyModelFilters()` engine.
  - `core.js`: Public re-export of the filter engine.
  - `index.html`: Anchored floating filter popover (`#filter-popover`), relative button container (`.filter-btn-container`), active dot indicator (`#filter-active-dot`), and descriptive count badge (`#model-count-indicator`) supporting 3 runtime states.
  - Interactive Table Enhancements: Empty-state card with embedded reset button (`#empty-state-reset-btn`), atomic 8-step `handleFilterReset()`, model-bound extended-row lifecycle (`appState.expanded = { modelId, colIndex }`), and table body event delegation on `<tbody id="table-body">` replacing legacy globals.
  - Cache & Version Management: `sw.js` bumped to `matrix-cache-v11` with `./adapters/_filter.js` precached and navigation network-first route; `index.html` module import bumped to `./core.js?v=0I`.

The remainder of this document records architectural research, backlog items, technical debt, and the master milestone roadmap.

---

## 2. DEFERRED FILTERING & INTERACTION ENHANCEMENTS

### 2.1 Capability Filter Extension (`has_tools`, `has_files`)
- **Tri-State Capability Filtering:**
  - Vision / File Ingestion (`has_files: 1 | 0`) and Tool / Function Calling (`has_tools: 1 | 0`).
  - Tri-state filter semantics:
    - `'any'` / `null`: Pass-through (no filtering on this attribute).
    - `'require'` / `true`: Restrict to models where `has_files === 1` or `has_tools === 1`.
    - `'exclude'` / `false`: Restrict to models where `has_files === 0` or `has_tools === 0`.
- **Modality Filters:**
  - Input modality toggles (Text, Image, Audio) evaluating the normalized `raw_modalities` comma-separated string.
- **Implementation Strategy:**
  - Pure declarative extension in `adapters/_filter.js` by adding entries to `FILTER_DEFINITIONS`.
  - Zero HTML churn; the popover dynamically renders controls from `FILTER_DEFINITIONS`.
  - Deferred to **Milestone 0C-6G (Advanced Capability & Modality Filters)**.

### 2.2 Global Filter State & Multi-Provider Home Page Pre-requisites
- **Storage Key:** `filterState_global` is reserved in `localStorage` for cross-provider filtering.
- **Architectural Sequencing Invariant:**
  - The multi-provider Home Page must follow **Milestone 0C-6E (Dynamic Column UI)**.
  - *Rationale:* Implementing the Home Page prior to dynamic columns would force designing table layouts twice (once for static 6 columns, then refactored for dynamic columns).
- **Global Filter Cascade:**
  - When viewing the Home Page, `applyModelFilters()` operates across the aggregated, deduplicated cross-provider model pool using `filterState_global`.
  - Deferred to **Milestone 0C-6F (Multi-Provider Home Page & Global View)**.

### 2.3 Cross-Tab & Multi-PWA Synchronization
- **Problem Statement:** If a user opens `Top_Models` in multiple browser tabs or runs an installed Capacitor PWA alongside a mobile browser tab, changes to filter states or active provider in one tab are not reflected in the other until reload.
- **Proposed Architecture:**
  - Attach a window storage listener:
    ```javascript
    window.addEventListener('storage', (event) => {
        if (event.key.startsWith('filterState_') || event.key === 'activeProvider') {
            loadPersistedState();
            recalculateAndRender();
        }
    });
    ```
  - Provides instant cross-tab state consistency without network overhead.
  - Deferred to post-Phase 0C maintenance / polish.

### 2.4 Export Payload Modernization
- **Current State:** The `Export Data` button downloads raw matrix arrays (`appState.rankedColumns`) without metadata.
- **Required Metadata Modernization:**
  - Export timestamp (`exported_at: ISO8601`).
  - Active provider identifier (`provider: string`).
  - Active filter criteria snapshot (`filterState: object`).
  - Total models vs. filtered models count (`total_models: number`, `displayed_models: number`).
  - Benchmark source provenance and schema version.
- Deferred to **Milestone 0E-1 (CLI Parity & Metadata Export Modernization)**.

---

## 3. PROVIDER ADAPTER TECHNICAL DEBT & METADATA PARITY

An audit of the 9 implemented Group A provider adapters identified areas of metadata debt and hardcoded assumptions to be resolved:

### 3.1 Dynamic `is_chat` Derivation
- **OpenRouter (`adapters/openrouter/index.js`):** Currently hardcodes `is_chat: true` for all models without inspecting endpoints or architecture modalities. Some catalog entries may be non-chat embeddings or completions.
- **SambaNova (`adapters/sambanova/index.js`):** Hardcodes `is_chat: true` for all 6 models. While true today, dynamic catalog expansion should inspect model capabilities.
- **Resolution Plan:** Dynamic inspection of upstream endpoint types and modality properties during Stage 1 normalization.

### 3.2 Advanced Capability Detection
- **Groq (`adapters/groq/index.js`):** Correctly checks `supported_features.includes('tools')`, but currently ignores reasoning tokens and JSON structured output flags available in Groq's model metadata.
- **Google Gemini (`adapters/gemini/index.js`):** Hardcodes `has_tools: null` despite Gemini models having native function calling support via `generateContent`.
- **Mistral AI (`adapters/mistral/index.js`):** Capabilities dictionary mapping should be expanded to capture system prompt and fine-tuning support.

### 3.3 Dynamic Modality Parsing
- **SambaNova:** Hardcodes `raw_modalities: "text"` despite hosting multimodal models (e.g. Llama 3.2 11B/90B Vision). Upstream endpoint responses should be parsed dynamically.

### 3.4 CLI Parity Debt
- **`cli.js` Divergence:**
  - `cli.js` still uses legacy OpenRouter-only `fetchData` and lacks multi-provider switching.
  - CLI commands lack in-memory filtering flags (`--free-only`, `--chat-only`).
  - Scheduled for resolution in **Milestone 0E-1 (CLI Parity & Metadata Export Modernization)**.

---

## 4. TELEMETRY & RATE LIMIT RESEARCH (TTFT, RPM, RPD)

### 4.1 Ingestion Feasibility Audit
A thorough audit across all 9 Group A providers confirmed that zero adapters currently ingest TTFT (Time to First Token), RPM (Requests per Minute), RPD (Requests per Day), or TPM (Tokens per Minute).

#### Key Research Findings:
1. **Account-Level vs. Model-Level Constraints:**
   - Most providers (Groq, Gemini, SambaNova, Mistral, Cohere) govern rate limits at the account/tier level, documented statically in developer consoles rather than returned in `/models` catalog responses.
   - For example, Groq provides tier limits (e.g. Free Tier: 30 RPM, 14,400 RPD for Llama-3.3-70B), but `/openai/v1/models` returns zero rate limit fields.
2. **Response Header Extraction Constraints:**
   - Rate limit headers (e.g., `x-ratelimit-remaining-requests`, `x-ratelimit-limit-tokens`) are only returned during inference requests (`/chat/completions`), not during model catalog discovery (`/models`).
   - In browser environments, CORS security policies block client scripts from reading custom HTTP response headers unless explicitly listed in `Access-Control-Expose-Headers`.
3. **Static Reference Fallback:**
   - A feasible approach for free tier rate limits is maintaining a curated `rate_limits.json` configuration mapping `{ provider, model_id }` to documented baseline limits (RPM, RPD, TPM), refreshed periodically.

### 4.2 CORS Constraints & Edge Proxy Role
- Where dynamic headers can be queried, the local CORS proxy (`proxy.py`) or the future production Cloudflare Worker (Milestone 0E-2) can expose `Access-Control-Expose-Headers: *`, allowing client-side telemetry capture.

### 4.3 Integration into Knowledge Graph & Routing Engine
- Telemetry metrics will serve two primary functions:
  1. **Visual Dimensions (`KG_column`):** Exposed as optional columns in Milestone 0C-6E / 0C-9 so users can sort by throughput or latency.
  2. **Routing Constraints:** Fed into the Model Routing & Recommendation Engine in Milestone 0D-2 to prevent recommending models whose rate limits cannot accommodate the user's workload.

---

## 5. TWO-LAYER NORMALIZATION ARCHITECTURAL ROADMAP

### 5.1 The Need for Two-Layer Normalization
The current 15-field `NormalizedModel` schema created by `_normalize.js` is a static canonical contract. While it stabilizes columns 0–5, it introduces rigidity:
- Any new metric (e.g. rate limits, KV cache support, novel benchmark suites) requires modifying `createNormalizedModel()`, updating all 9 provider adapters, and altering sorting hierarchies.
- Vendor-specific features that do not fit the 15 fields are lost during normalization.

### 5.2 Layer 1: Lossless Dynamic Ingestion (Heavy Lift)
- **Objective:** Ingest upstream provider payloads losslessly into structured raw records.
- **Scope:**
  - Dynamically capture all vendor properties, pricing tiers, endpoint capabilities, rate limits, and hardware backends.
  - Ingest all metrics from the **Multi-Source Benchmark Enrichment** sources (Artificial Analysis, LiveBench, HuggingFace Open LLM, BenchLM, BenchGecko, LMArena).
  - No information is clipped or discarded during the ingestion phase.

### 5.3 Layer 2: Interactive Semantic Mapping
- **Objective:** Client-side ontology mapping projecting Layer 1 attributes into matrix columns and filters.
- **Capabilities:**
  - User-driven mapping: Users can choose which Layer 1 attributes map to matrix columns (`KG_column`) and filter criteria (`KG_filter`).
  - Pre-configured profiles: Provide sensible default mappings (e.g. "Coding Focus", "Low Latency / High RPM", "Zero Cost Exploration").
  - Future-proof: Adapts to upstream API additions without requiring codebase refactoring.
- Scheduled as **Milestone 0D-1 (2-Layer Normalization Architecture — Heavy Lift)**.

---

## 6. MASTER ROADMAP OF REMAINING MILESTONES

### 6.1 Derivation Logic & Grouping Principles

The roadmap is organized into three sequential phases that balance immediate UI maturation with long-term engine architecture:

1. **Phase 0C (Phase II) — Matrix Maturation, Global Aggregation & Multi-Source Data Enrichment:**
   - **0C-6E (Dynamic Column UI):** Decouples single-provider rendering from the fixed 6-column layout, establishing dynamic column schema configuration.
   - **0C-6F (Multi-Provider Home Page & Global View):** Aggregate multi-cloud discovery root view. **Core Invariant:** Retains exact physical button positioning matching individual provider pages (Refresh, Estimate Refusal Rates, Export at top; Filter, Zoom at bottom), cascading functionality globally (e.g., Export outputs nested multi-provider JSON).
   - **0C-6G (Advanced Capability & Modality Filters):** Extends declarative filter engine with tri-state capability controls (`has_tools`, `has_files`) and input modality toggles across both provider and global views.
   - **0C-2 (Multi-Source Benchmark Enrichment):** Comprehensive multi-source benchmark ingestion spanning:
     - **Artificial Analysis:** Quality Index, Coding Index, Agentic Index
     - **LiveBench:** Free, hard benchmark suite (coding, reasoning, math, data analysis, instruction following)
     - **HuggingFace Open LLM Leaderboard:** Free, community-standard evaluation metrics (MMLU-Pro, IFEval, MuSR, MATH, GPQA, GSM8k)
     - **BenchLM:** Free tier benchmark evaluations
     - **BenchGecko:** Free tier comparative evaluation metrics
     - **LMArena:** Web-only crowdsourced Elo ratings (Chatbot Arena)
   - **0C-7 (Cross-Provider Refusal Rates):** Extends the existing `refreshRefusalRates` estimation logic to normalize model slugs across all providers, populating the Refusal Rates column across all non-OpenRouter models.
   - **0C-8 (Group B Provider Adapters):** Implements remaining 4 registry providers (Cloudflare Workers AI, Ollama, OVHcloud, IBM watsonx.ai).
   - **0C-9 (Telemetry & Rate Limit Ingestion):** Ingests RPM, RPD, TPM, and TTFT metrics via headers/endpoints with documented static fallback.

2. **Phase 0D — Heavy Lift: 2-Layer Normalization & Intelligent Routing Engine:**
   - **0D-1 (2-Layer Normalization Architecture — Heavy Lift):**
     - Refactors data ingestion into two clean architectural layers:
       - **Layer 1 (Lossless Dynamic Ingestion):** Dynamically captures all upstream provider properties, endpoints, pricing, rate limits, AND all evaluation fields from the newly-integrated **Multi-Source Benchmark Enrichment** sources (Artificial Analysis, LiveBench, HuggingFace, BenchLM, BenchGecko, LMArena) into raw, provider-faithful structures.
       - **Layer 2 (Interactive Semantic Mapping):** User-configurable ontology mapping projecting Layer 1 attributes into dynamic matrix columns (`KG_column`) and filter criteria (`KG_filter`).
   - **0D-2 (Model Routing & Recommendation Engine):**
     - Autonomous client-side model router evaluating user task constraints (free tier, context window, latency, benchmark thresholds, rate limits), computing multi-criteria Pareto-optimal scoring across ranked columns, and generating API connection snippets.

3. **Phase 0E — Tooling, Production Infrastructure & Release:**
   - **0E-1 (CLI Parity & Metadata Export Modernization):** Brings `cli.js` to universal 13-provider parity with CLI filtering, and modernizes `Export Data` JSON with provenance, timestamps, active filters, and schema versioning.
   - **0E-2 (Production Edge CORS Proxy Deployment):** Deploys lightweight edge proxy (e.g. Cloudflare Worker) to resolve Mixed Content blocking on live HTTPS origins (GitHub Pages).
   - **0E-3 (Production Release: GitHub Pages & Native APK):** Final push to `origin/main`, live GitHub Pages PWA deployment, signed Capacitor Android APK build, and v1.0.0 release tagging.

---

### 6.2 Master Roadmap Table

| Seq | Milestone ID | Milestone Name | Logical Phase / Group | High-Level Scope & Key Deliverables | Dependencies | Architectural Rationale & Invariants |
| :---: | :--- | :--- | :--- | :--- | :--- | :--- |
| **1** | **0C-6E** | **Dynamic Column UI (`KG_column`)** | Phase 0C: Matrix Maturation | - Replace fixed 6-column `thead` with dynamic, schema-driven column selection.<br>- Column visibility toggle popover/drawer.<br>- User-selected sort hierarchies across any numeric/comparable schema property.<br>- Persistent column layout per provider (`columnState_<providerId>`). | 0C-6D (Filter UI complete) | **Prerequisite for Home Page.** Decouples table structure from hardcoded column assumptions. Must precede Home Page to avoid redesigning multi-provider tables twice. |
| **2** | **0C-6F** | **Multi-Provider Home Page & Global View** | Phase 0C: Global Aggregation | - Root multi-provider matrix view aggregating top models across all enabled providers.<br>- **UI Parity Invariant:** Top controls (Refresh, Estimate Refusal Rates, Export) and bottom controls (Filter, Zoom) maintain exact physical positions as individual provider pages.<br>- Global functional cascade: Refresh triggers multi-provider fetch; Export downloads nested multi-provider JSON; Filter applies `filterState_global`. | 0C-6E | Core multi-cloud discovery payoff. Preserves spatial muscle memory and visual consistency across single-provider and global views. |
| **3** | **0C-6G** | **Advanced Capability & Modality Filters** | Phase 0C: Matrix Maturation | - Add `has_tools` (Tool Calling) and `has_files` (Vision) tri-state toggles (`Require`, `Exclude`, `Any`) to filter popover.<br>- Add input modality filter (Text, Image, Audio).<br>- Pure declarative configuration in `adapters/_filter.js` without HTML churn. | 0C-6D, 0C-6F | Expands declarative `FILTER_DEFINITIONS` established in 0C-6D. Operates seamlessly on both individual provider pages and the global Home Page. |
| **4** | **0C-2** | **Multi-Source Benchmark Enrichment** | Phase 0C: Data Enrichment | - Ingest multi-source benchmarks from: **Artificial Analysis**, **LiveBench** (Free, coding/reasoning), **HuggingFace Open LLM Leaderboard** (Free), **BenchLM** (Free tier), **BenchGecko** (Free tier), and **LMArena** (Web only).<br>- Cross-provider model slug normalization and fuzzy name resolution.<br>- Bundled offline snapshot dataset with manual update trigger. | 0C-6F | Eliminates `null` benchmark scores on non-OpenRouter models (Groq, Gemini, SambaNova, etc.) using diverse, authoritative public leaderboards. |
| **5** | **0C-7** | **Cross-Provider Refusal Rates** | Phase 0C: Safety & Refusal | - Extend existing `refreshRefusalRates` estimation logic to all non-OpenRouter providers.<br>- Cross-provider model slug normalization mapping proprietary/hosted endpoints to canonical model families.<br>- Populate the Refusal Rates column across all 9 Group A providers. | 0C-2 | Replaces `null` refusal estimates across non-OpenRouter models without altering the established estimation pipeline architecture. |
| **6** | **0C-8** | **Group B Provider Adapters (Custom APIs)** | Phase 0C: Provider Expansion | - Implement remaining 4 providers in `PROVIDER_REGISTRY`: Cloudflare Workers AI, Ollama (local server), OVHcloud, IBM watsonx.ai.<br>- Individual adapter modules under `adapters/<provider>/index.js`.<br>- Update sidebar drawer to mark Group B as active/ready. | 0C-1, 0C-6B | Completes universal 13-provider catalog coverage. |
| **7** | **0C-9** | **Telemetry & Rate Limit Ingestion** | Phase 0C: Data Enrichment | - Ingest model-level and account-level rate limits (RPM, RPD, TPM) and latency/TTFT.<br>- Dynamic HTTP response header parsing where CORS permits.<br>- Documented static reference fallback where endpoints omit limits. | 0C-8, 0C-6E | Supplies crucial throughput and capacity limits required for production model selection. |
| **8** | **0D-1** | **2-Layer Normalization Architecture (Heavy Lift)** | Phase 0D: Heavy Lift | - **Layer 1 (Lossless Dynamic Ingestion):** Dynamically capture unclipped upstream properties, endpoints, quotas, AND metadata from all 6 Multi-Source Benchmark Enrichment sources into provider-faithful raw records.<br>- **Layer 2 (Interactive Semantic Mapping):** User-configurable ontology mapping projecting Layer 1 attributes into dynamic matrix columns (`KG_column`) and filter criteria (`KG_filter`). | 0C-2, 0C-9, 0C-6E | Eliminates hardcoded 15-field schema rigidity. Enables client-side extensibility for any novel upstream metric or benchmark without codebase refactors. |
| **9** | **0D-2** | **Model Routing & Recommendation Engine** | Phase 0D: Heavy Lift | - Autonomous client-side model router evaluating user task constraints (free tier, context window, latency, benchmark thresholds, rate limits, modalities).<br>- Multi-criteria Pareto-optimal scoring across ranked columns.<br>- One-click "Copy API connection snippet" and agent dispatch configuration for top-recommended model. | 0D-1 | Transforms passive matrix dashboard into an active agentic dispatch intelligence engine. |
| **10** | **0E-1** | **CLI Parity & Metadata Export Modernization** | Phase 0E: Tooling & Release | - Upgrade `cli.js` from OpenRouter-only to universal 13-provider pipeline support.<br>- Add CLI filter flags (`--free-only`, `--chat-only`).<br>- Modernize `Export Data` payload to include provenance, timestamps, active filters, and schema version. | 0C-8, 0C-6D | Closes the divergence between CLI capabilities and web dashboard architecture. |
| **11** | **0E-2** | **Production Edge CORS Proxy Deployment** | Phase 0E: Production Infra | - Build and deploy lightweight Cloudflare Worker / Vercel Edge function to replace local `proxy.py`.<br>- Secure header relay for NVIDIA, SambaNova, and LLM7 on live HTTPS origins.<br>- Origin validation and rate-limiting safeguards. | 0C-8 | Solves Mixed Content blocking on live GitHub Pages (`https://` cannot query `http://localhost:8081`). |
| **12** | **0E-3** | **Production Release (GitHub Pages & Native APK)** | Phase 0E: Release | - Push clean local git history to `origin/main`.<br>- Deploy production PWA to GitHub Pages.<br>- Build, package, and sign release APK via Capacitor Android.<br>- Tag release `v1.0.0` and finalize user-facing documentation. | All prior milestones | Final delivery across web and mobile platforms. |

---

### 6.3 Detailed Scope Profiles for Key Milestones

#### Milestone 0C-6E: Dynamic Column UI (`KG_column`)
- **Objective:** Free the dashboard from the rigid 6-column matrix (Context, Thinking, Coding, Agentic, Summarizer, Refusal).
- **Key Deliverables:**
  - Column registry mapping model properties (`context_length`, `uptime`, `latency`, `intelligence_index`, `max_completion_tokens`, etc.) to column definitions with sort orders and formatters.
  - "Columns" toggle popover allowing users to check/uncheck visible columns.
  - Dynamic table header and row rendering accommodating arbitrary column counts (with responsive horizontal scrolling).
  - Storage key `columnState_<providerId>` maintaining per-provider column preferences.

#### Milestone 0C-6F: Multi-Provider Home Page & Global View
- **Objective:** Provide a holistic overview of the entire AI landscape across all 13 providers with strict UI parity.
- **Key Invariants & Layout Constraints:**
  - Pinned "All Providers (Home)" item at the top of the sidebar drawer (`.side-panel`).
  - **Identical Physical Button Layout:** All buttons remain in the exact same physical positions as individual provider pages:
    - Top bar: `Refresh` (`#refresh-btn`), `Estimate Refusal Rates` (`#refresh-refusal-btn`), and `Export Data` (`#export-btn`).
    - Bottom bar: `Filter` (`#filter-btn`) and `Zoom` (`#desktop-toggle-fab`).
  - **Global Cascades:**
    - `Refresh`: Sequentially / concurrently refreshes all configured provider adapters.
    - `Estimate Refusal Rates`: Runs estimation on the deduplicated cross-provider model pool.
    - `Export Data`: Downloads a single nested JSON document containing all cached providers' ranked columns, raw catalogs, and active filter states.
    - `Filter`: Anchored popover filtering across the entire unified model catalog via `filterState_global`.
    - `Zoom`: Toggles desktop scaling across the global table.

#### Milestone 0C-6G: Advanced Capability & Modality Filtering
- **Objective:** Add rich capability and modality toggles to the popover without modifying HTML layout.
- **Key Deliverables:**
  - Add `has_tools` group: `Tool Calling Required`, `Exclude Tools`, `Any`.
  - Add `has_files` group: `Vision / Files Required`, `Text Only`, `Any`.
  - Add `modality` group: Filter by input modality (`text`, `image`, `audio`).
  - Pure declarative extension in `adapters/_filter.js` (`FILTER_DEFINITIONS`) with zero regressions to default chat/free views.

#### Milestone 0C-2: Multi-Source Benchmark Enrichment
- **Objective:** Ingest comprehensive, multi-source evaluation metrics to eliminate `null` benchmark scores across all providers.
- **Multi-Source Data Providers:**
  1. **Artificial Analysis:** Quality Index, Coding Index, Agentic Index.
  2. **LiveBench:** Free, hard benchmark suite testing reasoning, coding, math, data analysis, and instruction following.
  3. **HuggingFace Open LLM Leaderboard:** Free, community-standard evaluation metrics (MMLU-Pro, IFEval, MuSR, MATH, GPQA, GSM8k).
  4. **BenchLM:** Free tier benchmark evaluations.
  5. **BenchGecko:** Free tier comparative evaluation metrics.
  6. **LMArena:** Web-only crowdsourced Elo ratings (Chatbot Arena).
- **Key Deliverables:**
  - Multi-source bundled offline dataset with scheduled/manual update scripts.
  - Cross-provider slug normalizer matching provider endpoints (e.g., `meta-llama/Llama-3.3-70B-Instruct` on SambaNova vs `llama-3.3-70b-versatile` on Groq) to canonical benchmark records.
  - Blended/categorized score calculation for display in ranked columns.

#### Milestone 0C-7: Cross-Provider Refusal Rates
- **Objective:** Extend refusal estimation across all non-OpenRouter providers.
- **Key Deliverables:**
  - Model slug normalizer mapping provider-specific model identifiers to canonical model families.
  - Extended `refreshRefusalRates()` function that batches unique canonical slugs across all active providers.
  - Populate `cached_refusalRates` and fill the Refusal Rates column across all 9 Group A providers (Groq, Gemini, SambaNova, Mistral, Cohere, LLM7, ModelScope, NVIDIA NIM), eliminating `null` displays.

#### Milestone 0D-1: 2-Layer Normalization Architecture (Heavy Lift)
- **Objective:** Completely eliminate schema rigidity by refactoring data ingestion into two distinct layers.
- **Layer 1: Lossless Dynamic Ingestion:**
  - Normalizers ingest all raw vendor attributes, endpoints, quotas, and headers dynamically into unconstrained records.
  - **Multi-Source Benchmark Ingestion:** Seamlessly captures all fields from the newly added benchmark sources (Artificial Analysis, LiveBench, HuggingFace, BenchLM, BenchGecko, LMArena).
- **Layer 2: Interactive Semantic Mapping:**
  - Client-side mapping engine allowing users to configure which Layer 1 attributes map to matrix columns (`KG_column`) and filter criteria (`KG_filter`).
  - Future-proofs the application against upstream API changes without code edits.

#### Milestone 0D-2: Model Routing & Recommendation Engine
- **Objective:** Transform the passive matrix into an active model dispatch engine.
- **Key Deliverables:**
  - Client-side heuristic router evaluating task prompts or explicit constraints (cost tier, context window, latency, benchmark thresholds, rate limits, modalities).
  - Multi-criteria Pareto-optimal scoring algorithm across ranked columns.
  - One-click "Copy API connection snippet" and agent dispatch configuration for the top-recommended model.
