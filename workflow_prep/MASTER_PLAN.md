# Top_Models: Master Architecture Plan, Roadmap & Milestone Execution Specs

**Target File:** `~/storage/downloads/Sync/MASTER_PLAN.md`  
**Document Role:** Canonical authority for forward-looking milestone requirements, roadmap sequencing, cache version ledgers, and execution specifications.
**Status:** CANONICAL FORWARD EXECUTION ROADMAP & UNIFIED MILESTONE SPECS  
**Author:** AI Architecture & Execution Pair (Argon / DeepSeek / Antigravity)  
**Date:** October 2026  
**Reference Document:** `~/storage/downloads/Sync/codebase_1.md` (Current Architecture & Technical Baseline)  
**Baseline Git Commit:** `942bb06` (`Milestone 0C-6D: Implement in-memory filter UI, model-bound extended rows, and event delegation`)  
**Active Cache & Script State:** `core.js?v=0I`, `matrix-cache-v11`  

---

## DOCUMENT PURPOSE & ARCHITECTURAL CONTRACT

This document represents the definitive, unified master plan for `Top_Models`. It merges strategic forward planning, technical backlog curation, and execution-ready milestone specifications into a single building artifact.

- **Part 1 (Master Roadmap, Backlog & Cross-Milestone Invariants):** Synthesizes project context, retained backlog items (each mapped to its execution spec), architectural research (telemetry, rate limits, 2-layer normalization), the 12-milestone sequencing matrix, and the canonical **Version, Service Worker & Build Sync Ledger**.
- **Part 2 (Unified Milestone Execution Specs 2.1 through 2.12):** Provides deep, self-contained, implementation-grade specifications for all remaining 12 milestones (`0C-6E` through `0E-3`). Each spec is structured with four non-negotiable sections:
  1. *Objective & Scope* (Deliverables and target file changes)
  2. *Architecture & Integration Details* (Data models, state transitions, DOM contracts, and mandatory cross-milestone bridges)
  3. *Execution Directives & Safeguards* (Strict "DO NOTs", cache busting, SW precaching, and `codebase_1.md` updates)
  4. *Two-Party Verification Protocol* (Automated CLI/node checks for the agent and physical browser/device tests for the user)

---

# PART 1: MASTER ROADMAP, BACKLOG & CROSS-MILESTONE INVARIANTS

## 1. IMPLEMENTATION ARCHIVE REFERENCE (MILESTONE 0C-6D)

Milestone 0C-6D established the dynamic in-memory filtering architecture and interaction foundation:
- **Verified Commit:** `942bb06` (`Milestone 0C-6D: Implement in-memory filter UI, model-bound extended rows, and event delegation`).
- **Canonical Architecture Reference:** Consolidated in `~/storage/downloads/Sync/codebase_1.md`.
- **Implemented Capabilities Summary:**
  - `adapters/_filter.js`: Pure declarative engine exporting `FILTER_DEFINITIONS`, `DEFAULT_FILTER_STATE`, and `applyModelFilters()`.
  - `core.js`: Public ESM facade re-exporting the filter engine alongside sorting and normalization.
  - `index.html`: Anchored floating filter popover (`#filter-popover`), active dot indicator (`#filter-active-dot`), dynamic counter indicator (`#model-count-indicator`) supporting 3 runtime states, empty-state card with embedded reset trigger (`#empty-state-reset-btn`), atomic 8-step `handleFilterReset()`, and event delegation on `<tbody id="table-body">` with model-bound extended rows (`appState.expanded = { modelId, colIndex }`).
  - Cache & Build Integrity: Service Worker bumped to `matrix-cache-v11` with `./adapters/_filter.js` precached; `index.html` import bumped to `./core.js?v=0I`.

---

## 2. DEFERRED BACKLOG & INTERACTION ENHANCEMENTS

Every deferred feature from previous milestones is mapped to its target execution spec in Part 2:

### 2.1 Capability Filter Extension (`has_tools`, `has_files`, Modalities)
- **Scope:** Vision / File Ingestion (`has_files: 1 | 0`), Tool / Function Calling (`has_tools: 1 | 0`), and input modality toggles (`text`, `image`, `audio`).
- **Semantics:** Tri-state controls (`any`, `require`, `exclude`) evaluating normalized model properties.
- **Target Execution Spec:** **Part 2, Spec 2.3 (Milestone 0C-6G: Advanced Capability & Modality Filters)**.

### 2.2 Global Filter State & Multi-Provider Aggregation
- **Scope:** Cross-provider model aggregation under `activeProvider === 'all'`, applying `filterState_global` and `columnState_global` stored in `localStorage`.
- **Sequencing Invariant:** Must follow Dynamic Column UI (`0C-6E`) to avoid redesigning table layouts twice.
- **Target Execution Spec:** **Part 2, Spec 2.2 (Milestone 0C-6F: Multi-Provider Home Page & Global View)**.

### 2.3 Cross-Tab & Multi-PWA Storage Synchronization
- **Scope:** Window `storage` event listener keeping multiple tabs or installed PWA instances in sync when filter states, column configurations, or active providers change.
- **Target Execution Spec:** **Part 2, Spec 2.2 (Milestone 0C-6F: Multi-Provider Home Page & Global View)**.

### 2.4 Modernized Export Payload with Provenance
- **Scope:** Upgrade `Export Data` button and CLI `models fetch` to emit rich JSON with ISO8601 timestamps, active provider, active filter/column criteria snapshot, model counts, and schema versioning.
- **Target Execution Spec:** **Part 2, Spec 2.10 (Milestone 0E-1: CLI Parity & Metadata Export Modernization)**.

---

## 3. PROVIDER ADAPTER TECHNICAL DEBT & METADATA PARITY

An audit of the 9 implemented Group A provider adapters identified metadata debts that must be resolved prior to or during filter and data enrichment:

### 3.1 Dynamic `is_chat` Derivation
- **OpenRouter (`adapters/openrouter/index.js`):** Hardcodes `is_chat: true` for all models without verifying architecture or endpoint types. Non-chat completions or embeddings must be detected dynamically.
- **SambaNova (`adapters/sambanova/index.js`):** Hardcodes `is_chat: true` across all models.
- **Resolution Plan:** Inspect model architecture, endpoint capabilities, and modality descriptions during Stage 1 normalization.
- **Target Execution Spec:** **Part 2, Spec 2.3 (Milestone 0C-6G: Advanced Capability & Modality Filters)**.

### 3.2 Advanced Capability Detection
- **Groq (`adapters/groq/index.js`):** Checks `supported_features.includes('tools')`, but omits reasoning token extraction and structured JSON output capability flags present in upstream metadata.
- **Google Gemini (`adapters/gemini/index.js`):** Hardcodes `has_tools: null` despite native `generateContent` tool/function calling support across Gemini 1.5 Pro / Flash.
- **Mistral AI (`adapters/mistral/index.js`):** Capabilities dictionary should be fully parsed for system prompt support and function calling.
- **Target Execution Spec:** **Part 2, Spec 2.3 (Milestone 0C-6G: Advanced Capability & Modality Filters)**.

### 3.3 Dynamic Modality Parsing
- **SambaNova:** Hardcodes `raw_modalities: "text"` despite hosting multimodal models (e.g. Llama 3.2 11B/90B Vision). Dynamic string construction (`text,image`) is required.
- **Target Execution Spec:** **Part 2, Spec 2.3 (Milestone 0C-6G: Advanced Capability & Modality Filters)**.

### 3.4 CLI Multi-Provider Parity Debt
- **`cli.js` Divergence:** CLI remains hardcoded to OpenRouter `fetchData` and lacks multi-provider switching, key configuration for other providers, and CLI filter flags (`--free-only`, `--chat-only`, `--columns`).
- **Target Execution Spec:** **Part 2, Spec 2.10 (Milestone 0E-1: CLI Parity & Metadata Export Modernization)**.

---

## 4. TELEMETRY & RATE LIMIT RESEARCH (TTFT, RPM, RPD, TPM)

### 4.1 Ingestion Feasibility Audit Across Group A Providers
A comprehensive audit confirmed that zero providers expose TTFT, RPM, RPD, or TPM directly inside their `/models` catalog endpoints.

#### Key Architectural Findings:
1. **Tier/Account Governance vs Catalog Metadata:**
   - Providers (Groq, Gemini, SambaNova, Mistral, Cohere) enforce rate limits at the API key / account tier level. Catalog discovery endpoints (`/models`) do not return limit numbers.
2. **Inference Header Extraction Constraints:**
   - Rate limit headers (e.g., `x-ratelimit-remaining-requests`, `x-ratelimit-limit-tokens`, `retry-after`) are returned only on inference endpoints (`/chat/completions`), not discovery.
   - In browser environments, CORS security policies block client JavaScript from reading custom response headers unless explicitly permitted via `Access-Control-Expose-Headers`.
3. **Static Baseline Dataset Requirement:**
   - To provide reliable rate limits for free tier models without spamming inference endpoints, a curated reference dataset (`rate_limits.json`) mapping `{ provider, model_id }` to documented limits (RPM, RPD, TPM) must serve as the primary baseline, supplemented by dynamic response header extraction during live calls.
- **Target Execution Spec:** **Part 2, Spec 2.7 (Milestone 0C-9: Telemetry & Rate Limit Ingestion)**.

---

## 5. TWO-LAYER NORMALIZATION ARCHITECTURAL ROADMAP

### 5.1 Schema Rigidity in the 15-Field Normalization Schema
The current `createNormalizedModel()` schema enforces a rigid 15-field contract. While this stabilized initial dashboard columns, it creates major friction:
- New metrics (benchmarks, rate limits, latency, KV cache limits) require mutating the schema, modifying all provider adapters, and updating sorting hierarchies.
- Vendor-specific features (e.g., reasoning tokens, speculative decoding, specialized license tiers) are lost during normalization.

### 5.2 Layer 1: Lossless Dynamic Ingestion
- Ingest upstream provider payloads losslessly into structured raw records.
- Preserve all vendor-specific metadata, hardware endpoints, pricing tiers, and multi-source benchmark scores without clipping.

### 5.3 Layer 2: Interactive Semantic Mapping
- Client-side ontology mapping projecting Layer 1 attributes into dynamic matrix columns (`KG_column`) and filter criteria (`KG_filter`).
- Enables custom user profiles ("Coding Focus", "Low Latency Free Tier", "Agentic Tool Use") without code modifications.
- **Target Execution Spec:** **Part 2, Spec 2.8 (Milestone 0D-1: 2-Layer Normalization Architecture — Heavy Lift)**.

---

## 6. MASTER ROADMAP OF REMAINING MILESTONES

### 6.1 Derivation Logic & Sequential Phases
1. **Phase 0C — Matrix Maturation, Global Aggregation & Multi-Source Data Enrichment:**
   - `0C-6E`: Dynamic Column UI (`KG_column`) — Decouples table from fixed 6 columns.
   - `0C-6F`: Multi-Provider Home Page & Global View — Aggregates multi-cloud matrix with strict UI parity.
   - `0C-6G`: Advanced Capability & Modality Filters — Extends declarative filters and fixes Group A metadata debt.
   - `0C-2`: Multi-Source Benchmark Enrichment — Integrates 6 public benchmark suites with canonical model slug normalization.
   - `0C-7`: Cross-Provider Refusal Rates — Expands refusal rate estimation across all providers via canonical slug matching.
   - `0C-8`: Group B Provider Adapters — Implements Cloudflare, Ollama, OVHcloud, IBM watsonx.ai.
   - `0C-9`: Telemetry & Rate Limit Ingestion — Integrates RPM, RPD, TPM, and TTFT metrics via hybrid header/static data.
2. **Phase 0D — Heavy Lift: 2-Layer Normalization & Intelligent Routing Engine:**
   - `0D-1`: 2-Layer Normalization Architecture — Refactors ingestion into Layer 1 (Lossless) and Layer 2 (Semantic Projection).
   - `0D-2`: Model Routing & Recommendation Engine — Client-side Pareto-optimal recommendation and API snippet generator.
3. **Phase 0E — Tooling, Production Infrastructure & Release:**
   - `0E-1`: CLI Parity & Metadata Export Modernization — Universal 13-provider CLI and rich export JSON.
   - `0E-2`: Production Edge CORS Proxy Deployment — Cloudflare Worker deployment resolving HTTPS Mixed Content.
   - `0E-3`: Production Release (GitHub Pages & Native APK) — PWA deploy, signed Capacitor APK build, `v1.0.0` release.

### 6.2 Master Roadmap Table

| Seq | Milestone ID | Milestone Name | Logical Phase | Dependencies | Target Spec | Core Invariants & Key Deliverables |
| :---: | :--- | :--- | :--- | :--- | :---: | :--- |
| **1** | **0C-6E** | **Dynamic Column UI (`KG_column`)** | Phase 0C | 0C-6D | **Spec 2.1** | Min 1 column invariant; Popover mutual exclusion; Declarative `_columns.js`; In-memory dynamic ranking; Model-bound expansion reconciliation. |
| **2** | **0C-6F** | **Multi-Provider Home Page & Global View** | Phase 0C | 0C-6E | **Spec 2.2** | Core UI Parity Invariant (exact button layout); Composite model IDs (`<provider>:<model>`); Provider badges; Resilient global fetch; Cross-tab sync. |
| **3** | **0C-6G** | **Advanced Capability & Modality Filters** | Phase 0C | 0C-6D, 0C-6F | **Spec 2.3** | Declarative `FILTER_DEFINITIONS` extension (`has_tools`, `has_files`, modalities); Resolve Group A metadata debt across 9 adapters. |
| **4** | **0C-2** | **Multi-Source Benchmark Enrichment** | Phase 0C | 0C-6F | **Spec 2.4** | Canonical cross-provider slug normalizer (`_slug.js`); 6 benchmark sources (Artificial Analysis, LiveBench, HF, BenchLM, BenchGecko, LMArena). |
| **5** | **0C-7** | **Cross-Provider Refusal Rates** | Phase 0C | 0C-2 | **Spec 2.5** | Cross-provider refusal estimation reusing `_slug.js`; Authenticates via `api_key_openrouter` or falls back to bundled `refusal_rates.json`. |
| **6** | **0C-8** | **Group B Provider Adapters (Custom APIs)** | Phase 0C | 0C-1, 0C-6B | **Spec 2.6** | Implement Cloudflare Workers AI, Ollama (direct `127.0.0.1:11434`), OVHcloud, IBM watsonx.ai; Update registry and sidebar badges. |
| **7** | **0C-9** | **Telemetry & Rate Limit Ingestion** | Phase 0C | 0C-8, 0C-6E | **Spec 2.7** | Hybrid ingestion: response headers via CORS proxy `Expose-Headers` + curated `rate_limits.json` static baseline; Add RPM, RPD, TPM, TTFT columns. |
| **8** | **0D-1** | **2-Layer Normalization Architecture** | Phase 0D | 0C-2, 0C-9, 0C-6E | **Spec 2.8** | Layer 1 Lossless dynamic ingestion; Layer 2 Semantic mapping onto `_columns.js` and `_filter.js`; `schema_version` cache migration guard. |
| **9** | **0D-2** | **Model Routing & Recommendation Engine** | Phase 0D | 0D-1 | **Spec 2.9** | Client-side heuristic router evaluating constraints (cost, ctx, TTFT, benchmarks); Multi-criteria Pareto scoring; One-click API code snippet generator. |
| **10** | **0E-1** | **CLI Parity & Metadata Export Modernization** | Phase 0E | 0C-8, 0C-6D | **Spec 2.10** | Universal 13-provider CLI subcommands (`keys`, `refresh`, `estimate`, `fetch`); CLI filter flags; Rich export metadata format with native Capacitor share. |
| **11** | **0E-2** | **Production Edge CORS Proxy Deployment** | Phase 0E | 0C-8 | **Spec 2.11** | Deploy Cloudflare Worker Edge Proxy; Origin locking & header relay; Client runtime proxy resolution (Termux `8080` vs GitHub Pages HTTPS vs Capacitor). |
| **12** | **0E-3** | **Production Release (GitHub Pages & Native APK)** | Phase 0E | All prior | **Spec 2.12** | Final git push to `origin/main`; GitHub Pages live PWA; Signed Capacitor Android release APK (`v1.0.0`); User documentation. |

---

## 7. VERSION, SERVICE WORKER & BUILD SYNC LEDGER

Every milestone modifying JavaScript modules, HTML structure, or precached static assets MUST advance the cache-busting version query string and update `sw.js` `CACHE_NAME`. Furthermore, any newly introduced asset must be registered in both `sw.js` and `sync-www.js` to ensure 100% offline parity for both the PWA and the Capacitor Android APK build.

| Milestone ID | Target Milestone Name | `index.html` Import | `sw.js` `CACHE_NAME` | New Precached Assets (`sw.js`) | `sync-www.js` Asset Registration | Build & Sync Commands |
| :---: | :--- | :---: | :---: | :--- | :--- | :--- |
| **0C-6D** | *Filter UI & Extended Rows (Current)* | `core.js?v=0I` | `matrix-cache-v11` | `./adapters/_filter.js` | Mirrored via `adapters/` | `npm run build:web` |
| **0C-6E** | Dynamic Column UI (`KG_column`) | `core.js?v=0J` | `matrix-cache-v12` | `./adapters/_columns.js` | Mirrored via `adapters/` | `node --check core.js && npm run build:web` |
| **0C-6F** | Multi-Provider Home Page & Global View | `core.js?v=0K` | `matrix-cache-v13` | None (Updates to existing modules) | Mirrored via `adapters/` | `node --check core.js && npm run build:web` |
| **0C-6G** | Advanced Capability & Modality Filters | `core.js?v=0L` | `matrix-cache-v14` | None (Updates to `_filter.js` & adapters) | Mirrored via `adapters/` | `node --check core.js && npm run build:web` |
| **0C-2** | Multi-Source Benchmark Enrichment | `core.js?v=0M` | `matrix-cache-v15` | `./adapters/_slug.js`, `./benchmarks/benchmarks_data.json` | Add `benchmarks/` copy step to `sync-www.js` | `node --check core.js && npm run build:web` |
| **0C-7** | Cross-Provider Refusal Rates | `core.js?v=0N` | `matrix-cache-v16` | `./refusal_rates.json` | Verify `refusal_rates.json` copy step in `sync-www.js` (already conditionally included; add only if absent) | `node --check core.js && npm run build:web` |
| **0C-8** | Group B Provider Adapters (Custom APIs) | `core.js?v=0O` | `matrix-cache-v17` | `./adapters/cloudflare/index.js`, `./adapters/ollama/index.js`, `./adapters/ovh/index.js`, `./adapters/watsonx/index.js` | Mirrored via `adapters/` | `node --check core.js && npm run build:web` |
| **0C-9** | Telemetry & Rate Limit Ingestion | `core.js?v=0P` | `matrix-cache-v18` | `./rate_limits.json` | Add `rate_limits.json` copy step to `sync-www.js` | `node --check core.js && npm run build:web` |
| **0D-1** | 2-Layer Normalization Architecture | `core.js?v=0Q` | `matrix-cache-v19` | `./adapters/_layer1.js`, `./adapters/_layer2.js` | Mirrored via `adapters/` | `node --check core.js && npm run build:web` |
| **0D-2** | Model Routing & Recommendation Engine | `core.js?v=0R` | `matrix-cache-v20` | `./adapters/_router.js` | Mirrored via `adapters/` | `node --check core.js && npm run build:web` |
| **0E-1** | CLI Parity & Metadata Export Modernization | `core.js?v=0S` | `matrix-cache-v21` | None (Updates to `core.js`, `index.html`) | Mirrored via `adapters/` | `node --check cli.js core.js && npm run build:web` |
| **0E-2** | Production Edge CORS Proxy Deployment | `core.js?v=0T` | `matrix-cache-v22` | None (Runtime proxy resolution update) | Mirrored via `adapters/` | `node --check core.js && npm run build:web` |
| **0E-3** | Production Release (GitHub Pages & Native APK) | `core.js?v=1.0.0` | `matrix-cache-v1.0.0` | Full audit of all precached assets | Full sync & verification of `www/` | `npm run build:web && npx cap sync android` |

---

# PART 2: UNIFIED MILESTONE EXECUTION SPECS (2.1 THROUGH 2.12)

```
================================================================================
PART 2 STRUCTURAL CONTRACT:
Every Milestone Execution Spec contains four required subsections:
  1. Objective & Scope (Exact deliverables and target files to create or modify)
  2. Architecture & Integration Details (Module boundaries, exported symbols, DOM hooks, state mutations, and cross-milestone architectural bridges)
  3. Execution Directives & Safeguards (The strict Prompt Rules, DO NOTs, cache busting, and documentation integrity)
  4. Two-Party Verification Protocol (Automated checks for the agent, mobile interactive steps for the user)
================================================================================
```

---

## 2.1 MILESTONE 0C-6E: DYNAMIC COLUMN UI (`KG_column`)

### 1. Objective & Scope
- **Objective:** Liberate the dashboard from the hardcoded 6-column table layout by implementing dynamic, user-configurable column selection (`KG_column`), allowing arbitrary visible column configurations with responsive horizontal scrolling, dynamic ranking, and persistent per-provider layout preferences.
- **Target Files to Create / Modify:**
  - `adapters/_columns.js` (NEW): Declarative column registry, default column states, formatter utilities, and dynamic ranking functions.
  - `adapters/_sorting.js` (PRESERVE): Safeguard #1 applies. Keep `sortHierarchy[0..5]` intact for backwards compatibility; extend or wrap for dynamic sorting.
  - `adapters/_pipeline.js` (PRESERVE): Ensure `runProviderPipeline` remains compatible, continuing to return `rankedColumns` 0..5 while supporting dynamic in-memory column ranking.
  - `core.js` (MODIFY): Re-export column definitions, default state, and column sorting helpers.
  - `index.html` (MODIFY): Add `#columns-btn`, `#columns-active-dot`, and `#columns-popover` inside `.table-actions-bar`. Implement dynamic `thead` generation, dynamic `renderTable()`, model-bound extended row reconciliation, dynamic `colspan`, and Popover Mutual Exclusion.
  - `sw.js` (MODIFY): Bump cache to `matrix-cache-v12`, add `./adapters/_columns.js` to `ASSETS_TO_CACHE`.
  - `sync-www.js` (EXECUTE): Run `npm run build:web` to mirror `adapters/_columns.js` to `www/adapters/`.

---

### 2. Architecture & Integration Details

#### 2.1.1 Declarative Column Registry (`adapters/_columns.js`)
Mirror the declarative pattern of `adapters/_filter.js` to ensure clean forward-compatibility with Milestone `0D-1` (Layer 2 semantic mapping):

```javascript
// adapters/_columns.js
export const COLUMN_DEFINITIONS = [
    {
        id: 'context_length',
        label: 'Context Window',
        shortLabel: 'Context',
        key: 'context_length',
        sortDirection: 'desc',
        fallback: -999999,
        defaultVisible: true,
        formatter: (val) => formatNumeric(val)
    },
    {
        id: 'intelligence_index',
        label: 'Thinking',
        shortLabel: 'Thinking',
        key: 'intelligence_index',
        sortDirection: 'desc',
        fallback: -999999,
        defaultVisible: true,
        formatter: (val) => formatNumeric(val)
    },
    {
        id: 'coding_index',
        label: 'Coding',
        shortLabel: 'Coding',
        key: 'coding_index',
        sortDirection: 'desc',
        fallback: -999999,
        defaultVisible: true,
        formatter: (val) => formatNumeric(val)
    },
    {
        id: 'agentic_index',
        label: 'Agentic',
        shortLabel: 'Agentic',
        key: 'agentic_index',
        sortDirection: 'desc',
        fallback: -999999,
        defaultVisible: true,
        formatter: (val) => formatNumeric(val)
    },
    {
        id: 'max_completion_tokens',
        label: 'Summarizer / Max Output',
        shortLabel: 'Summarizer',
        key: 'max_completion_tokens',
        sortDirection: 'desc',
        fallback: -999999,
        defaultVisible: true,
        formatter: (val) => formatNumeric(val)
    },
    {
        id: 'refusal_rate',
        label: 'Refusal Rates',
        shortLabel: 'Refusal',
        key: 'refusal_rate',
        sortDirection: 'asc', // Lower refusal is ranked higher
        fallback: 999999,      // Ascending sentinel (+999999) pushes nulls to bottom
        defaultVisible: true,
        formatter: (val) => formatPercentage(val)
    },
    {
        id: 'uptime',
        label: 'Uptime',
        shortLabel: 'Uptime',
        key: 'uptime',
        sortDirection: 'desc',
        fallback: -999999,
        defaultVisible: false,
        formatter: (val) => formatPercentage(val)
    },
    {
        id: 'latency',
        label: 'Latency',
        shortLabel: 'Latency',
        key: 'latency',
        sortDirection: 'asc',
        fallback: 999999,
        defaultVisible: false,
        formatter: (val) => (val !== null && val !== undefined && val !== 999999) ? `${val}ms` : '-'
    },
    {
        id: 'raw_modalities',
        label: 'Modalities',
        shortLabel: 'Modalities',
        key: 'raw_modalities',
        sortDirection: 'desc',
        fallback: '',
        defaultVisible: false,
        formatter: (val) => val || '-'
    }
];

export const DEFAULT_COLUMN_STATE = [
    'context_length',
    'intelligence_index',
    'coding_index',
    'agentic_index',
    'max_completion_tokens',
    'refusal_rate'
];
```

#### 2.1.2 Dynamic Column Ranking & Pipeline Safeguards
- **Safeguard #1 Strict Adherence:** `adapters/_sorting.js` is NOT modified.
- For dynamic columns, `adapters/_columns.js` exports `sortModelsForDynamicColumn(models, colDef)`:
  - If `colDef.sortDirection === 'asc'`, missing values (`null`, `undefined`, `NaN`) map to `+999999` so they sink to the bottom of the table.
  - If `colDef.sortDirection === 'desc'`, missing values map to `-999999`.
  - Secondary tie-breakers resolve gracefully using `context_length` and model ID.
- Dynamic matrix generation in `index.html`:
  - `appState.activeColumns`: Array of active column IDs (retrieved from `columnState_<providerId>`).
  - `appState.rankedColumnsDynamic`: Map or array keyed by active column index/ID containing sorted arrays of `appState.displayModels`.

#### 2.1.3 Minimum 1 Visible Column Invariant & Reset UX
- **The Invariant:** At all times, at least one column MUST remain checked.
- If a user attempts to uncheck the sole remaining active column checkbox in `#columns-popover`, the action is intercepted:
  - The checkbox remains checked.
  - A brief visual tooltip or warning appears: `"At least one column must remain visible."`
- **Atomic Reset (`handleColumnReset`):**
  1. Reset `appState.activeColumns` to `[...DEFAULT_COLUMN_STATE]`.
  2. Persist to storage via `safeSetItem('columnState_' + appState.activeProvider, JSON.stringify(appState.activeColumns))`.
  3. Re-sync all checkbox elements in `#columns-popover`.
  4. Hide `#columns-active-dot`.
  5. Recompute dynamic ranking and invoke `renderTable()`.

#### 2.1.4 Popover Mutual Exclusion & Dismissal Lifecycle
- In `.table-actions-bar`, add `#columns-btn` alongside `#filter-btn` and `#desktop-toggle-fab`:
  ```html
  <div class="columns-btn-container">
      <button id="columns-btn" title="Configure visible columns" aria-haspopup="true" aria-expanded="false">
          Columns <span id="columns-active-dot" class="columns-dot hidden">•</span>
      </button>
      <div id="columns-popover" class="columns-popover hidden" role="region" aria-labelledby="columns-popover-title">
          <div class="columns-popover-header">
              <span id="columns-popover-title" class="columns-title">Visible Columns</span>
              <button id="columns-close-btn" class="close-btn" aria-label="Close columns">&times;</button>
          </div>
          <div id="columns-popover-body" class="columns-popover-body"></div>
          <div class="columns-popover-footer">
              <button id="columns-reset-btn" class="columns-reset-btn">Reset to Default</button>
          </div>
      </div>
  </div>
  ```
- **Mutual Exclusion Rule:**
  - Clicking `#filter-btn` checks if `#columns-popover` is open; if so, it closes `#columns-popover` before toggling `#filter-popover`.
  - Clicking `#columns-btn` checks if `#filter-popover` is open; if so, it closes `#filter-popover` before toggling `#columns-popover`.
  - Pointerdown outside `.filter-btn-container` and `.columns-btn-container` closes both popovers.
  - Pressing `Escape` closes whichever popover is currently open.

#### 2.1.5 Table Rendering, Dynamic Colspan & Extended Row Reconciliation
- **Dynamic Table Header (`#table-head`):**
  - Generates `<th>` elements dynamically matching `appState.activeColumns`.
- **Dynamic Empty-State Colspan:**
  - When zero models match active filters, the empty-state card `<td colspan="${appState.activeColumns.length}">` spans the exact count of active columns.
- **Model-Bound Extended Row Lifecycle:**
  - `appState.expanded` stores `{ modelId, colKey }` (using string `colKey` instead of fragile numerical index).
  - Extended row `<tr class="extended-row">` renders all primary values for the active columns, followed by auxiliary attributes:
    - Auxiliary metrics: `Modalities`, `Uptime`, `Latency`.
    - **Non-Duplication Rule:** If `uptime`, `latency`, or `raw_modalities` is already active as a primary visible column in `appState.activeColumns`, it is omitted from the extended auxiliary cells at the end of the row to prevent confusing duplicate displays.
    - If active auxiliary columns are added, `<th>` headers for auxiliary columns are appended to the header row only while extended rows are expanded.

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **DO NOT modify `adapters/_sorting.js` core logic.** Wrap or supplement it via `adapters/_columns.js`.
2. **DO NOT modify `adapters/_normalize.js` without schema agreement.**
3. **DO NOT use inline `onclick` attributes.** All checkbox changes, reset clicks, and extend toggles must use scoped `addEventListener` or event delegation on `<tbody id="table-body">`.
4. **DO NOT allow 0 visible columns.** Enforce the minimum 1 column invariant unconditionally.
5. **Preserve Quota-Safe Storage:** Always write storage keys (`columnState_<providerId>`) using safe try/catch wrapper preventing quota exceptions.
6. **Precache & Cache Busting:**
   - Update `index.html` script import to `./core.js?v=0J`.
   - Update `sw.js` `CACHE_NAME` to `matrix-cache-v12` and precache `./adapters/_columns.js`.
   - Run `npm run build:web` to mirror files into `www/`.
7. **Post-Milestone Handover:** Update `codebase_1.md` with new `adapters/_columns.js` specification, DOM layout, and updated git state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Syntax check core and column modules
node --check adapters/_columns.js
node --check core.js

# 2. Build sync to Capacitor www directory
npm run build:web

# 3. Verify sw.js precache array contains _columns.js
grep -q "_columns.js" sw.js && echo "SW Precache Verified"
```

#### User Mobile Verification (`http://localhost:8080`):
1. **Column Toggle Test:** Open browser at `http://localhost:8080`. Tap the `Columns` button in the bottom bar. Verify `#columns-popover` opens cleanly and `#filter-popover` is not open.
2. **Mutual Exclusion Test:** With `#columns-popover` open, tap `Filter`. Verify `#columns-popover` closes immediately as `#filter-popover` opens.
3. **Column Invariant Test:** In `#columns-popover`, uncheck columns one by one until only 1 remains. Attempt to uncheck the last column. Verify it cannot be unchecked and the table never renders 0 columns.
4. **Active Dot Test:** With non-default columns visible, verify `#columns-active-dot` is visible. Tap `Reset to Default`. Verify defaults restore and dot disappears.
5. **Extended Row Test:** Tap `Extend` on any model cell. Verify the extended row matches the active column count without layout breakage or duplicate cells for promoted columns.

---

## 2.2 MILESTONE 0C-6F: MULTI-PROVIDER HOME PAGE & GLOBAL VIEW

### 1. Objective & Scope
- **Objective:** Establish the root multi-provider global view (`activeProvider === 'all'`) aggregating top models across all configured providers into a unified comparative matrix while maintaining absolute UI parity with single-provider views.
- **Target Files to Create / Modify:**
  - `adapters/_registry.js` (MODIFY): Add global provider descriptor (`id: 'all'`, `name: 'All Providers (Global)'`).
  - `adapters/_pipeline.js` (MODIFY): Export `runGlobalPipeline(configuredProviders, storageAdapter)` orchestrating multi-provider execution with failure isolation.
  - `core.js` (MODIFY): Re-export global pipeline and aggregation helpers.
  - `index.html` (MODIFY): Add pinned "All Providers (Home)" option in `.side-panel`, implement composite model keys (`<providerId>:<modelId>`), cell provider badges, header UX adaptation, global refresh with `Promise.allSettled()`, and cross-tab storage listener.
  - `sw.js` (MODIFY): Bump cache to `matrix-cache-v13`.
  - `sync-www.js` (EXECUTE): Run `npm run build:web`.

---

### 2. Architecture & Integration Details

#### 2.2.1 Core UI Parity Invariant
To preserve spatial muscle memory and visual ergonomics on mobile screens, the Global View MUST maintain the exact physical button positions and DOM structures as individual provider views:
- **Top Control Bar:**
  1. `Refresh` (`#refresh-btn`): Refreshes all providers with configured credentials.
  2. `Estimate Refusal Rates` (`#refresh-refusal-btn`): Runs refusal estimation across the cross-provider pool.
  3. `Export Data` (`#export-btn`): Downloads consolidated multi-provider export JSON.
- **Bottom Action Bar:**
  1. `Desktop View` (`#desktop-toggle-fab`): Toggles desktop viewport scaling.
  2. `Filter` (`#filter-btn`): Filters pooled global models via `filterState_global`.
  3. `Columns` (`#columns-btn`): Adjusts visible columns globally via `columnState_global`.

#### 2.2.2 Global Multi-Provider Model Aggregation & Provenance
- When `appState.activeProvider === 'all'`:
  - Iterate through all implemented providers in `PROVIDER_REGISTRY`.
  - Ingest models exclusively from `cached_richModels_<providerId>` (never legacy un-suffixed keys).
  - Attach explicit provenance to each model instance:
    ```javascript
    const modelWithProvenance = {
        ...model,
        _providerId: providerId,
        _providerName: PROVIDER_REGISTRY[providerId].name
    };
    ```
  - Pool models into `appState.parsedModels`.
  - Apply active filters using `filterState_global` to yield `appState.displayModels`.
  - Rank dynamic columns via `_columns.js`.

#### 2.2.3 Cell Rendering & Provider Badges
- In table cells, display a provider badge alongside or beneath the model name:
  ```html
  <span class="model-name">${model.name}</span>
  <span class="provider-pill provider-${model._providerId}">${model._providerName}</span>
  ```
- This gives immediate visual feedback on which provider hosts each top-ranked model.

#### 2.2.4 Collision Prevention: Composite Model Identity
- **The Collision Risk:** Multiple providers offer models with identical IDs (e.g. `meta-llama/llama-3.3-70b-instruct`).
- **Composite Key Mandate:**
  - For model expansion and row binding, identity is strictly defined as `${model._providerId}:${model.id}`.
  - In `appState.expanded`: `{ compositeKey: `${providerId}:${modelId}`, colKey: 'context_length' }`.
  - In DOM buttons: `<button class="extend-btn" data-model-key="${model._providerId}:${model.id}" data-col="${colKey}">`.
  - Completely prevents cross-provider ID collisions from expanding the wrong row.

#### 2.2.5 Header UX Adaptation in Global View
- `#active-provider-badge`: Displays `"All Providers (Global View)"`.
- `#api-key`: Becomes read-only with value `""` and placeholder `"Keys configured per provider in side drawer"`.
- `#api-key-link`: Text changes to `"Open side drawer (☰) to configure individual provider keys"`, opening the side panel on tap.
- `#model-count-indicator`: Displays `"Showing ${N} of ${M} models across ${P} providers"`.

#### 2.2.6 Resilient Global Refresh Lifecycle
- When `Refresh` is clicked in Global View:
  1. Identify all providers where `implemented === true` and either `requiresKey === false` OR an API key exists in storage.
  2. If zero providers are configured, display: `"No providers configured. Please add an API key in the side panel."`
  3. Execute provider pipeline calls concurrently or sequentially using `Promise.allSettled()`.
  4. Isolate errors: if one provider fails (CORS proxy offline or invalid key), capture the failure, report in `#status`, and continue rendering all successful providers.
  5. Pool all successful results, update `cached_richModels_<providerId>`, re-filter, and re-render.

#### 2.2.7 Cross-Tab Storage Synchronization
- Implement window storage event listener:
  ```javascript
  window.addEventListener('storage', (event) => {
      if (event.key.startsWith('filterState_') || 
          event.key.startsWith('columnState_') || 
          event.key === 'active_provider') {
          updateProviderUI();
      }
  });
  ```
- Guarantees seamless synchronization across multiple browser tabs and installed Capacitor PWA windows without reloads.

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **DO NOT mutate single-provider storage caches when running in global view.** Never overwrite `cached_richModels_<providerId>` with aggregated global arrays.
2. **DO NOT fire unmetered endpoint loops.** Global refresh only fetches providers with valid keys or anonymous endpoints.
3. **Preserve Core UI Parity Invariant:** Never move, hide, or re-order the 5 core control buttons in Global View.
4. **Use Composite IDs:** Always use `<providerId>:<modelId>` for event delegation and model expansion.
5. **Precache & Cache Busting:**
   - Bump `index.html` import to `./core.js?v=0K`.
   - Bump `sw.js` `CACHE_NAME` to `matrix-cache-v13`.
   - Run `npm run build:web` to synchronize Capacitor assets.
6. **Post-Milestone Handover:** Update `codebase_1.md` with Global View architecture, composite model key specification, and updated git state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Syntax check all modified modules
node --check adapters/_pipeline.js
node --check adapters/_registry.js
node --check core.js

# 2. Build sync to Capacitor www directory
npm run build:web
```

#### User Mobile Verification (`http://localhost:8080`):
1. **Navigation Test:** Open side panel (☰). Tap `All Providers (Home)`. Verify table renders models from all cached providers with provider pill badges.
2. **UI Parity Test:** Verify top control bar and bottom action bar contain all buttons in the exact same positions as single-provider pages.
3. **Collision Test:** In Global View, find models from different providers (e.g. Groq vs OpenRouter). Tap `Extend` on one. Verify ONLY that specific provider's model row expands.
4. **Global Filter Test:** Tap `Filter`, select `Verified Free Only ($0)`. Verify counter updates to `"Showing X of Y models across Z providers"` and only zero-cost models remain.
5. **Cross-Tab Sync Test:** Open two browser tabs on the phone. Change filter in Tab 1; switch to Tab 2 and verify state updates automatically.


---

## 2.3 MILESTONE 0C-6G: ADVANCED CAPABILITY & MODALITY FILTERS (+ GROUP A METADATA DEBT FIXES)

### 1. Objective & Scope
- **Objective:** Extend the declarative filter popover with tri-state capability controls (`has_tools`, `has_files`) and input modality toggles (`text`, `image`, `audio`) with zero HTML churn in `.table-actions-bar`, while simultaneously resolving Section 3 Group A provider adapter metadata debt across all 9 adapters.
- **Target Files to Create / Modify:**
  - `adapters/_filter.js` (MODIFY): Extend `FILTER_DEFINITIONS` and `DEFAULT_FILTER_STATE` to declaratively define `has_tools`, `has_files`, and `raw_modalities` filters.
  - Group A Provider Adapters (MODIFY):
    - `adapters/gemini/index.js`: Fix `has_tools: 1` detection for Gemini 1.5 Pro / Flash.
    - `adapters/sambanova/index.js`: Fix dynamic `raw_modalities: "text,image"` for multimodal Llama 3.2 Vision models and dynamic `is_chat`.
    - `adapters/openrouter/index.js`: Dynamically derive `is_chat` from architecture/modalities rather than hardcoding `true`.
    - `adapters/groq/index.js`: Capture structured output and reasoning metadata.
    - `adapters/mistral/index.js`: Expand capabilities dictionary parsing.
  - `core.js` (MODIFY): Re-export updated filter definitions.
  - `index.html` (PRESERVE): Zero HTML structural changes required; filter popover dynamically generates UI from `FILTER_DEFINITIONS`.
  - `sw.js` (MODIFY): Bump cache to `matrix-cache-v14`.
  - `sync-www.js` (EXECUTE): Run `npm run build:web`.

---

### 2. Architecture & Integration Details

#### 2.3.1 Declarative Filter Extension (`adapters/_filter.js`)
Extend `FILTER_DEFINITIONS` to include capability and modality sections without altering popover DOM scaffolding:

```javascript
export const DEFAULT_FILTER_STATE = {
    free: 'free_eligible',       // 'all' | 'free_eligible' | 'strict_free' | 'paid_only'
    is_chat: 'chat_only',         // 'all' | 'chat_only' | 'non_chat'
    has_tools: 'any',             // 'any' | 'require' | 'exclude'
    has_files: 'any',             // 'any' | 'require' | 'exclude'
    raw_modalities: 'all'         // 'all' | 'text' | 'image' | 'audio'
};

export const FILTER_DEFINITIONS = [
    // Existing free and is_chat groups...
    {
        id: 'has_tools',
        label: 'Function / Tool Calling',
        type: 'radio',
        options: [
            { value: 'any',     label: 'Any Tool Support (Default)', predicate: () => true },
            { value: 'require', label: 'Tools Required (has_tools)', predicate: m => m.has_tools === 1 },
            { value: 'exclude', label: 'No Tools (Text Only)',      predicate: m => m.has_tools === 0 }
        ]
    },
    {
        id: 'has_files',
        label: 'Vision & File Ingestion',
        type: 'radio',
        options: [
            { value: 'any',     label: 'Any File Support (Default)', predicate: () => true },
            { value: 'require', label: 'Vision / Files Required',    predicate: m => m.has_files === 1 },
            { value: 'exclude', label: 'No Vision / Files',          predicate: m => m.has_files === 0 }
        ]
    },
    {
        id: 'raw_modalities',
        label: 'Input Modalities',
        type: 'radio',
        options: [
            { value: 'all',   label: 'All Modalities (Default)',   predicate: () => true },
            { value: 'image', label: 'Multimodal Vision (Images)', predicate: m => (m.raw_modalities || '').includes('image') },
            { value: 'audio', label: 'Audio Ingestion (Speech)',   predicate: m => (m.raw_modalities || '').includes('audio') }
        ]
    }
];
```

#### 2.3.2 Resolution of Group A Provider Adapter Technical Debt
To ensure filters return accurate results across all 9 providers, the following adapter fixes are baked into this milestone:
1. **Google Gemini (`adapters/gemini/index.js`):**
   - Gemini models natively support function calling via `generateContent`.
   - Update normalization: if model ID includes `gemini-1.5` or `gemini-2.0`, set `has_tools = 1` (instead of `null`).
   - For multimodal vision (Gemini 1.5 Pro, Flash), ensure `has_files = 1` and `raw_modalities = "text,image,audio"`.
2. **SambaNova (`adapters/sambanova/index.js`):**
   - Multimodal models (`Llama-3.2-11B-Vision`, `Llama-3.2-90B-Vision`) must set `has_files = 1` and `raw_modalities = "text,image"`.
   - Dynamic `is_chat`: Verify model ID does not contain `guard` or non-instruct identifiers.
3. **OpenRouter (`adapters/openrouter/index.js`):**
   - Parse `model.architecture?.modality` and `model.architecture?.instruct_type`.
   - Set `is_chat = false` for embedding (`text->embedding`) or base completion models.
4. **Groq (`adapters/groq/index.js`):**
   - Retain `has_tools = supported_features.includes('tools') ? 1 : 0`.
   - Capture structured outputs (`json_mode`) and reasoning tokens (`deepseek-r1-distill`) in normalized model properties.
5. **Mistral AI (`adapters/mistral/index.js`):**
   - Inspect `model.capabilities`: set `has_tools = 1` if `capabilities.function_calling === true`, and `has_files = 1` if `capabilities.vision === true` (e.g., Pixtral).

#### 2.3.3 Dynamic Filter Popover Synchronization & Reset
- Popover DOM generator (`buildFilterPopoverDOM()`) iterates over all 5 `FILTER_DEFINITIONS` groups dynamically.
- `handleFilterReset()` atomically restores all 5 filter keys to `DEFAULT_FILTER_STATE`, hides `#filter-active-dot`, updates storage (`filterState_<providerId>` or `filterState_global`), and re-renders table.

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **Zero HTML Churn:** Do not alter the static HTML structure of `.table-actions-bar` or `#filter-popover`. All controls must render dynamically from `FILTER_DEFINITIONS`.
2. **Schema Invariant:** Do not introduce unapproved fields into `createNormalizedModel()`. Use approved nullable properties.
3. **Preserve Default Behaviors:** Default filter settings MUST retain default view (`free_eligible`, `chat_only`, `any` for capabilities).
4. **Precache & Cache Busting:**
   - Update `index.html` import to `./core.js?v=0L`.
   - Update `sw.js` `CACHE_NAME` to `matrix-cache-v14`.
   - Run `npm run build:web` to mirror files into `www/`.
5. **Post-Milestone Handover:** Update `codebase_1.md` with resolved technical debt and updated git state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Syntax check all modified adapters and filter engine
node --check adapters/_filter.js
node --check adapters/gemini/index.js
node --check adapters/sambanova/index.js
node --check adapters/openrouter/index.js
node --check adapters/groq/index.js
node --check adapters/mistral/index.js
node --check core.js

# 2. Build sync to Capacitor www directory
npm run build:web
```

#### User Mobile Verification (`http://localhost:8080`):
1. **Gemini Capability Test:** Switch to Gemini. Tap `Filter`. Select `Tools Required`. Verify Gemini 1.5 Pro and Flash remain visible. Select `Vision / Files Required`. Verify multimodal Gemini models remain visible.
2. **SambaNova Vision Test:** Switch to SambaNova. Select `Vision / Files Required`. Verify Llama-3.2-11B-Vision remains visible while text-only models are filtered out.
3. **Empty State & Reset Test:** Select conflicting filters (e.g. `Vision / Files Required` on a text-only provider). Verify empty state card displays with dynamic colspan. Tap `Reset to Default`. Verify all models restore cleanly.

---

## 2.4 MILESTONE 0C-2: MULTI-SOURCE BENCHMARK ENRICHMENT

### 1. Objective & Scope
- **Objective:** Eliminate `null` benchmark scores (`-`) across non-OpenRouter models (Groq, Gemini, SambaNova, Mistral, Cohere, etc.) by ingesting and blending metrics from six authoritative public benchmark sources, paired with a canonical cross-provider model slug normalizer.
- **Target Files to Create / Modify:**
  - `adapters/_slug.js` (NEW): Canonical cross-provider model slug normalizer mapping vendor-specific model identifiers to unified canonical family keys.
  - `benchmarks/benchmarks_data.json` (NEW): Bundled offline JSON dataset containing normalized benchmark scores from all 6 sources.
  - `adapters/_pipeline.js` (MODIFY): Hydrate normalized model objects with benchmark scores during pipeline execution.
  - `index.html` (MODIFY): Hydrate cached models on load/provider switch so existing stored models receive benchmark scores without requiring forced re-fetch.
  - `sw.js` (MODIFY): Bump cache to `matrix-cache-v15`, precache `./adapters/_slug.js` and `./benchmarks/benchmarks_data.json`.
  - `sync-www.js` (MODIFY): Add copy rule for `benchmarks/` directory to `www/benchmarks/`.

---

### 2. Architecture & Integration Details

#### 2.4.1 Canonical Slug Normalizer (`adapters/_slug.js`)
Model IDs across providers use conflicting naming patterns:
- Groq: `llama-3.3-70b-versatile`
- SambaNova: `meta-llama/Llama-3.3-70B-Instruct`
- OpenRouter: `meta-llama/llama-3.3-70b-instruct:free`
- Cohere: `command-r-08-2024`
- Gemini: `models/gemini-1.5-flash-latest`

`adapters/_slug.js` normalizes these into canonical slugs:

```javascript
// adapters/_slug.js
export function normalizeModelSlug(rawId) {
    if (!rawId || typeof rawId !== 'string') return '';
    let s = rawId.toLowerCase().trim();

    // 1. Strip vendor prefixes
    s = s.replace(/^(models\/|meta-llama\/|google\/|qwen\/|mistralai\/|cohere\/|nvidia\/|deepseek-ai\/)/, '');

    // 2. Strip tags and suffixes
    s = s.replace(/:free$/, '');
    s = s.replace(/-versatile$/, '');
    s = s.replace(/-instruct$/, '');
    s = s.replace(/-chat$/, '');
    s = s.replace(/-latest$/, '');
    s = s.replace(/@preview$/, '');

    // 3. Normalize delimiter variants
    s = s.replace(/_/g, '-');

    return s;
}
```

#### 2.4.2 Benchmark Sources & Disposition of Legacy `model_stats.json`
- Ingested evaluation sources:
  1. **Artificial Analysis:** Quality Index, Coding Index, Agentic Index.
  2. **LiveBench:** Hard evaluation suite covering Reasoning, Coding, Math, Data Analysis, and Instruction Following.
  3. **HuggingFace Open LLM Leaderboard:** MMLU-Pro, IFEval, MuSR, MATH, GPQA, GSM8k.
  4. **BenchLM:** Free-tier latency and capability benchmarks.
  5. **BenchGecko:** Free-tier comparative evaluations.
  6. **LMArena:** Crowdsourced Elo ratings.
- **Legacy Disposition:** Any useful records from legacy `model_stats.json` are consolidated into `benchmarks/benchmarks_data.json`. The application standardizes on `benchmarks/benchmarks_data.json` as the single canonical offline benchmark snapshot.

#### 2.4.3 Hydration Pipeline Integration
1. In `adapters/_pipeline.js` (`runProviderPipeline`):
   - After `adapter.normalize(rawData)` creates `NormalizedModel` instances, invoke benchmark enrichment:
     ```javascript
     normalizedModels.forEach(model => {
         const slug = normalizeModelSlug(model.id);
         const bench = BENCHMARK_MAP[slug];
         if (bench) {
             if (model.intelligence_index === null && bench.intelligence_index !== undefined) {
                 model.intelligence_index = bench.intelligence_index;
             }
             if (model.coding_index === null && bench.coding_index !== undefined) {
                 model.coding_index = bench.coding_index;
             }
             if (model.agentic_index === null && bench.agentic_index !== undefined) {
                 model.agentic_index = bench.agentic_index;
             }
         }
     });
     ```
2. In `index.html` on startup / provider switch:
   - Hydrate cached models stored in `cached_richModels_<providerId>` using the bundled dataset so users do not need to burn API quotas to see benchmark scores.

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **DO NOT invent fake metrics (Safeguard #4):** If a model does not match any benchmark in the dataset, its score MUST remain `null` so the UI renders `-`.
2. **DO NOT fire network calls for benchmarks on mobile reload.** Use the bundled, precached snapshot in `benchmarks/benchmarks_data.json`.
3. **Register Assets in Build:** Both `sw.js` and `sync-www.js` MUST include `benchmarks/benchmarks_data.json`.
4. **Precache & Cache Busting:**
   - Update `index.html` import to `./core.js?v=0M`.
   - Update `sw.js` `CACHE_NAME` to `matrix-cache-v15`.
   - Run `npm run build:web`.
5. **Post-Milestone Handover:** Update `codebase_1.md` with `adapters/_slug.js` specification, benchmark schema, and updated git state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Syntax check slug normalizer
node --check adapters/_slug.js
node --check adapters/_pipeline.js
node --check core.js

# 2. Verify JSON integrity
node -e "JSON.parse(fs.readFileSync('benchmarks/benchmarks_data.json'))"

# 3. Build sync to Capacitor www directory
npm run build:web
```

#### User Mobile Verification (`http://localhost:8080`):
1. **Groq Benchmark Test:** Switch to Groq in the side drawer. Verify `Llama-3.3-70b-versatile` now displays non-null Thinking, Coding, and Agentic scores in columns 1, 2, and 3.
2. **SambaNova Benchmark Test:** Switch to SambaNova. Verify `Meta-Llama-3.3-70B-Instruct` displays benchmark scores matching the canonical Llama 3.3 70B family.
3. **Sorting Hierarchy Test:** Tap the `Coding` column header. Verify models sort in descending order based on the enriched benchmark scores.

---

## 2.5 MILESTONE 0C-7: CROSS-PROVIDER REFUSAL RATES

### 1. Objective & Scope
- **Objective:** Extend refusal rate estimation across all non-OpenRouter providers and Global View by reusing canonical model slug normalization, authenticating via OpenRouter credentials when available or falling back to a bundled baseline dataset (`refusal_rates.json`).
- **Target Files to Create / Modify:**
  - `refusal_rates.json` (NEW / STANDARDIZE): Bundled baseline dataset containing canonical slug refusal rates.
  - `core.js` (MODIFY): Update `refreshRefusalRates()` to accept cross-provider model arrays, resolve canonical slugs, authenticate via `api_key_openrouter` or fall back to bundled rates.
  - `index.html` (MODIFY): Enable `#refresh-refusal-btn` across all providers and Global View (removing the single-provider restriction), updating caches and re-ranking column 5.
  - `sw.js` (MODIFY): Bump cache to `matrix-cache-v16`, precache `./refusal_rates.json`.
  - `sync-www.js` (EXECUTE): Ensure `refusal_rates.json` is synced to `www/refusal_rates.json`.

---

### 2. Architecture & Integration Details

#### 2.5.1 Cross-Provider Slug Normalization Reuse
- Reuses `normalizeModelSlug()` from `adapters/_slug.js`.
- When estimating refusal rates across non-OpenRouter models (e.g. SambaNova, Groq, Mistral), IDs are mapped to canonical family slugs before submission to the LLM.
- Deduplicates identical model families across providers so the LLM skeleton contains only unique slugs, conserving token usage.

#### 2.5.2 Authentication Resolution & Bundled Fallback
When the user taps `Estimate Refusal Rates` from a non-OpenRouter provider view or Global View:
1. **Key Resolution:** Check `browserStorageAdapter.getItem('api_key_openrouter')` or `browserStorageAdapter.getItem('openRouterApiKey')`.
2. **Live LLM Estimation Route (If OpenRouter Key Present):**
   - Submit skeleton JSON of canonical slugs to `openrouter/free` (`openai/v1/chat/completions`).
   - Parse returned refusal rates (0–100 scale).
   - Persist to `cached_refusalRates`.
3. **Bundled Baseline Fallback Route (If No OpenRouter Key Configured):**
   - Fetch `./refusal_rates.json`.
   - Hydrate matching canonical slugs.
   - Display informative status: `"Applied bundled baseline refusal rates (OpenRouter key not configured for live LLM estimation)."`

#### 2.5.3 Multi-Cache Hydration & Column 5 Re-Ranking
- Hydrates `refusal_rate` property on:
  - Active `appState.displayModels` and `appState.parsedModels`.
  - `cached_richModels_<providerId>` for all affected providers.
- **Column 5 Ascending Sentinel Rule:**
  - Re-ranks Column 5 using `sortModelsForColumn(models, 5)` or dynamic `_columns.js`.
  - Sentinel `+999999` pushes missing/null refusal rates to the bottom while sorting lowest refusal rates (0% = least censored / most compliant) at the top.

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **DO NOT lock refusal rates to OpenRouter UI.** Remove the `style.display = (p.id === 'openrouter') ? '' : 'none'` guard from `index.html`.
2. **Respect Column 5 Sorting Contract:** Refusal rate ranking must remain ascending (0% at top, nulls at bottom via `+999999`).
3. **Sync `refusal_rates.json`:** Both `sw.js` and `sync-www.js` must track `refusal_rates.json` (verify existing conditional copy in `sync-www.js`; add only if absent).
4. **Precache & Cache Busting:**
   - Update `index.html` import to `./core.js?v=0N`.
   - Update `sw.js` `CACHE_NAME` to `matrix-cache-v16`.
   - Run `npm run build:web`.
5. **Post-Milestone Handover:** Update `codebase_1.md` with cross-provider refusal estimation specification and updated git state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Syntax check core.js and sw.js
node --check core.js
node -e "JSON.parse(fs.readFileSync('refusal_rates.json'))"

# 2. Build sync to Capacitor www directory
npm run build:web
```

#### User Mobile Verification (`http://localhost:8080`):
1. **Non-OpenRouter UI Test:** Switch to Groq or SambaNova. Verify the `Refresh Refusal Rates` button is now visible.
2. **Refusal Ingestion Test:** Tap `Refresh Refusal Rates`. Verify status updates and Column 5 fills with percentages across models.
3. **Ascending Order Test:** Verify models with lowest refusal rates rank at the top of Column 5, with `-` values at the bottom.
4. **Global View Test:** Switch to `All Providers (Global)`. Tap `Refresh Refusal Rates`. Verify cross-provider models are enriched.


---

## 2.6 MILESTONE 0C-8: GROUP B PROVIDER ADAPTERS (CUSTOM APIS)

### 1. Objective & Scope
- **Objective:** Complete universal 13-provider catalog coverage by implementing the 4 remaining Group B provider adapters: Cloudflare Workers AI, Ollama (local/cloud), OVHcloud AI Endpoints, and IBM watsonx.ai, updating registry metadata and sidebar badges.
- **Target Files to Create / Modify:**
  - `adapters/cloudflare/index.js` (NEW): Adapter for Cloudflare Workers AI model search endpoint.
  - `adapters/ollama/index.js` (NEW): Adapter for local/remote Ollama instance (`/api/tags`).
  - `adapters/ovh/index.js` (NEW): Adapter for OVHcloud AI Endpoints.
  - `adapters/watsonx/index.js` (NEW): Adapter for IBM watsonx.ai foundation model specs.
  - `adapters/_registry.js` (MODIFY): Update Group B entries to `implemented: true`, register adapter modules, configure dynamic placeholder text for composite keys.
  - `proxy.py` (MODIFY): Allow local `127.0.0.1:11434` connection exemption for local Ollama instances while maintaining `https://` proxy guard for remote endpoints.
  - `index.html` (MODIFY): Remove "Coming Soon" badges in sidebar drawer for Group B providers; handle composite key inputs in header.
  - `sw.js` (MODIFY): Bump cache to `matrix-cache-v17`, precache all 4 new adapter files.
  - `sync-www.js` (EXECUTE): Run `npm run build:web`.

---

### 2. Architecture & Integration Details

#### 2.6.1 Endpoint, Authentication & Data Contracts

##### 1. Cloudflare Workers AI (`adapters/cloudflare/index.js`):
- **Endpoint:** `https://api.cloudflare.com/client/v4/accounts/{account_id}/ai/models/search`
- **Authentication:** Bearer token with composite credential format: `<account_id>:<api_token>`.
- **Parsing:** Split key on `:`:
  ```javascript
  const [accountId, apiToken] = (apiKey || '').split(':');
  ```
- **Normalization:** Ingest `result` array. Extract context window, task type (`Text Generation`, `Text-to-Image`), and map `is_chat: true` for chat/instruct models.

##### 2. Ollama (`adapters/ollama/index.js`):
- **Endpoint:** `http://127.0.0.1:11434/api/tags` (or custom host).
- **Authentication:** `requiresKey: false` (optional key for remote tunnels).
- **CORS & Proxy Architecture:**
  - Ollama natively handles CORS when started with `OLLAMA_ORIGINS="*"`.
  - In browser mode, fetch connects directly to `http://127.0.0.1:11434/api/tags` bypassing `proxy.py` (since `proxy.py` enforces `https://`), or `proxy.py` allows an explicit `http://127.0.0.1` origin relay.
- **Normalization:** Ingest `models` array (`name`, `details.parameter_size`, `details.family`), mark `free: true`, `is_chat: true`.

##### 3. OVHcloud AI Endpoints (`adapters/ovh/index.js`):
- **Endpoint:** `https://endpoints.ai.cloud.ovh.net/v1/models`
- **Authentication:** Optional token (`requiresKey: false`). Anonymous discovery permitted.
- **Routing:** Routed through `proxy.py` in browser environment.
- **Normalization:** OpenAI-compatible list format. Identify free/community models.

##### 4. IBM watsonx.ai (`adapters/watsonx/index.js`):
- **Endpoint:** `https://us-south.ml.cloud.ibm.com/ml/v1/foundation_model_specs?version=2024-05-01`
- **Authentication:** Composite format: `<project_id>:<api_key>`.
- **Token Exchange:** Ingest API key, perform IAM token exchange via `https://iam.cloud.ibm.com/identity/token` (through proxy) to retrieve temporary bearer token.
- **Normalization:** Ingest `resources` array, extracting `model_id`, `input_tier`, `max_sequence_length`, `task_ids`.

#### 2.6.2 Dynamic Header UX for Composite Credentials
- In `index.html` and `_registry.js`:
  - When Cloudflare is selected, `#api-key` placeholder updates to `"Format: <Account_ID>:<API_Token>"`.
  - When watsonx is selected, `#api-key` placeholder updates to `"Format: <Project_ID>:<API_Key>"`.
  - When Ollama or OVHcloud is selected, placeholder updates to `"Optional (Leave blank for default localhost / anonymous)"`.
- Zero new header input fields are introduced; the single existing `#api-key` field accommodates composite strings cleanly.

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **DO NOT hardcode Account IDs or API Tokens in repository code.**
2. **Handle Optional Keys Gracefully:** If `requiresKey: false` (Ollama/OVH), allow immediate fetching without prompting "Please enter API Key".
3. **Local Ollama Network Handling:** Do not force local `http://127.0.0.1:11434` requests through HTTPS-only proxy paths.
4. **Precache & Cache Busting:**
   - Update `index.html` import to `./core.js?v=0O`.
   - Update `sw.js` `CACHE_NAME` to `matrix-cache-v17`.
   - Register all 4 new adapter paths in `sw.js` `ASSETS_TO_CACHE`.
   - Run `npm run build:web`.
5. **Post-Milestone Handover:** Update `codebase_1.md` with complete 13-provider specifications, composite key formats, and updated git state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Syntax check all 4 new adapters and registry
node --check adapters/cloudflare/index.js
node --check adapters/ollama/index.js
node --check adapters/ovh/index.js
node --check adapters/watsonx/index.js
node --check adapters/_registry.js
node --check core.js

# 2. Build sync to Capacitor www directory
npm run build:web
```

#### User Mobile Verification (`http://localhost:8080`):
1. **Sidebar Badges Test:** Open side panel (☰). Verify all Group B items (Cloudflare, Ollama, OVHcloud, watsonx) are now active without "Coming Soon" tags.
2. **Ollama Fetch Test:** If local Ollama is active on the phone or PC, select Ollama and tap `Refresh`. Verify models populate.
3. **Cloudflare Composite Key Test:** Select Cloudflare, enter test composite string `<id>:<token>`. Verify input accepts the string and attempts connection.

---

## 2.7 MILESTONE 0C-9: TELEMETRY & RATE LIMIT INGESTION

### 1. Objective & Scope
- **Objective:** Ingest throughput, capacity, and latency metrics—Requests per Minute (RPM), Requests per Day (RPD), Tokens per Minute (TPM), and Time to First Token (TTFT)—using a hybrid architecture combining dynamic HTTP response header extraction and a curated static reference baseline (`rate_limits.json`).
- **Target Files to Create / Modify:**
  - `rate_limits.json` (NEW): Curated baseline dataset mapping `{ provider, model_id }` to documented free/developer tier limits (RPM, RPD, TPM) and baseline TTFT.
  - `proxy.py` (MODIFY): Add `Access-Control-Expose-Headers` for rate limit and telemetry headers.
  - `adapters/_normalize.js` (MODIFY): Add nullable `rpm`, `rpd`, `tpm`, `ttft` fields to `createNormalizedModel()`.
  - `adapters/_columns.js` (MODIFY): Add column definitions for `rpm`, `rpd`, `tpm`, and `ttft`.
  - `adapters/_pipeline.js` (MODIFY): Enrich normalized models with static baseline limits and dynamic telemetry overlays.
  - `sw.js` (MODIFY): Bump cache to `matrix-cache-v18`, precache `./rate_limits.json`.
  - `sync-www.js` (MODIFY): Add copy step for `rate_limits.json` to `www/rate_limits.json`.

---

### 2. Architecture & Integration Details

#### 2.7.1 Hybrid Telemetry Ingestion Architecture
As established in Section 4 research, `/models` catalog endpoints omit rate limits. The system uses a two-tier hybrid ingestion strategy:
1. **Tier A: Curated Static Baseline (`rate_limits.json`):**
   - Maintained offline snapshot mapping canonical slugs and provider IDs to free tier limits:
     ```json
     {
       "groq:llama-3.3-70b-versatile": { "rpm": 30, "rpd": 14400, "tpm": 6000, "ttft": 180 },
       "gemini:gemini-1.5-flash": { "rpm": 15, "rpd": 1500, "tpm": 1000000, "ttft": 240 },
       "sambanova:meta-llama-3.3-70b-instruct": { "rpm": 20, "rpd": 10000, "tpm": 5000, "ttft": 150 }
     }
     ```
   - Automatically hydrates models during pipeline normalization.
2. **Tier B: Dynamic Response Header Interception:**
   - Captured during live LLM calls (e.g. refusal rate estimation or test probes).
   - Ingests headers: `x-ratelimit-remaining-requests`, `x-ratelimit-limit-requests`, `x-ratelimit-limit-tokens`, `retry-after`.
   - Overwrites static baseline with real-time values when received.

#### 2.7.2 CORS Proxy Header Exposure (`proxy.py`)
Update `proxy.py` to allow browser JavaScript to read rate limit headers:
```python
def _send_cors_headers(self):
    self.send_header('Access-Control-Allow-Origin', '*')
    self.send_header('Access-Control-Allow-Headers', 'Authorization, Content-Type')
    self.send_header('Access-Control-Allow-Methods', 'GET, OPTIONS')
    self.send_header('Access-Control-Expose-Headers', 
                     'x-ratelimit-limit-requests, x-ratelimit-limit-tokens, '
                     'x-ratelimit-remaining-requests, x-ratelimit-remaining-tokens, '
                     'retry-after')
    self.send_header('Access-Control-Max-Age', '86400')
```

#### 2.7.3 Schema & Dynamic Column Extensions
1. In `adapters/_normalize.js`:
   - Extend `createNormalizedModel()` with nullable fields: `rpm = null`, `rpd = null`, `tpm = null`, `ttft = null`.
2. In `adapters/_columns.js`:
   - Add column definitions:
     - `rpm`: Label: `"RPM"`, shortLabel: `"RPM"`, sortDirection: `'desc'`, fallback: `-999999`, defaultVisible: `false`.
     - `rpd`: Label: `"RPD"`, shortLabel: `"RPD"`, sortDirection: `'desc'`, fallback: `-999999`, defaultVisible: `false`.
     - `tpm`: Label: `"TPM"`, shortLabel: `"TPM"`, sortDirection: `'desc'`, fallback: `-999999`, defaultVisible: `false`.
     - `ttft`: Label: `"TTFT Latency"`, shortLabel: `"TTFT"`, sortDirection: `'asc'`, fallback: `999999`, defaultVisible: `false`, formatter: `v => v !== null ? `${v}ms` : '-'`.

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **DO NOT spam inference endpoints:** Rate limits must NOT be queried by firing loops of completions calls across all models. Use `rate_limits.json` baseline.
2. **Missing data remains `null`:** If a model has no documented limit, field remains `null` and renders `-`.
3. **Register `rate_limits.json` in Build:** Track in both `sw.js` and `sync-www.js`.
4. **Precache & Cache Busting:**
   - Update `index.html` import to `./core.js?v=0P`.
   - Update `sw.js` `CACHE_NAME` to `matrix-cache-v18`.
   - Run `npm run build:web`.
5. **Post-Milestone Handover:** Update `codebase_1.md` with rate limit telemetry schemas, proxy headers, and updated git state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Syntax check schema and column modules
node --check adapters/_normalize.js
node --check adapters/_columns.js
node --check core.js

# 2. Verify rate_limits.json JSON syntax
node -e "JSON.parse(fs.readFileSync('rate_limits.json'))"

# 3. Build sync to Capacitor www directory
npm run build:web
```

#### User Mobile Verification (`http://localhost:8080`):
1. **Column Toggle Test:** Tap `Columns`. Enable `RPM`, `RPD`, and `TTFT Latency`. Verify columns appear in the table header.
2. **Rate Limit Display Test:** Check Groq or Gemini models. Verify RPM (e.g. 30 for Groq Llama 3.3 70B) and RPD values render correctly.
3. **Latency Sorting Test:** Tap the `TTFT Latency` column header. Verify lowest latency models rank at top, with missing values at bottom.

---

## 2.8 MILESTONE 0D-1: 2-LAYER NORMALIZATION ARCHITECTURE (HEAVY LIFT)

### 1. Objective & Scope
- **Objective:** Completely resolve schema rigidity by refactoring the ingestion pipeline into two distinct architectural layers: Layer 1 (Lossless Dynamic Ingestion) preserving unclipped vendor metadata and multi-source benchmark fields, and Layer 2 (Interactive Semantic Mapping) projecting raw attributes into dynamic matrix columns and filter dimensions, guarded by a cache migration engine.
- **Target Files to Create / Modify:**
  - `adapters/_layer1.js` (NEW): Lossless ingestion normalizer capturing unconstrained vendor payloads, benchmark leaderboards, and telemetry.
  - `adapters/_layer2.js` (NEW): Semantic ontology projection engine mapping Layer 1 attributes into `_columns.js` and `_filter.js`.
  - `adapters/_normalize.js` (MODIFY): Wrap Layer 1/2 while maintaining backward-compatible `createNormalizedModel` facade.
  - `adapters/_pipeline.js` (MODIFY): Direct raw payloads through Layer 1 ingestion and Layer 2 projection.
  - `index.html` (MODIFY): Implement `schema_version: 2` cache migration guard for `localStorage` caches.
  - `sw.js` (MODIFY): Bump cache to `matrix-cache-v19`, precache `./adapters/_layer1.js` and `./adapters/_layer2.js`.
  - `sync-www.js` (EXECUTE): Run `npm run build:web`.

---

### 2. Architecture & Integration Details

#### 2.8.1 Layer 1: Lossless Dynamic Ingestion (`adapters/_layer1.js`)
Instead of pruning vendor responses down to a fixed 15-field record, Layer 1 captures everything:

```javascript
// adapters/_layer1.js
export function ingestLosslessModel(providerId, rawModel, benchmarks = {}, rateLimits = {}) {
    return {
        // Universal Identifiers
        id: rawModel.id || rawModel.name,
        name: rawModel.name || rawModel.id,
        provider: providerId,
        schema_version: 2,
        ingested_at: Date.now(),

        // Preserved Raw Vendor Attributes
        raw_vendor: { ...rawModel },

        // Canonical Normalized Anchors
        context_length: extractContextLength(rawModel),
        max_completion_tokens: extractMaxOutput(rawModel),
        pricing: extractPricing(rawModel),
        capabilities: extractCapabilities(rawModel),

        // Multi-Source Benchmark Provenance
        benchmarks: { ...benchmarks },

        // Capacity & Telemetry Metrics
        telemetry: { ...rateLimits }
    };
}
```

#### 2.8.2 Layer 2: Interactive Semantic Mapping (`adapters/_layer2.js`)
Layer 2 dynamically projects Layer 1 structured attributes into matrix columns and filters:
- **Projection Maps:** Defines declarative mappings between Layer 1 JSON paths (e.g., `benchmarks.artificial_analysis.quality_index` or `telemetry.rpm`) and column definitions.
- **Pre-Configured Semantic Profiles:**
  - `Default Balanced`: Context, Thinking, Coding, Agentic, Max Output, Refusal.
  - `Coding & Architecture`: Coding Index, Context Length, TPM, Reasoning Support.
  - `Free Tier Production`: Strict Free, RPM, RPD, TTFT Latency, Refusal Rate.

#### 2.8.3 Cache Migration Guard (`schema_version: 2`)
To prevent app crashes or blank tables when users upgrade with existing `localStorage` data:
```javascript
function migrateCachedModels(rawCachedData) {
    if (!rawCachedData) return null;
    try {
        const parsed = JSON.parse(rawCachedData);
        if (!Array.isArray(parsed)) return null;

        // Detect Version 1 Schema (Missing schema_version or schema_version < 2)
        if (parsed.length > 0 && (!parsed[0].schema_version || parsed[0].schema_version < 2)) {
            console.info("Migrating legacy v1 model cache to Layer 1/2 v2 schema...");
            return parsed.map(v1Model => ({
                id: v1Model.id,
                name: v1Model.name,
                provider: appState.activeProvider,
                schema_version: 2,
                raw_vendor: { ...v1Model },
                context_length: v1Model.context_length,
                max_completion_tokens: v1Model.max_completion_tokens,
                intelligence_index: v1Model.intelligence_index,
                coding_index: v1Model.coding_index,
                agentic_index: v1Model.agentic_index,
                refusal_rate: v1Model.refusal_rate,
                uptime: v1Model.uptime,
                latency: v1Model.latency,
                free: v1Model.free,
                is_chat: v1Model.is_chat,
                benchmarks: {},
                telemetry: {}
            }));
        }
        return parsed;
    } catch (e) {
        console.warn("Corrupt cache detected during migration; invalidating.", e);
        return null;
    }
}
```

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **Never throw uncaught errors on legacy cache formats.** The `schema_version` guard must silently migrate or invalidate outdated caches.
2. **Preserve `NormalizedModel` Facade:** Any downstream script relying on `createNormalizedModel` must continue to receive backward-compatible objects.
3. **Precache & Cache Busting:**
   - Update `index.html` import to `./core.js?v=0Q`.
   - Update `sw.js` `CACHE_NAME` to `matrix-cache-v19`.
   - Register `./adapters/_layer1.js` and `./adapters/_layer2.js` in `sw.js` precache array.
   - Run `npm run build:web`.
4. **Post-Milestone Handover:** Update `codebase_1.md` with complete 2-layer normalization architecture, migration guard specifications, and updated git state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Syntax check layer modules
node --check adapters/_layer1.js
node --check adapters/_layer2.js
node --check adapters/_normalize.js
node --check core.js

# 2. Build sync to Capacitor www directory
npm run build:web
```

#### User Mobile Verification (`http://localhost:8080`):
1. **Cache Migration Test:** Reload browser with existing cached provider data. Verify dashboard loads smoothly without exceptions or blank tables.
2. **Lossless Inspection Test:** Tap `Extend` on any model. Verify raw vendor metadata and full benchmark attributes display in the expanded card.
3. **Semantic Profile Test:** Select a semantic profile (e.g. "Coding Focus"). Verify table columns re-project dynamically to display coding metrics.


---

## 2.9 MILESTONE 0D-2: MODEL ROUTING & RECOMMENDATION ENGINE

### 1. Objective & Scope
- **Objective:** Transform the passive model dashboard into an active, intelligent dispatch engine by implementing a client-side Pareto-optimal recommendation algorithm (`adapters/_router.js`), constraint evaluation interface, and one-click connection code snippet generator.
- **Target Files to Create / Modify:**
  - `adapters/_router.js` (NEW): Constraint evaluation, multi-criteria scoring, Pareto frontier calculator, and SDK connection snippet generator.
  - `core.js` (MODIFY): Re-export routing engine and snippet generation functions.
  - `index.html` (MODIFY): Add Model Router modal / drawer (`#router-modal`), interactive constraint sliders, recommendation cards, and one-click copy buttons, respecting Popover Mutual Exclusion.
  - `sw.js` (MODIFY): Bump cache to `matrix-cache-v20`, precache `./adapters/_router.js`.
  - `sync-www.js` (EXECUTE): Run `npm run build:web`.

---

### 2. Architecture & Integration Details

#### 2.9.1 Multi-Criteria Pareto Optimization Algorithm (`adapters/_router.js`)
The router evaluates user-defined workload parameters to discover non-dominated, optimal models across multi-dimensional criteria:
1. **Hard Constraint Filtering:**
   - Task category: `coding`, `reasoning`, `agentic`, `summarization`, `general_chat`.
   - Pricing constraint: `strict_free` ($0 verified) vs `free_eligible` vs `any`.
   - Minimum context window requirement (e.g. >= 32,768 or >= 131,072 tokens).
   - Minimum RPM capacity (e.g. >= 15 RPM).
   - Multimodal inputs: `vision_required` (enforces `has_files === 1`).
   - Function calling: `tools_required` (enforces `has_tools === 1`).
2. **Soft Criteria Scoring & Pareto Frontier:**
   - Normalizes scores across:
     - Target task index (Coding, Thinking, or Agentic benchmark).
     - Context window capacity.
     - Latency / TTFT (inverting so lower ms produces higher score).
     - Safety compliance (Refusal rate inverted so lower refusal scores higher).
   - Computes weighted composite score and determines top 3 Pareto-optimal models with human-readable rationales (e.g., *"Top Speed/Throughput Option"*, *"Highest Intelligence Benchmark"*, *"Maximum Context Window"*).

#### 2.9.2 One-Click SDK & API Snippet Generator
Provides ready-to-paste integration snippets in 3 formats:
- **Python (OpenAI / Provider Native SDK):**
  ```python
  from openai import OpenAI
  client = OpenAI(
      base_url="{provider_base_url}",
      api_key=os.environ.get("{PROVIDER_ENV_KEY}")
  )
  response = client.chat.completions.create(
      model="{selected_model_id}",
      messages=[{"role": "user", "content": "Hello!"}]
  )
  ```
- **JavaScript / Node.js (Fetch & SDK):**
  ```javascript
  import OpenAI from 'openai';
  const client = new OpenAI({
      baseURL: '{provider_base_url}',
      apiKey: process.env.{PROVIDER_ENV_KEY}
  });
  ```
- **cURL Command:**
  ```bash
  curl -X POST "{provider_base_url}/chat/completions" \
       -H "Authorization: Bearer ${PROVIDER_ENV_KEY}" \
       -H "Content-Type: application/json" \
       -d '{"model": "{selected_model_id}", "messages": [{"role": "user", "content": "Hello"}]}'
  ```

#### 2.9.3 UI Integration & Mutual Exclusion
- In `.table-actions-bar`, add `#router-btn` ("⚡ Recommend Model").
- **Popover Mutual Exclusion Invariant:**
  - Opening `#router-modal` immediately closes `#filter-popover` and `#columns-popover`.
  - Closing the modal restores focus cleanly.

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **Client-Side Only:** Router calculations must execute 100% in-browser without sending user constraints to remote servers.
2. **Key Security Directive:** Never embed actual API keys into generated code snippets. Always use placeholder environment variable syntax (`os.environ.get(...)`, `process.env....`).
3. **Preserve Core UI Parity:** Router button integration must not disrupt the physical order of bottom bar action buttons.
4. **Precache & Cache Busting:**
   - Update `index.html` import to `./core.js?v=0R`.
   - Update `sw.js` `CACHE_NAME` to `matrix-cache-v20`.
   - Precache `./adapters/_router.js`.
   - Run `npm run build:web`.
5. **Post-Milestone Handover:** Update `codebase_1.md` with routing engine algorithms, snippet generators, and updated git state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Syntax check router module
node --check adapters/_router.js
node --check core.js

# 2. Build sync to Capacitor www directory
npm run build:web
```

#### User Mobile Verification (`http://localhost:8080`):
1. **Router Modal Test:** Tap `⚡ Recommend Model`. Verify the recommendation interface opens and any open filter/column popovers close.
2. **Constraint Test:** Select `Coding Focus` + `Strict Free ($0)` + `Min 64k Context`. Tap `Find Models`. Verify top recommendations match all 3 criteria.
3. **Snippet Copy Test:** Tap `Copy Python Snippet`. Verify clipboard contains the formatted snippet with proper model ID and environment variable placeholder.

---

## 2.10 MILESTONE 0E-1: CLI PARITY & METADATA EXPORT MODERNIZATION

### 1. Objective & Scope
- **Objective:** Upgrade `cli.js` to full 13-provider pipeline parity with multi-provider switching, in-memory CLI filtering flags, and termux clipboard integration, while modernizing the web and native `Export Data` feature to emit rich, versioned metadata payloads.
- **Target Files to Create / Modify:**
  - `cli.js` (MODIFY): Rewrite command router to support 13 providers across all 4 subcommands (`keys`, `refresh`, `estimate`, `fetch`), CLI filter flags (`--free-only`, `--chat-only`, `--columns`), and robust `config.json` serialization.
  - `core.js` (MODIFY): Export modernized export payload builder `buildExportPayload()`.
  - `index.html` (MODIFY): Modernize `Export Data` click listener to invoke `buildExportPayload()` and handle native Capacitor sharing via `@capacitor/filesystem` and `@capacitor/share`.
  - `sw.js` (MODIFY): Bump cache to `matrix-cache-v21`.
  - `sync-www.js` (EXECUTE): Run `npm run build:web`.

---

### 2. Architecture & Integration Details

#### 2.10.1 Universal 13-Provider CLI Subcommands (`cli.js`)
Upgrade `cli.js` to support all configured providers:

```bash
# Save API Key for any provider
models keys <providerId> <apiKey>

# Refresh model catalog for a specific provider or all providers
models refresh [providerId|--all]

# Estimate refusal rates across canonical slugs
models estimate [providerId|--all]

# Copy ranked model matrix JSON to Termux clipboard with filters
models fetch [providerId|--all] [--free-only] [--chat-only] [--columns=ctx,intel,code]
```

- **Backward-Compatible Key Storage:**
  - `models keys openrouter <key>` saves to `api_key_openrouter` AND legacy `openRouterApiKey` in `config.json`.
- **Storage Serialization Robustness:**
  - Safely handles stringified JSON arrays vs raw objects in `config.json`, preventing double-serialization errors.

#### 2.10.2 Modernized Export Payload Schema (`buildExportPayload`)
Export payloads emitted by both the web `Export Data` button and `models fetch` CLI command conform to the modernized schema:

```json
{
  "metadata": {
    "exported_at": "2026-10-20T16:00:00.000Z",
    "provider": "groq",
    "schema_version": 2,
    "total_models": 24,
    "displayed_models": 18,
    "filter_state": {
      "free": "free_eligible",
      "is_chat": "chat_only",
      "has_tools": "any",
      "has_files": "any",
      "raw_modalities": "all"
    },
    "visible_columns": [
      "context_length",
      "intelligence_index",
      "coding_index",
      "agentic_index",
      "max_completion_tokens",
      "refusal_rate"
    ]
  },
  "columns": [
    {
      "column_id": "context_length",
      "label": "Context Window",
      "models": [ ... ]
    }
  ]
}
```

#### 2.10.3 Native Capacitor Android Sharing Integration
In `index.html`, detect native execution environment:
- If `window.Capacitor?.isNativePlatform?.()` is true:
  1. Write export file via `@capacitor/filesystem` into `DOCUMENTS` directory.
  2. Share file using `@capacitor/share`.
- If browser environment:
  1. Trigger instant download via `URL.createObjectURL(new Blob(...))`.

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **Preserve CLI Dependencies:** Do not add external npm dependencies for CLI argument parsing. Use native Node.js ESM `process.argv` parsing.
2. **Termux API Graceful Fallback:** If `termux-clipboard-set` is not installed or fails, print the JSON to `stdout` with an informative tip.
3. **Backward-Compatibility:** Maintain `models keys <key>` default to `openrouter` if provider argument is omitted.
4. **Precache & Cache Busting:**
   - Update `index.html` import to `./core.js?v=0S`.
   - Update `sw.js` `CACHE_NAME` to `matrix-cache-v21`.
   - Run `npm run build:web`.
5. **Post-Milestone Handover:** Update `codebase_1.md` with modernized CLI reference, export schemas, and updated git state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Syntax check CLI and core modules
node --check cli.js
node --check core.js

# 2. Test CLI help output
node cli.js

# 3. Build sync to Capacitor www directory
npm run build:web
```

#### User Mobile Verification:
1. **CLI Multi-Provider Test (Termux):** Run `node cli.js refresh groq`. Verify Groq catalog refreshes and saves to `config.json`.
2. **CLI Filter Test (Termux):** Run `node cli.js fetch groq --free-only`. Verify clipboard receives filtered Groq models.
3. **Web Export Test (`http://localhost:8080`):** Tap `Export Data`. Verify the downloaded JSON file contains the new `metadata` envelope with active filter states and timestamps.

---

## 2.11 MILESTONE 0E-2: PRODUCTION EDGE CORS PROXY DEPLOYMENT

### 1. Objective & Scope
- **Objective:** Deploy a lightweight, serverless edge CORS proxy (Cloudflare Worker) to resolve browser Mixed Content blocking on production HTTPS origins (GitHub Pages), implementing origin locking, header relays, and automated runtime proxy URL resolution.
- **Target Files to Create / Modify:**
  - `edge/worker.js` (NEW): Cloudflare Worker script handling CORS preflights, HTTPS forwarding, header relay, and origin validation.
  - `edge/wrangler.toml` (NEW): Wrangler configuration file for Cloudflare Worker deployment.
  - `adapters/` (MODIFY): Update `IS_BROWSER` proxy URL resolution to select local vs production proxy dynamically based on `window.location.origin`.
  - `core.js` (MODIFY): Export `resolveProxyUrl(targetUrl)`.
  - `sw.js` (MODIFY): Bump cache to `matrix-cache-v22`.
  - `sync-www.js` (EXECUTE): Run `npm run build:web`.

---

### 2. Architecture & Integration Details

#### 2.11.1 Cloudflare Worker Edge Proxy Script (`edge/worker.js`)
Solves the fundamental browser constraint where an HTTPS dashboard (e.g. `https://<username>.github.io`) cannot query `http://127.0.0.1:8081` due to Mixed Content security blocking:

```javascript
// edge/worker.js
export default {
    async fetch(request, env, ctx) {
        // Handle CORS Preflight
        if (request.method === "OPTIONS") {
            return new Response(null, {
                status: 204,
                headers: {
                    "Access-Control-Allow-Origin": "*",
                    "Access-Control-Allow-Methods": "GET, POST, OPTIONS",
                    "Access-Control-Allow-Headers": "Authorization, Content-Type",
                    "Access-Control-Expose-Headers": "x-ratelimit-remaining-requests, x-ratelimit-limit-requests, x-ratelimit-limit-tokens, retry-after",
                    "Access-Control-Max-Age": "86400"
                }
            });
        }

        const url = new URL(request.url);
        const targetUrl = url.searchParams.get("url");

        if (!targetUrl || !targetUrl.startsWith("https://")) {
            return new Response("Bad Request: 'url' parameter must start with https://", { status: 400 });
        }

        // Forward Request to Upstream
        const upstreamHeaders = new Headers();
        if (request.headers.has("Authorization")) {
            upstreamHeaders.set("Authorization", request.headers.get("Authorization"));
        }
        upstreamHeaders.set("User-Agent", "TopModels-EdgeProxy/1.0");

        try {
            const upstreamResponse = await fetch(targetUrl, {
                method: request.method,
                headers: upstreamHeaders,
                body: request.method === "POST" ? request.body : undefined
            });

            const responseHeaders = new Headers(upstreamResponse.headers);
            responseHeaders.set("Access-Control-Allow-Origin", "*");
            responseHeaders.set("Access-Control-Expose-Headers", "x-ratelimit-remaining-requests, x-ratelimit-limit-requests, x-ratelimit-limit-tokens, retry-after");

            return new Response(upstreamResponse.body, {
                status: upstreamResponse.status,
                headers: responseHeaders
            });
        } catch (e) {
            return new Response(`Bad Gateway: ${e.message}`, { status: 502 });
        }
    }
};
```

#### 2.11.2 Dynamic Runtime Proxy URL Resolution
In client modules, proxy routing resolves dynamically based on the execution host:

```javascript
export function resolveProxyUrl(targetUrl) {
    if (typeof window === 'undefined') {
        // Node CLI / Direct environment
        return targetUrl;
    }

    const host = window.location.hostname;
    const port = window.location.port;

    if (host === 'localhost' && port === '8080') {
        // Termux Local Development Server
        return `http://127.0.0.1:8081/proxy?url=${encodeURIComponent(targetUrl)}`;
    }

    if (window.Capacitor?.isNativePlatform?.()) {
        // Capacitor Native App: uses edge proxy or direct HTTPS
        return `https://top-models-proxy.<your-subdomain>.workers.dev/proxy?url=${encodeURIComponent(targetUrl)}`;
    }

    // GitHub Pages or other HTTPS Production Deployments
    return `https://top-models-proxy.<your-subdomain>.workers.dev/proxy?url=${encodeURIComponent(targetUrl)}`;
}
```

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **DO NOT break local Termux proxy:** Local dev environment on `localhost:8080` must continue routing to `127.0.0.1:8081`.
2. **Secure Edge Proxy:** The Edge Worker must strictly validate that `targetUrl` starts with `https://` to prevent SSRF vulnerabilities.
3. **Precache & Cache Busting:**
   - Update `index.html` import to `./core.js?v=0T`.
   - Update `sw.js` `CACHE_NAME` to `matrix-cache-v22`.
   - Run `npm run build:web`.
4. **Post-Milestone Handover:** Update `codebase_1.md` with edge proxy architecture, deployment configs, and updated git state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Syntax check edge worker and core modules
node --check edge/worker.js
node --check core.js

# 2. Build sync to Capacitor www directory
npm run build:web
```

#### User Mobile Verification:
1. **Local Proxy Integrity Test:** Run on `http://localhost:8080`. Refresh NVIDIA NIM or SambaNova. Verify local proxy handles request seamlessly.
2. **Edge Proxy Validation:** If Cloudflare Worker is deployed, test curl request:
   ```bash
   curl "https://<your-worker>.workers.dev/proxy?url=https://api.groq.com/openai/v1/models"
   ```
   Verify 200/401 upstream response with CORS headers.

---

## 2.12 MILESTONE 0E-3: PRODUCTION RELEASE (GITHUB PAGES & NATIVE APK)

### 1. Objective & Scope
- **Objective:** Finalize the production release `v1.0.0` of `Top_Models`: push clean git history to `origin/main`, deploy the PWA to GitHub Pages, build and package the native Capacitor Android APK, create the `v1.0.0` release tag, and publish complete user-facing documentation.
- **Target Files to Create / Modify:**
  - `package.json` (MODIFY): Bump version to `"1.0.0"`.
  - `index.html` (MODIFY): Bump module import to `./core.js?v=1.0.0`.
  - `sw.js` (MODIFY): Bump `CACHE_NAME` to `matrix-cache-v1.0.0`.
  - `README.md` (MODIFY): Document multi-provider BYOK setup, PWA installation, and CLI usage.
  - Capacitor Android project: Execute `npm run build:web && npx cap sync android && cd android && ./gradlew assembleRelease`.
  - Git repository: Execute final commit, tag `v1.0.0`, and push to `origin/main`.

---

### 2. Architecture & Integration Details

#### 2.12.1 Release Build Sequence
1. **Final Asset Synchronization:**
   - Run `npm run build:web` to ensure `www/` mirrors all 13 provider adapters, benchmarks, refusal rates, and rate limits.
2. **Capacitor Android Synchronization:**
   - Run `npx cap sync android` to copy `www/` into Android project assets.
3. **Android Release APK Compilation:**
   ```bash
   cd android && ./gradlew assembleRelease
   ```
   - Produces unsigned or keystore-signed release APK in `android/app/build/outputs/apk/release/`.
4. **GitHub Pages Deployment:**
   - Ensure repository settings have GitHub Pages enabled from branch `main` (root or `/docs`).
   - Clean git status verification before push.

#### 2.12.2 Production Version State
- `package.json`: `"version": "1.0.0"`
- `index.html`: `<script type="module" src="./core.js?v=1.0.0">`
- `sw.js`: `const CACHE_NAME = 'matrix-cache-v1.0.0';`

---

### 3. Execution Directives & Safeguards (Prompt Rules)
1. **Sole Authorized Remote Push:** This is the ONLY milestone where `git push origin main` and `git push --tags` are executed, strictly upon user command.
2. **Verify Clean Git Status:** Ensure zero untracked scratch files or uncommitted modifications exist before tagging.
3. **Offline Build Verification:** Verify the built PWA operates with full functionality while device is in Airplane Mode.
4. **Post-Milestone Requirement:** Perform final update to `~/storage/downloads/Sync/codebase_1.md` documenting `v1.0.0` production release state.

---

### 4. Two-Party Verification Protocol

#### Agent Automated Checks:
```bash
# 1. Verify build sync
npm run build:web

# 2. Capacitor Android sync check
npx cap sync android

# 3. Verify clean git working tree
git status --porcelain
```

#### User Mobile Verification:
1. **GitHub Pages Test:** Open `https://<username>.github.io/Top_Models/` on phone. Verify PWA installs cleanly, loads offline, and fetches via Edge Proxy.
2. **Native APK Test:** Install generated `app-release.apk` on realme 11 5G. Verify native file export, offline table caching, and UI responsiveness.
3. **Final Sign-Off:** Authorize git push to `origin/main` and tag `v1.0.0`.
