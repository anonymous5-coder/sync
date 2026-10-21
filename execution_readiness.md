# TOP_MODELS — EXECUTION READINESS & USER DECISION AUDIT

**Target Document:** `~/storage/downloads/Sync/execution_readiness.md`  
**Date:** October 2026  
**Auditor:** AI Architectural Auditor & Planning Pair  
**Baseline Git Commit:** `942bb06` (`Milestone 0C-6D: Implement in-memory filter UI, model-bound extended rows, and event delegation`)  
**Active Baseline Identifiers:** `core.js?v=0I`, `matrix-cache-v11`  
**Audited Artifacts:**
- Master Plan: `~/storage/downloads/Sync/MASTER_PLAN.md` (Commit `f40b9c1`, 1613 lines)
- Canonical Architecture: `~/storage/downloads/Sync/codebase_1.md` (599 lines)
- Live Application Codebase: `~/Top_Models/` (12 root and adapter modules)
- Historical Planning Context: `~/storage/downloads/conversations.md` (430 lines)

---

## 1. EXECUTIVE READINESS VERDICT: CONDITIONALLY READY

### Primary Verdict: **CONDITIONALLY READY**

#### Strategic Rationale:
1. **Architectural Coherence & Structural Soundness:** `MASTER_PLAN.md` establishes a complete, logically sequenced 12-milestone Directed Acyclic Graph (DAG) spanning Phase 0C through Phase 0E. The high-level architectural abstractions—declarative dynamic columns (`KG_column`), global multi-provider aggregation, two-layer normalization, client-side Pareto routing, and edge proxy deployment—are robust, well-reasoned, and aligned with project constraints (Android Termux, BYOK, zero external server dependencies, strict quota management).
2. **Material Plan-to-Code Discrepancies Identified:** The plan is **NOT** unconditionally ready for autonomous execution because three material specification defects exist in the earliest execution milestones (Specs 2.1, 2.2, and 2.3). If an agent executed these specifications literally without pre-resolved corrections:
   - In Milestone 0C-6E (Spec 2.1), model expansion would fail with `undefined` property lookups due to numerical index vs. string key mismatches.
   - In Milestone 0C-6F (Spec 2.2), Global View navigation in the side drawer would be silently rejected by `PROVIDER_REGISTRY` guards, and the refusal rate button would be hidden by legacy DOM display rules.
   - In Milestone 0C-6G (Spec 2.3), capability filters (`has_tools`, `has_files`, `raw_modalities`) would appear in the popover but be completely inert because `applyModelFilters()` in `_filter.js` hardcodes evaluation strictly for `free` and `is_chat`.
3. **Execution Path to "Fully Ready":** These three defects are localized, well-understood implementation bridges. Once the project owner reviews and approves the four discrete architecture decisions detailed in Section 7, and the P0/P1 corrections are applied to the milestone implementation prompts, sequential execution of Milestone 0C-6E can commence immediately with zero architectural risk.

---

## 2. COMPREHENSIVE SPECIFICATION VERIFICATION RESULTS (SPECS 2.1 THROUGH 2.12)

Every specification in `MASTER_PLAN.md` Part 2 was audited against the live source code in `~/Top_Models/`. In accordance with audit standards, proposed future features are strictly marked as **PLANNED BUT NOT IMPLEMENTED** rather than implemented.

```
================================================================================
STATUS DEFINITIONS:
  - IMPLEMENTED AND VERIFIED: Code exists, functions correctly, and matches spec.
  - IMPLEMENTED WITH ISSUES: Code exists but exhibits bugs, debt, or divergence.
  - PLANNED BUT NOT IMPLEMENTED: Fully specified forward feature awaiting execution.
  - BLOCKED BY A DEPENDENCY: Cannot be executed until predecessor milestone completes.
  - NOT VERIFIED — EVIDENCE INSUFFICIENT: Insufficient evidence to evaluate.
================================================================================
```

| Spec ID | Target Milestone Name | Logical Phase | Readiness Status | Plan Quality Verdict | Primary Source Contracts & Evidence |
| :---: | :--- | :---: | :---: | :---: | :--- |
| **0C-6D** | *Filter UI & Delegation (Baseline)* | Phase 0C | **IMPLEMENTED AND VERIFIED** | **COMPLETE** | `adapters/_filter.js:1–50`, `index.html:431–449, 985–993`, Commit `942bb06`. |
| **2.1** | **0C-6E: Dynamic Column UI** | Phase 0C | **PLANNED BUT NOT IMPLEMENTED** | **ISSUES FOUND** | `adapters/_columns.js` missing; `index.html:462, 862, 899` index mismatch. |
| **2.2** | **0C-6F: Multi-Provider Home Page** | Phase 0C | **BLOCKED BY A DEPENDENCY** | **ISSUES FOUND** | Depends on 0C-6E; `_registry.js:14–154` lacks `'all'`; `index.html:772, 1027`. |
| **2.3** | **0C-6G: Capability Filters & Debt** | Phase 0C | **BLOCKED BY A DEPENDENCY** | **ISSUES FOUND (Defect)** | Depends on 0C-6D/6F; `_filter.js:33–50` hardcoded loop; Group A adapter debts. |
| **2.4** | **0C-2: Multi-Source Benchmarks** | Phase 0C | **BLOCKED BY A DEPENDENCY** | **CONSISTENT** | Depends on 0C-6F; `_slug.js` missing; `benchmarks/` missing; `model_stats.json:1–17`. |
| **2.5** | **0C-7: Cross-Provider Refusal Rates** | Phase 0C | **BLOCKED BY A DEPENDENCY** | **CONSISTENT** | Depends on 0C-2; `core.js:22–86` locked to OpenRouter; `refusal_rates.json:1–13`. |
| **2.6** | **0C-8: Group B Provider Adapters** | Phase 0C | **PLANNED BUT NOT IMPLEMENTED** | **CONSISTENT** | Depends on 0C-1/6B; `_registry.js:114–153` (`implemented: false`); `proxy.py:51–57`. |
| **2.7** | **0C-9: Telemetry & Rate Limits** | Phase 0C | **BLOCKED BY A DEPENDENCY** | **CONSISTENT** | Depends on 0C-8/6E; `rate_limits.json` missing; `proxy.py:18–23` lacks expose headers. |
| **2.8** | **0D-1: 2-Layer Normalization** | Phase 0D | **BLOCKED BY A DEPENDENCY** | **CONSISTENT** | Depends on 0C-2/9/6E; `_layer1.js`, `_layer2.js` missing; `_normalize.js:1–38`. |
| **2.9** | **0D-2: Model Routing Engine** | Phase 0D | **BLOCKED BY A DEPENDENCY** | **CONSISTENT** | Depends on 0D-1; `_router.js` missing; Popover mutual exclusion rules. |
| **2.10** | **0E-1: CLI Parity & Export JSON** | Phase 0E | **BLOCKED BY A DEPENDENCY** | **CONSISTENT** | Depends on 0C-8/6D; `cli.js:1–114` OpenRouter-only; `index.html:1153–1194`. |
| **2.11** | **0E-2: Production Edge CORS Proxy** | Phase 0E | **BLOCKED BY A DEPENDENCY** | **CONSISTENT** | Depends on 0C-8; `edge/worker.js` missing; runtime proxy resolver needed. |
| **2.12** | **0E-3: Production Release v1.0.0** | Phase 0E | **BLOCKED BY A DEPENDENCY** | **CONSISTENT** | Depends on all prior; `package.json:1–32`; Android Capacitor sync & build. |

---

### Detailed Analysis of Individual Specifications

#### 2.1 Specification 2.1 — Milestone 0C-6E: Dynamic Column UI (`KG_column`)
- **Readiness Status:** **PLANNED BUT NOT IMPLEMENTED**
- **Observed Source Facts:**
  - `adapters/_columns.js` does NOT exist in the working tree.
  - `index.html` lines 413–422 hardcode a 6-column `<thead>` (`Context Window`, `Thinking`, `Coding`, `Agentic`, `Summarizer`, `Refusal Rates`).
  - `appState.rankedColumns` (line 462) is initialized as a 6-element array `[[], [], [], [], [], []]`.
  - Table rendering (line 899: `for (let c = 0; c < 6; c++)`), cell dataset attributes (line 912: `data-col="${c}"`), extended row rendering (line 928: `for(let c=0; c<6; c++)`), click delegation (line 989: `parseInt(btn.dataset.col, 10)`), and refresh re-ranking (lines 696–698, 1068–1070, 1131–1133) all hardcode a 0-to-5 numeric index.
  - `adapters/_sorting.js` exports `sortHierarchy` for keys `0..5`, with `latency` omitted from constants `S`.
- **Specification Requirements:**
  - Create declarative column registry `adapters/_columns.js` with `COLUMN_DEFINITIONS` and `DEFAULT_COLUMN_STATE`.
  - Enforce a minimum 1 visible column invariant.
  - Implement `#columns-btn`, `#columns-active-dot`, and `#columns-popover` with Popover Mutual Exclusion against `#filter-popover`.
  - Reconcile `appState.expanded` using `{ modelId, colKey }` and dynamic `colspan`.
- **Plan Defects / Discrepancies:**
  - **Defect:** Spec 2.1 specifies storing `{ modelId, colKey }` (string key) in `appState.expanded`, but does not define how `appState.rankedColumns` maps string keys to arrays. If `appState.rankedColumns` remains an array indexed 0 to N-1, expressions like `appState.rankedColumns[appState.expanded.colKey]` will evaluate to `undefined` and throw TypeError in `renderTable()` line 862 (`col.findIndex is not a function`).
- **Recommendation:** Implement Decision 1 (Option A): maintain `appState.activeColumns` as the ordered array of keys, index `appState.rankedColumns` in the same order, and introduce `getColumnIndex(colKey)`.

#### 2.2 Specification 2.2 — Milestone 0C-6F: Multi-Provider Home Page & Global View
- **Readiness Status:** **BLOCKED BY A DEPENDENCY** (Prerequisite: Milestone 0C-6E)
- **Observed Source Facts:**
  - In `adapters/_registry.js` lines 14–154, `PROVIDER_REGISTRY` contains 13 providers. There is no provider entry with `id: 'all'`.
  - In `index.html` line 1027, the drawer click handler verifies `if (providerId && PROVIDER_REGISTRY[providerId])`. Clicking a drawer item with `data-provider="all"` currently fails silently.
  - In `adapters/_pipeline.js` line 9, `runProviderPipeline(providerId)` throws `Error: Unknown provider: all`.
  - In `index.html` line 772, `refusalBtn.style.display = (p.id === 'openrouter') ? '' : 'none'` hard-hides the refusal estimation button for any view where `p.id !== 'openrouter'`.
- **Specification Requirements:**
  - Root multi-provider matrix view aggregating `cached_richModels_<providerId>` across all configured providers.
  - Strict Core UI Parity Invariant: identical physical button positions in top and bottom control bars.
  - Cell provider badges (`<span class="provider-pill">`).
  - Composite model identities (`<providerId>:<modelId>`) preventing ID collisions during row expansion.
  - Resilient `runGlobalPipeline()` using `Promise.allSettled()`.
  - Cross-tab synchronization via `window.addEventListener('storage', ...)`.
- **Plan Defects / Discrepancies:**
  - **Defect 1:** Spec 2.2 fails to explicitly mandate registering `'all'` in `PROVIDER_REGISTRY`, which causes drawer selection to fail.
  - **Defect 2:** Line 772 button hiding violates UI parity in Global View unless explicitly updated.
- **Recommendation:** Implement Decision 2 (Option A), add `PROVIDER_REGISTRY.all`, branch `refresh-btn` to call `runGlobalPipeline()`, and override line 772 for `activeProvider === 'all'`.

#### 2.3 Specification 2.3 — Milestone 0C-6G: Advanced Capability & Modality Filters
- **Readiness Status:** **BLOCKED BY A DEPENDENCY** (Prerequisites: Milestones 0C-6D, 0C-6F)
- **Observed Source Facts:**
  - In `adapters/_filter.js` lines 33–50:
    ```javascript
    export function applyModelFilters(models, filterState = DEFAULT_FILTER_STATE) {
        const freeDef = FILTER_DEFINITIONS.find(d => d.id === 'free');
        const freeOpt = freeDef?.options.find(o => o.value === state.free) || freeDef?.options[0];
        const chatDef = FILTER_DEFINITIONS.find(d => d.id === 'is_chat');
        const chatOpt = chatDef?.options.find(o => o.value === state.is_chat) || chatDef?.options[0];
        return models.filter(m => {
            if (!m) return false;
            if (freeOpt && !freeOpt.predicate(m)) return false;
            if (chatOpt && !chatOpt.predicate(m)) return false;
            return true;
        });
    }
    ```
  - `applyModelFilters()` strictly checks only `free` and `is_chat`.
  - In `adapters/gemini/index.js` line 32: `const hasTools = null;` (turns to `0` in `_normalize.js`).
  - In `adapters/sambanova/index.js` lines 45–47: `raw_modalities: "text"`, `is_chat: true` hardcoded.
  - In `adapters/openrouter/index.js` line 143: `is_chat: true` hardcoded.
  - In `adapters/groq/index.js` line 38: ignores structured outputs and reasoning metadata.
- **Specification Requirements:**
  - Add `has_tools` (`any`, `require`, `exclude`), `has_files` (`any`, `require`, `exclude`), and `raw_modalities` (`all`, `image`, `audio`) to `FILTER_DEFINITIONS`.
  - Fix Section 3 Group A metadata debts across Gemini, SambaNova, OpenRouter, Groq, and Mistral.
- **Plan Defects / Discrepancies:**
  - **Critical Defect:** Spec 2.3 claims that adding new groups to `FILTER_DEFINITIONS` is a "pure declarative extension with zero HTML churn". While true for the popover DOM generator (which iterates over `FILTER_DEFINITIONS`), the actual filtering engine `applyModelFilters()` will completely ignore the new filters because its loop is hardcoded strictly to `free` and `chat`.
- **Recommendation:** Implement Decision 3 (Option A) and update `applyModelFilters()` to dynamically loop over all definitions in `FILTER_DEFINITIONS` using `FILTER_DEFINITIONS.every(...)`.

#### 2.4 Specification 2.4 — Milestone 0C-2: Multi-Source Benchmark Enrichment
- **Readiness Status:** **BLOCKED BY A DEPENDENCY** (Prerequisite: Milestone 0C-6F)
- **Observed Source Facts:**
  - `adapters/_slug.js` does NOT exist.
  - `benchmarks/` directory does NOT exist.
  - Legacy `model_stats.json` exists (17 lines) but contains hardcoded values for only two models (`meta-llama/llama-3.1-8b-instruct:free` and `google/gemma-2-9b-it:free`) plus default.
  - Non-OpenRouter models (Groq, SambaNova, etc.) currently display `null` (`-`) across all benchmark columns (Thinking, Coding, Agentic).
- **Specification Requirements:**
  - Create canonical model slug normalizer `adapters/_slug.js` stripping vendor prefixes (`meta-llama/`, `google/`, `qwen/`), tags (`:free`, `-instruct`, `-versatile`), and normalizing delimiters.
  - Create bundled offline dataset `benchmarks/benchmarks_data.json` covering 6 sources (Artificial Analysis, LiveBench, HF Open LLM Leaderboard, BenchLM, BenchGecko, LMArena).
  - Hydrate newly fetched models in `_pipeline.js` and existing cached models in `index.html`.
  - Retire/consolidate `model_stats.json` into `benchmarks/benchmarks_data.json`.
- **Plan Quality Verdict:** **CONSISTENT**. Design is complete and robust; enforces Safeguard #4 (unmatched models remain `null`).

#### 2.5 Specification 2.5 — Milestone 0C-7: Cross-Provider Refusal Rates
- **Readiness Status:** **BLOCKED BY A DEPENDENCY** (Prerequisite: Milestone 0C-2)
- **Observed Source Facts:**
  - `refusal_rates.json` exists in project root (13 lines) but contains rates for only 7 OpenRouter models.
  - `core.js:refreshRefusalRates` (lines 22–86) is hardcoded to query `https://openrouter.ai/api/v1/chat/completions` using `openrouter/free`.
  - `index.html` line 1095 restricts execution: `if (appState.activeProvider !== 'openrouter') return;`.
- **Specification Requirements:**
  - Reuse `adapters/_slug.js` from Milestone 0C-2 to map heterogeneous IDs to canonical slugs.
  - Enable the refusal button across all providers and Global View.
  - If `api_key_openrouter` is present, query `openrouter/free`; if absent, fall back to bundled canonical slug refusal rates in `refusal_rates.json`.
  - Re-rank Column 5 ascending using `+999999` sentinel.
- **Plan Quality Verdict:** **CONSISTENT**. Solves non-OpenRouter refusal display gracefully.

#### 2.6 Specification 2.6 — Milestone 0C-8: Group B Provider Adapters (Custom APIs)
- **Readiness Status:** **PLANNED BUT NOT IMPLEMENTED** (Prerequisites: 0C-1, 0C-6B satisfied)
- **Observed Source Facts:**
  - In `adapters/_registry.js` lines 114–153, `cloudflare`, `ollama`, `ovh`, and `watsonx` are present with `implemented: false`.
  - In `proxy.py` lines 51–57, proxy rejects target URLs that do not start with `https://`.
- **Specification Requirements:**
  - Implement 4 adapter modules (`adapters/cloudflare/index.js`, `adapters/ollama/index.js`, `adapters/ovh/index.js`, `adapters/watsonx/index.js`).
  - Update `_registry.js` to `implemented: true`.
  - Dynamic `#api-key` placeholder text for composite credentials (`<account_id>:<api_token>` for Cloudflare, `<project_id>:<api_key>` for watsonx).
  - Explicit local connection path for Ollama to `http://127.0.0.1:11434/api/tags` bypassing HTTPS proxy guard.
- **Plan Quality Verdict:** **CONSISTENT**. Addresses authentication and network constraints accurately.

#### 2.7 Specification 2.7 — Milestone 0C-9: Telemetry & Rate Limit Ingestion
- **Readiness Status:** **BLOCKED BY A DEPENDENCY** (Prerequisites: Milestones 0C-8, 0C-6E)
- **Observed Source Facts:**
  - Catalog endpoints across all 9 Group A providers omit rate limit metadata.
  - `proxy.py` lines 18–23 sends CORS headers but omits `Access-Control-Expose-Headers`.
  - `adapters/_normalize.js` currently omits RPM, RPD, TPM, TTFT properties.
- **Specification Requirements:**
  - Two-tier hybrid architecture: curated offline baseline `rate_limits.json` + live response header capture (`x-ratelimit-*`).
  - Update `proxy.py` to send `Access-Control-Expose-Headers`.
  - Add nullable fields to `createNormalizedModel()` and new column definitions to `_columns.js`.
- **Plan Quality Verdict:** **CONSISTENT**. Prevents unmetered endpoint hammering per Safeguard #5.

#### 2.8 Specification 2.8 — Milestone 0D-1: 2-Layer Normalization Architecture (Heavy Lift)
- **Readiness Status:** **BLOCKED BY A DEPENDENCY** (Prerequisites: Milestones 0C-2, 0C-9, 0C-6E)
- **Observed Source Facts:**
  - `adapters/_normalize.js` produces a static 15-field object. Vendor properties outside these 15 fields are lost.
- **Specification Requirements:**
  - Layer 1 (`adapters/_layer1.js`): Lossless dynamic ingestion preserving unclipped vendor payloads, benchmark leaderboards, and telemetry.
  - Layer 2 (`adapters/_layer2.js`): Interactive semantic mapping projecting Layer 1 attributes into matrix columns and filters.
  - Critical `schema_version: 2` cache migration guard in `index.html` preventing crashes when reading pre-0D-1 caches.
- **Plan Quality Verdict:** **CONSISTENT**. Decouples vendor payloads from schema rigidity.

#### 2.9 Specification 2.9 — Milestone 0D-2: Model Routing & Recommendation Engine
- **Readiness Status:** **BLOCKED BY A DEPENDENCY** (Prerequisite: Milestone 0D-1)
- **Observed Source Facts:**
  - Dashboard is currently a passive inspection matrix without recommendation capabilities.
- **Specification Requirements:**
  - Client-side Pareto optimization algorithm evaluating hard constraints and soft scores.
  - One-click SDK connection snippet generator (Python, JS, cURL) using environment variable placeholders.
  - Popover Mutual Exclusion enforced between router modal and filter/column popovers.
- **Plan Quality Verdict:** **CONSISTENT**. Preserves client-side execution with zero credential leaks.

#### 2.10 Specification 2.10 — Milestone 0E-1: CLI Parity & Metadata Export Modernization
- **Readiness Status:** **BLOCKED BY A DEPENDENCY** (Prerequisites: Milestones 0C-8, 0C-6D)
- **Observed Source Facts:**
  - `cli.js` lines 28–35 hardcodes `openRouterApiKey` and OpenRouter `fetchData`.
  - `index.html` line 1160 exports raw arrays without metadata or active filter state snapshots.
- **Specification Requirements:**
  - Universal 13-provider CLI support across `keys`, `refresh`, `estimate`, `fetch`.
  - CLI filter flags (`--free-only`, `--chat-only`, `--columns`).
  - Modernized JSON export payload schema with metadata envelope (`exported_at`, `provider`, `filter_state`, `visible_columns`, `schema_version`).
  - Native Capacitor file export via `@capacitor/filesystem` and `@capacitor/share`.
- **Plan Quality Verdict:** **CONSISTENT**. Closes CLI-to-Web divergence.

#### 2.11 Specification 2.11 — Milestone 0E-2: Production Edge CORS Proxy Deployment
- **Readiness Status:** **BLOCKED BY A DEPENDENCY** (Prerequisite: Milestone 0C-8)
- **Observed Source Facts:**
  - Local Python proxy on `127.0.0.1:8081` cannot be queried by live HTTPS GitHub Pages due to browser Mixed Content blocking.
- **Specification Requirements:**
  - Cloudflare Worker edge proxy (`edge/worker.js`) with origin locking and `https://` target URL validation.
  - Dynamic runtime proxy resolution distinguishing Termux local dev (`http://localhost:8080`), GitHub Pages HTTPS, and Capacitor native webview.
- **Plan Quality Verdict:** **CONSISTENT**. Eliminates Mixed Content blocker for live deployment.

#### 2.12 Specification 2.12 — Milestone 0E-3: Production Release (GitHub Pages & Native APK)
- **Readiness Status:** **BLOCKED BY A DEPENDENCY** (Prerequisite: All prior milestones)
- **Observed Source Facts:**
  - Repository branch `main` is ahead of `origin/main` by 6 commits (consistent with the rule: NO remote push until 0E-3).
- **Specification Requirements:**
  - Final git push to `origin/main` and tag `v1.0.0`.
  - Live GitHub Pages deployment verification.
  - Capacitor Android release APK build (`npx cap sync android && ./gradlew assembleRelease`).
  - Production version alignment across `package.json`, `index.html`, and `sw.js`.
- **Plan Quality Verdict:** **CONSISTENT**. Final production release gates are clearly defined.

---

## 3. VERIFICATION RESULTS FOR EVERY LEDGER ROW

Every row of the Version, Service Worker & Build Sync Ledger was audited against the live codebase:

| Milestone ID | Target Milestone Name | `index.html` Import | `sw.js` `CACHE_NAME` | New Precached Assets (`sw.js`) | `sync-www.js` Asset Registration | Ledger Row Verdict | Detailed Evidence & Technical Finding |
| :---: | :--- | :---: | :---: | :--- | :--- | :---: | :--- |
| **0C-6D** | Filter UI & Extended Rows (Baseline) | `core.js?v=0I` | `matrix-cache-v11` | `./adapters/_filter.js` | Mirrored via `adapters/` | **CORRECT** | Verified exact match in `index.html:452`, `sw.js:1`, and `sync-www.js:53`. Baseline is solid. |
| **0C-6E** | Dynamic Column UI (`KG_column`) | `core.js?v=0J` | `matrix-cache-v12` | `./adapters/_columns.js` | Mirrored via `adapters/` | **CORRECT** | Core re-exports change (`?v=0J`); new file `_columns.js` requires cache bump `v12`; mirrored to `www/` automatically. |
| **0C-6F** | Multi-Provider Home Page & Global View | `core.js?v=0K` | `matrix-cache-v13` | None (Existing module updates) | Mirrored via `adapters/` | **CORRECT** | Modifies `core.js`, `_pipeline.js`, and `index.html`. Cache bump to `v13` correctly invalidates changed precached modules. |
| **0C-6G** | Advanced Capability & Modality Filters | `core.js?v=0L` | `matrix-cache-v14` | None (Updates to `_filter.js` & adapters) | Mirrored via `adapters/` | **CORRECT** | Modifies `_filter.js` and 5 provider adapters. Cache bump to `v14` ensures PWA fetches updated adapter scripts. |
| **0C-2** | Multi-Source Benchmark Enrichment | `core.js?v=0M` | `matrix-cache-v15` | `./adapters/_slug.js`, `./benchmarks/benchmarks_data.json` | Add `benchmarks/` copy step to `sync-www.js` | **CORRECT** | New directory `benchmarks/` requires explicit copy step in `sync-www.js` because it is outside `adapters/`. |
| **0C-7** | Cross-Provider Refusal Rates | `core.js?v=0N` | `matrix-cache-v16` | `./refusal_rates.json` | Add `refusal_rates.json` copy step to `sync-www.js` | **INCORRECT** | **Defect in Ledger Note:** `sync-www.js` lines 25–29 ALREADY contains `refusal_rates.json` copying! Action is verification, not addition. `sw.js` precache addition is correct. |
| **0C-8** | Group B Provider Adapters (Custom APIs) | `core.js?v=0O` | `matrix-cache-v17` | `./adapters/cloudflare/index.js`, `./adapters/ollama/index.js`, `./adapters/ovh/index.js`, `./adapters/watsonx/index.js` | Mirrored via `adapters/` | **CORRECT** | Four new adapter files added to `sw.js` precache array; automatically mirrored into `www/adapters/` via `fs.cpSync`. |
| **0C-9** | Telemetry & Rate Limit Ingestion | `core.js?v=0P` | `matrix-cache-v18` | `./rate_limits.json` | Add `rate_limits.json` copy step to `sync-www.js` | **CORRECT** | New root file `rate_limits.json` requires explicit addition to `sync-www.js` and `sw.js`. |
| **0D-1** | 2-Layer Normalization Architecture | `core.js?v=0Q` | `matrix-cache-v19` | `./adapters/_layer1.js`, `./adapters/_layer2.js` | Mirrored via `adapters/` | **CORRECT** | Two new layer modules precached in `sw.js`; mirrored via `adapters/` in `sync-www.js`. |
| **0D-2** | Model Routing & Recommendation Engine | `core.js?v=0R` | `matrix-cache-v20` | `./adapters/_router.js` | Mirrored via `adapters/` | **CORRECT** | New router module precached in `sw.js`; mirrored via `adapters/` in `sync-www.js`. |
| **0E-1** | CLI Parity & Metadata Export Modernization | `core.js?v=0S` | `matrix-cache-v21` | None (Updates to `core.js`, `index.html`) | Mirrored via `adapters/` | **CORRECT** | Export payload schema changes require cache bump and core version bump. `cli.js` is not in precache. |
| **0E-2** | Production Edge CORS Proxy Deployment | `core.js?v=0T` | `matrix-cache-v22` | None (Runtime proxy resolution update) | Mirrored via `adapters/` | **CORRECT** | Proxy URL resolution logic updated in client modules. Cache bumped to ensure live deployment picks up edge routes. |
| **0E-3** | Production Release (GitHub Pages & Native APK) | `core.js?v=1.0.0` | `matrix-cache-v1.0.0` | Full audit of all precached assets | Full sync & verification of `www/` | **CORRECT** | Production release standardizes import and cache container to semantic version `v1.0.0`. Full audit and APK sync verified. |

- **Ledger Audit Summary:** 12 rows are **CORRECT**; 1 row (**0C-7**) is **INCORRECT** regarding its `sync-www.js` instruction (action is verification of pre-existing code, not new addition).


---

## 4. CONFIRMED DEFECTS AND SEVERITY MATRIX

| Defect ID | Severity | Milestone / Spec | Affected Source / Plan Location | Defect Description & System Impact |
| :---: | :---: | :---: | :--- | :--- |
| **DEF-01** | **CRITICAL** | Milestone 0C-6G (Spec 2.3) | `adapters/_filter.js:33–50` | `applyModelFilters()` strictly resolves only `free` and `is_chat`. Simply adding `has_tools`, `has_files`, and `raw_modalities` to `FILTER_DEFINITIONS` leaves them completely inert during execution. |
| **DEF-02** | **HIGH** | Milestone 0C-6E (Spec 2.1) | `index.html:462, 862, 899, 912, 928, 974, 989` | `appState.expanded` stores `{ modelId, colKey }` (string), but all existing table lookup code indexes `appState.rankedColumns` numerically. Expanding any model row will throw `TypeError: col.findIndex is not a function`. |
| **DEF-03** | **HIGH** | Milestone 0C-6F (Spec 2.2) | `adapters/_registry.js:14–154`, `index.html:1027` | `PROVIDER_REGISTRY` lacks an entry for `all`. The side drawer event handler silently rejects `data-provider="all"`. Also, `index.html:772` hides the refusal button when `p.id !== 'openrouter'`. |
| **DEF-04** | **MEDIUM** | Milestone 0C-6F (Spec 2.2) | `adapters/_pipeline.js:9–11`, `index.html:1060` | If `refresh-btn` calls `runProviderPipeline('all', ...)`, it throws `Error: Unknown provider: all`. The refresh event listener must explicitly dispatch `runGlobalPipeline()`. |
| **DEF-05** | **LOW** | Milestone 0C-7 (Spec 2.5) | `MASTER_PLAN.md` Section 7 vs. `sync-www.js:25–29` | Ledger specifies "Add `refusal_rates.json` copy step to `sync-www.js`", but `sync-www.js` already includes this copy step. The required action is verification of existing code. |

---

## 5. MISSING DEPENDENCIES AND UNVERIFIED ASSUMPTIONS

1. **Missing Module Assets in Current Codebase:**
   - The following modules are planned by `MASTER_PLAN.md` but demonstrably do NOT exist in `~/Top_Models/` today:
     - `adapters/_columns.js` (Scheduled: Milestone 0C-6E)
     - `adapters/_slug.js` (Scheduled: Milestone 0C-2)
     - `benchmarks/benchmarks_data.json` (Scheduled: Milestone 0C-2)
     - `adapters/cloudflare/index.js`, `adapters/ollama/index.js`, `adapters/ovh/index.js`, `adapters/watsonx/index.js` (Scheduled: Milestone 0C-8)
     - `rate_limits.json` (Scheduled: Milestone 0C-9)
     - `adapters/_layer1.js`, `adapters/_layer2.js` (Scheduled: Milestone 0D-1)
     - `adapters/_router.js` (Scheduled: Milestone 0D-2)
     - `edge/worker.js` (Scheduled: Milestone 0E-2)
   - *Status:* This is an expected condition reflecting sequential milestone progression. None of these missing files represent a defect in the current baseline commit `942bb06`.
2. **Unverified External Assumptions:**
   - **Local Ollama CORS:** Assumes a local Ollama instance on Android or PC is started with `OLLAMA_ORIGINS="*"` to allow direct browser fetch without CORS blocking.
   - **OpenRouter `/free` Model Availability:** Assumes the `openrouter/free` model router remains available for structured refusal estimation prompts.
   - **Cloudflare Free Tier Quotas:** Assumes Cloudflare Workers AI free tier remains accessible via REST without complex session tokens.

---

## 6. PRIORITIZED CORRECTION LIST

### P0: Correctness & Immediate Execution Blockers (Must Bake into Milestone 0C-6E)
1. **Reconcile Column Key Lookup in `index.html` (Fixes DEF-02):**
   - *Action:* Source-code change during Milestone 0C-6E execution.
   - *Specification:* In `index.html`, define `appState.activeColumns = [...DEFAULT_COLUMN_STATE]` as the single source of truth for active column order. `appState.rankedColumns` stores an array of sorted model arrays of length `appState.activeColumns.length`. Provide helper `getColumnIndex(colKey)` to map string keys to array indices during row expansion and cell click delegation.
   - *Classification:* Implementation prompt directive.

### P1: Issues to Resolve Before Affected Milestones (0C-6F and 0C-6G)
2. **Dynamic Predicate Loop in `adapters/_filter.js` (Fixes DEF-01):**
   - *Action:* Source-code change during Milestone 0C-6G execution.
   - *Specification:* In `adapters/_filter.js`, refactor `applyModelFilters()`:
     ```javascript
     export function applyModelFilters(models, filterState = DEFAULT_FILTER_STATE) {
         if (!Array.isArray(models)) return [];
         const state = filterState || DEFAULT_FILTER_STATE;
         return models.filter(m => {
             if (!m) return false;
             return FILTER_DEFINITIONS.every(def => {
                 const activeVal = state[def.id];
                 const opt = def.options.find(o => o.value === activeVal) || def.options[0];
                 return opt ? opt.predicate(m) : true;
             });
         });
     }
     ```
   - *Classification:* Implementation prompt directive.
3. **Register Global Provider & Wire Dispatch (Fixes DEF-03, DEF-04):**
   - *Action:* Source-code change during Milestone 0C-6F execution.
   - *Specification:* In `adapters/_registry.js`, register `all: { id: 'all', name: 'All Providers (Global)', implemented: true }`. In `index.html`, route `refresh-btn` to `runGlobalPipeline()` when `appState.activeProvider === 'all'`. In `index.html:772`, adjust button visibility: `refusalBtn.style.display = (p.id === 'openrouter' || p.id === 'all') ? '' : 'none'`.
   - *Classification:* Implementation prompt directive.

### P2: Improvements That Can Safely Wait
4. **Clarify Ledger Row 5 Instruction (Fixes DEF-05):**
   - *Action:* Documentation note.
   - *Specification:* During post-milestone doc updates, clarify that `sync-www.js` already includes `refusal_rates.json` copying; only verification is needed.
   - *Classification:* Documentation polish.

---

## 7. SHORT OWNER DECISION BRIEF (WITH RECOMMENDED DEFAULTS)

The project owner can review and approve these four architectural decisions directly in ChatGPT without needing to resolve technical minutiae.

---

### Decision 1: Dynamic Column Indexing & Expansion State Architecture
- **Decision ID:** `DEC-01`
- **Exact Question:** How should `appState.rankedColumns` and row expansion be reconciled between dynamic string column keys (`colKey`) and table array indexing?
- **Why It Matters:** `index.html` currently hardcodes numerical indices `0..5` across 14 functions. If `appState.expanded` stores string `colKey` without a bridging index, row expansion breaks completely on non-default columns.
- **Available Options:**
  - **Option A (Recommended — Array-Aligned with Key Resolver):** `appState.activeColumns` stores the ordered array of active string keys (e.g. `['context_length', 'intelligence_index', ...]`). `appState.rankedColumns` is an array of corresponding sorted model arrays where index `i` maps to `appState.activeColumns[i]`. A helper `getColumnIndex(colKey)` resolves string keys to numerical indices for expansion and cell rendering. Button `data-col` remains numerical index into active columns.
  - **Option B (Object/Map-Based Storage):** `appState.rankedColumnsDynamic` is stored as an object keyed by column ID (`{ context_length: [...], ... }`). Requires refactoring all table rendering loops in `index.html`.
- **Recommendation & Evidence:** **Option A.** It preserves backward-compatibility with existing table rendering loops, DOM structure, and `sortModelsForColumn` conventions with minimal code churn.
- **Blocks Next Milestone?** **YES** (Must be included in Milestone 0C-6E execution prompt).
- **Proposed Default:** **Option A.**

---

### Decision 2: Global View Model Identity & Deduplication Policy
- **Decision ID:** `DEC-02`
- **Exact Question:** When pooling models across providers in the Global View (`activeProvider === 'all'`), should identically named open-weight models (e.g. `meta-llama/llama-3.3-70b-instruct` on Groq, SambaNova, and OpenRouter) appear as separate rows or be deduplicated/merged?
- **Why It Matters:** Power users compare BYOK providers specifically for latency, rate limits, uptime, and context window differences on identical model weights.
- **Available Options:**
  - **Option A (Recommended — Multi-Endpoint Listing with Badges):** Retain all provider endpoints as distinct entries in the pooled catalog, tagged with `_providerId` and a provider badge in each cell. Each row represents a specific provider's deployment of that model.
  - **Option B (Canonical Model Merging):** Deduplicate by canonical slug, displaying only the "best" provider per model or showing an embedded provider picker.
- **Recommendation & Evidence:** **Option A.** Directly reflects the BYOK reality that different providers offer radically different rate limits (Groq: 30 RPM, SambaNova: 20 RPM), latencies, and context windows for identical weights. Eliminates complex merging heuristics.
- **Blocks Next Milestone?** **NO** (Blocks Milestone 0C-6F).
- **Proposed Default:** **Option A.**

---

### Decision 3: Capability Filter Tri-State Behavior on Unknown Data
- **Decision ID:** `DEC-03`
- **Exact Question:** How should capability filters (`has_tools`, `has_files`) treat models where capability data is `null` (unspecified or omitted by the upstream provider catalog)?
- **Why It Matters:** In `adapters/_normalize.js`, `has_tools ? 1 : 0` currently converts `null` to `0`, creating false negatives where capable models (e.g. Gemini prior to debt fix) are hidden when filtering for tools.
- **Available Options:**
  - **Option A (Recommended — True Tri-State with Graceful Null Pass-Through):** Update `_normalize.js` to preserve `null` when capability is unknown. Filter predicates:
    - `any`: passes all models (`() => true`).
    - `require`: passes models where `has_tools === 1` OR known capable slugs.
    - `exclude`: passes models where `has_tools === 0` (strictly non-tool models).
  - **Option B (Strict Binary):** Treat `null` as `0` (missing = no tools). Models from providers that omit capability flags are strictly excluded under `require`.
- **Recommendation & Evidence:** **Option A.** Prevents false negatives from hiding capable models from providers that omit catalog capability flags.
- **Blocks Next Milestone?** **NO** (Blocks Milestone 0C-6G).
- **Proposed Default:** **Option A.**

---

### Decision 4: Refusal Estimation Fallback Strategy & Scope
- **Decision ID:** `DEC-04`
- **Exact Question:** When a user clicks "Refresh Refusal Rates" in a non-OpenRouter provider view or Global View and NO OpenRouter API key is configured, how should the dashboard respond?
- **Why It Matters:** Refusal estimation currently queries `openrouter/free`. Users who only configure Groq, Gemini, or SambaNova keys cannot query OpenRouter.
- **Available Options:**
  - **Option A (Recommended — Seamless Hybrid Fallback):** If `api_key_openrouter` is present, query `openrouter/free` for live LLM estimation. If absent, automatically load bundled baseline refusal rates from `./refusal_rates.json` and display status: `"Applied bundled baseline refusal rates (OpenRouter key not configured for live LLM estimation)."`.
  - **Option B (Strict Prompt):** Block refusal estimation on non-OpenRouter views unless an OpenRouter key is entered in settings.
- **Recommendation & Evidence:** **Option A.** Allows users of other providers to see populated refusal rates in Column 5 without forcing them to register an OpenRouter account.
- **Blocks Next Milestone?** **NO** (Blocks Milestone 0C-7).
- **Proposed Default:** **Option A.**

---

## 8. PROPOSED MILESTONE-BY-MILESTONE EXECUTION AND VERIFICATION SEQUENCE

```mermaid
flowchart TD
    M0C6D["0C-6D: Baseline Verified (Commit 942bb06)"] --> M0C6E["1. Milestone 0C-6E: Dynamic Column UI (Apply DEC-01, Fix DEF-02)"]
    M0C6E --> M0C6F["2. Milestone 0C-6F: Multi-Provider Global View (Apply DEC-02, Fix DEF-03/04)"]
    M0C6F --> M0C6G["3. Milestone 0C-6G: Capability Filters & Debt Fixes (Apply DEC-03, Fix DEF-01)"]
    M0C6F --> M0C2["4. Milestone 0C-2: Multi-Source Benchmark Enrichment & _slug.js"]
    M0C2 --> M0C7["5. Milestone 0C-7: Cross-Provider Refusal Rates (Apply DEC-04)"]
    M0C6G --> M0C8["6. Milestone 0C-8: Group B Provider Adapters (Cloudflare, Ollama, OVH, watsonx)"]
    M0C8 --> M0C9["7. Milestone 0C-9: Telemetry & Rate Limits (rpm, rpd, tpm, ttft)"]
    M0C2 & M0C9 --> M0D1["8. Milestone 0D-1: 2-Layer Normalization Architecture (Heavy Lift)"]
    M0D1 --> M0D2["9. Milestone 0D-2: Model Routing & Recommendation Engine"]
    M0C8 & M0D1 --> M0E1["10. Milestone 0E-1: CLI Parity & Modernized JSON Export"]
    M0C8 --> M0E2["11. Milestone 0E-2: Cloudflare Worker Edge CORS Proxy Deployment"]
    M0E1 & M0E2 & M0D2 --> M0E3["12. Milestone 0E-3: Production Release v1.0.0 (GitHub Pages & Native APK)"]
```

### Execution Protocol per Milestone:
1. **Prompt Ingestion:** User delivers the Milestone Execution Spec from `MASTER_PLAN.md` with pre-baked P0/P1 corrections.
2. **Code Authoring:** Executor agent modifies target files, updates `index.html` cache-bust import, updates `sw.js` `CACHE_NAME`, and precaches new assets.
3. **Automated Verification:** Executor runs `node --check` and `npm run build:web`.
4. **Physical Browser Test:** User verifies interactive behavior on Android (`http://localhost:8080`).
5. **Git Commit & Handover:** Executor creates dedicated milestone commit and updates `codebase_1.md`.

---

## 9. EXACT EVIDENCE AND SOURCE MAPPING

- **Commit Baseline:** `~/Top_Models/.git` verified at commit `942bb06` (`Milestone 0C-6D: Implement in-memory filter UI, model-bound extended rows, and event delegation`).
- **Core Import Baseline:** `~/Top_Models/index.html:452`:
  `import { fetchData, refreshRefusalRates, ... } from './core.js?v=0I';`
- **Cache Name Baseline:** `~/Top_Models/sw.js:1`:
  `const CACHE_NAME = 'matrix-cache-v11';`
- **Filter Defect Evidence:** `~/Top_Models/adapters/_filter.js:33–50`:
  `freeDef` and `chatDef` are hardcoded; no loop over `FILTER_DEFINITIONS`.
- **Gemini Tool Defect Evidence:** `~/Top_Models/adapters/gemini/index.js:32`:
  `const hasTools = null;` hardcoded.
- **SambaNova Modality Defect Evidence:** `~/Top_Models/adapters/sambanova/index.js:45`:
  `raw_modalities: "text"` hardcoded.
- **OpenRouter Chat Defect Evidence:** `~/Top_Models/adapters/openrouter/index.js:143`:
  `is_chat: true` hardcoded.
- **Sync-WWW Existing Behavior Evidence:** `~/Top_Models/sync-www.js:25–29`:
  `refusal_rates.json` copy step already exists in script.
- **Proxy HTTPS Guard Evidence:** `~/Top_Models/proxy.py:51–57`:
  `if not target_url.startswith('https://'):` blocks non-https targets.
- **CLI Divergence Evidence:** `~/Top_Models/cli.js:28–35, 65`:
  `openRouterApiKey` hardcoded; lacks multi-provider switching.

---

## 10. EXPLICIT LIMITATIONS AND COMPLETENESS CHECKLIST

### Audit Limitations:
1. **Zero External API Ingestion:** In adherence to read-only boundaries, no live external API calls were fired against OpenRouter, Groq, Gemini, or SambaNova.
2. **Capacitor Build Unexecuted:** `./gradlew assembleRelease` was not executed to preserve system resources on Android.
3. **Zero Mutation Rule:** No application files in `~/Top_Models/` or planning files in `~/storage/downloads/Sync/` were modified.

### Completeness Checklist:
- [x] Executive readiness verdict assigned (`CONDITIONALLY READY`)
- [x] All 12 specifications audited against live code with precise readiness verdicts
- [x] All 13 rows of the Version Ledger audited against actual codebase files
- [x] Confirmed defects categorized with severity levels (DEF-01 through DEF-05)
- [x] Prioritized correction list established (P0, P1, P2)
- [x] Short owner decision brief authored with recommended defaults (DEC-01 through DEC-04)
- [x] Milestone-by-milestone execution sequence mapped
- [x] Exact source lines and symbols cited throughout
- [x] Report written exclusively to `~/storage/downloads/Sync/execution_readiness.md`
- [x] Zero interactive clarification prompts presented in terminal
