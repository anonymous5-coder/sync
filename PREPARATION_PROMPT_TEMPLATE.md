# REUSABLE MILESTONE PREPARATION PROMPT TEMPLATE
*(Top_Models BYOK AI Intelligence Dashboard & CLI)*

> **Template Document Path:** `~/storage/downloads/Sync/PREPARATION_PROMPT_TEMPLATE.md`  
> **Repository:** `anonymous5-coder/sync` (`main`)  
> **Target Audience:** Project Operator, AI Planning Pair (Argon / DeepSeek), and Autonomous Executor (`agy-termux`)  
> **Workflow Stage:** Reusable Template for Stage 1 (Preparation Stage) of the Two-Stage Milestone Lifecycle  
> **Author:** AI Architectural Pair (Argon / DeepSeek / Antigravity)  
> **Date:** October 2026  

---

## I. TEMPLATE PURPOSE & OPERATIONAL INSTRUCTIONS

### 1.1 The Two-Stage Milestone Workflow
The `Top_Models` project implements 12 sequential milestones (`0C-6E` through `0E-3`). To guarantee rigorous architectural alignment, eliminate autonomous hallucinations, and protect project stability on Android Termux, **every milestone is executed through a strict two-stage cycle**:

```
+---------------------------------------------------------------------------------------------------+
|                                  TWO-STAGE MILESTONE WORKFLOW                                     |
+---------------------------------------------------------------------------------------------------+
|  STAGE 1: PREPARATION & ALIGNMENT (Read-Only Analysis)                                             |
|  1. Operator copies this template -> creates `PREPARATION_PROMPT_<MILESTONE_ID>.md`             |
|  2. Operator populates milestone placeholders with verified specs and baseline state              |
|  3. Run Preparation Prompt in Termux via `agy-termux`                                             |
|  4. `agy-termux` audits code, analyzes UX, identifies genuine owner decisions, and generates     |
|     `PREPARATION_REPORT_<MILESTONE_ID>.md`                                                        |
|  5. Operator reviews and uploads Preparation Report to ChatGPT for discussion and resolution       |
|                                                                                                   |
|  STAGE 2: EXECUTION & VERIFICATION (Implementation & Verification)                                |
|  6. ChatGPT and Operator refine the Milestone Execution Prompt with settled decisions            |
|  7. Operator delivers the refined Execution Prompt to `agy-termux`                                |
|  8. `agy-termux` writes code, runs automated checks (`node --check`, `npm run build:web`)         |
|  9. Operator performs physical interactive tests on Android (`http://localhost:8080`)              |
|  10. Executor creates dedicated git commit, updates `codebase_1.md`, and prepares next milestone   |
+---------------------------------------------------------------------------------------------------+
```

### 1.2 How to Instantiate This Template for a Milestone
1. **DO NOT run this template directly.** This file is a reusable blueprint containing generic placeholders.
2. For each upcoming milestone, copy this template to a milestone-specific prompt file in `~/storage/downloads/Sync/`:
   ```bash
   cp ~/storage/downloads/Sync/PREPARATION_PROMPT_TEMPLATE.md ~/storage/downloads/Sync/PREPARATION_PROMPT_<MILESTONE_ID>.md
   ```
   *(Example: `PREPARATION_PROMPT_0C-6E.md`)*
3. In the copied file, fill in all `{{PLACEHOLDER}}` tags located in Section II with verified information extracted from `MASTER_PLAN.md`, `codebase_1.md`, and `execution_readiness.md`.
4. Execute the populated prompt with `agy-termux`.
5. The resulting report (`PREPARATION_REPORT_<MILESTONE_ID>.md`) will be uploaded to ChatGPT to resolve decisions before code execution begins.
6. The template is reused sequentially: complete Milestone N, verify its results, and then copy this template again for Milestone N+1 using the updated codebase baseline.

---

## II. MILESTONE SPECIFIC PLACEHOLDER CONFIGURATION BLOCK
*(Operator: Populate all fields in this block before launching the preparation run)*

```yaml
# ==============================================================================
# MILESTONE CONFIGURATION METADATA (POPULATE PER MILESTONE)
# ==============================================================================
milestone_id: "{{MILESTONE_ID}}"                          # e.g., "0C-6E"
milestone_title: "{{MILESTONE_TITLE}}"                    # e.g., "Dynamic Column UI (KG_column)"
logical_phase: "{{LOGICAL_PHASE}}"                        # e.g., "Phase 0C: Matrix Maturation"
target_report_file: "PREPARATION_REPORT_{{MILESTONE_ID}}.md" # Output report in Sync/

# 1. Authoritative Specification Reference
master_plan_spec_section: "{{SPEC_SECTION_NUMBER}}"      # e.g., "Part 2, Spec 2.1 in MASTER_PLAN.md"
target_files_to_create:
  - "{{FILE_1_TO_CREATE}}"                               # e.g., "adapters/_columns.js"
target_files_to_modify:
  - "{{FILE_1_TO_MODIFY}}"                               # e.g., "index.html"
  - "{{FILE_2_TO_MODIFY}}"                               # e.g., "core.js"
  - "{{FILE_3_TO_MODIFY}}"                               # e.g., "sw.js"

# 2. Baseline & Dependencies
prerequisite_milestones:
  - "{{PREV_MILESTONE_ID}}"                              # e.g., "0C-6D (Verified in Commit 942bb06)"
expected_starting_commit: "{{BASELINE_COMMIT}}"          # e.g., "942bb06"
current_core_import: "{{CURRENT_CORE_VERSION}}"          # e.g., "core.js?v=0I"
current_sw_cache: "{{CURRENT_SW_CACHE}}"                 # e.g., "matrix-cache-v11"
target_core_import: "{{TARGET_CORE_VERSION}}"            # e.g., "core.js?v=0J"
target_sw_cache: "{{TARGET_SW_CACHE}}"                   # e.g., "matrix-cache-v12"

# 3. Known Carried-Forward Findings (from execution_readiness.md or prior reports)
carried_forward_defects:
  - "{{DEFECT_ID_AND_SUMMARY}}"                          # e.g., "DEF-02: Column key string vs numerical index lookup"
carried_forward_decisions:
  - "{{DECISION_ID_AND_SUMMARY}}"                        # e.g., "DEC-01: Array-aligned dynamic columns vs Object storage"
# ==============================================================================
```

---

## III. OPERATIONAL BOUNDARIES & SAFETY SAFEGUARDS (FOR AGY-TERMUX)

When executing an instantiated preparation prompt, `agy-termux` MUST strictly operate under read-only audit discipline:

### 3.1 Strictly Prohibited Actions
- **NO SOURCE CODE MODIFICATIONS:** Do not modify, create, touch, or delete any file in `~/Top_Models/` (`index.html`, `core.js`, `sw.js`, `adapters/*`, `proxy.py`, `cli.js`, etc.).
- **NO PLANNING ARTIFACT MUTATIONS:** Do not edit, rewrite, or delete `MASTER_PLAN.md`, `codebase_1.md`, `execution_readiness.md`, or this template.
- **NO EXECUTION ACTIONS:** Do not run build scripts (`npm run build:web`), sync tools (`npx cap sync`), or test compilers (`./gradlew`). Do not execute git commits, tags, or pushes.
- **NO INTERACTIVE TERMINAL PROMPTS:** Do NOT prompt the project owner with interactive clarification questions in Termux or use interactive agent tool calls (`ask_question`). All open decisions must be documented exclusively in the output preparation report for review in ChatGPT.
- **NO AUTONOMOUS APPROVALS:** Recommendations made in the preparation report are proposals only; never treat agent recommendations as owner approvals.

### 3.2 Exclusively Authorized Actions
- Perform read-only source code inspection, line-range reading, and non-mutating syntax checks (`node --check`).
- Inspect git status, branches, logs, and remotes without mutating working trees.
- Read authoritative planning documents in `~/storage/downloads/Sync/`.
- Create or overwrite exactly ONE report file: `~/storage/downloads/Sync/PREPARATION_REPORT_{{MILESTONE_ID}}.md`.

---

## IV. PREPARATION INVESTIGATION & REPORTING PROTOCOL

The instantiated prompt instructs `agy-termux` to perform five sequential investigative phases and compile the findings into `PREPARATION_REPORT_{{MILESTONE_ID}}.md`:

```
+---------------------------------------------------------------------------------------------------+
|                              PREPARATION INVESTIGATION PHASES                                     |
+---------------------------------------------------------------------------------------------------+
|  Phase A: Baseline Audit & Codebase Reconciliation                                                |
|  Phase B: Plain-Language Milestone Explanation & UI/UX Journey                                   |
|  Phase C: Systematic Identification of Genuine Owner Decisions                                    |
|  Phase D: Verification of Unambiguous Implementation Items                                        |
|  Phase E: Compilation of Decision-Ready Report (`PREPARATION_REPORT_<MILESTONE_ID>.md`)           |
+---------------------------------------------------------------------------------------------------+
```

---

### PHASE A: BASELINE AUDIT & CODEBASE RECONCILIATION

1. **Verify Starting State:**
   - Confirm current git HEAD commit in `~/Top_Models/` matches `{{expected_starting_commit}}`.
   - Verify active module import in `index.html` matches `{{current_core_import}}`.
   - Verify active cache container in `sw.js` matches `{{current_sw_cache}}`.
   - Record any discrepancy or uncommitted working tree changes.
2. **Audit Milestone Specification:**
   - Read the milestone execution spec `{{master_plan_spec_section}}` in `MASTER_PLAN.md`.
   - Inspect all target files (`{{target_files_to_create}}`, `{{target_files_to_modify}}`).
   - Cross-check known audit findings and carried-forward defects (`{{carried_forward_defects}}`).
3. **Distinguish Existing vs. Planned Code:**
   - Clearly delineate what code demonstrably exists in the working tree today vs. what is proposed.
   - Never assume a proposed module or export exists before it is implemented.

---

### PHASE B: PLAIN-LANGUAGE MILESTONE EXPLANATION & UI/UX JOURNEY

Explain the milestone in clear, accessible language suitable for review on a mobile device:
1. **Strategic Purpose:** Why does this milestone exist? What problem does it solve in the BYOK dashboard or CLI?
2. **What Will Change:** Enumerate concrete additions, removals, and structural refactors.
3. **User Interaction Flow (UI/UX Journey):**
   - For UI milestones (e.g. Columns, Global View, Capability Filters, Routing): Walk through the user's physical interaction on Android:
     - What buttons appear in the top bar or bottom action bar?
     - What happens when a button is tapped (popover open/close, focus, animations)?
     - How does touch ergonomics behave on mobile screens (minimum tap targets >= 44px, viewport scrolling)?
     - How do empty states, error cards, and active indicator dots visually communicate state?
   - For Non-UI / Backend milestones (e.g. Adapters, Telemetry, CLI, Edge Proxy): Walk through the user or developer interaction:
     - CLI command invocations and flag behaviors (`--free-only`, `--chat-only`).
     - Network request/response lifecycle and CORS header pass-through.
     - Offline caching, dataset hydration, and storage quota protection.
4. **Behavioral Contrast:** Provide an explicit *Before vs. After* comparison table detailing observable application behavior.

---

### PHASE C: SYSTEMATIC IDENTIFICATION OF GENUINE OWNER DECISIONS

Identify all decisions that require the owner's explicit input or preference. 

#### Rules for Identifying Decisions:
- **NO TRIVIAL ENGINEERING QUESTIONS:** Do NOT ask the owner how to write standard loops, syntax, CSS classes, or internal helper functions.
- **NO REDUNDANT QUESTIONS:** Do NOT ask questions already settled unambiguously in `MASTER_PLAN.md` or `codebase_1.md`.
- **FOCUS ON ARCHITECTURE & USER EXPERIENCE:** Surface trade-offs regarding data representation, deduplication policies, user defaults, fallbacks when credentials are missing, and Android mobile constraints.

#### Required Format for Every Genuine Decision:
Every decision must be documented using this standard schema:

```markdown
### Decision DEC-{{MILESTONE_ID}}-XX: [Concise Decision Title]
- **Exact Question:** [Clear, unambiguous question for the owner]
- **Context & Why It Matters:** [Explain the technical or UX dilemma and its architectural consequence]
- **Available Options & Trade-Offs:**
  - **Option A [Name]:** [Description] -> *Pros / Cons*
  - **Option B [Name]:** [Description] -> *Pros / Cons*
  - **Option C [Name] (if applicable):** [Description] -> *Pros / Cons*
- **Practical Consequences:** [What happens to code, storage, or UI under each option]
- **Recommendation & Supporting Evidence:** [Recommended choice with specific codebase justification]
- **Assumptions & Missing Information:** [Any unknowns affecting the recommendation]
- **Classification:** [Mandatory Blocker before execution | Optional Aesthetic/UX Preference]
- **Proposed Default:** [Default choice to execute if the owner accepts agent recommendations]
```

*Note: If a milestone is strictly technical and has zero genuine owner decisions, explicitly state: "Zero owner decisions required; implementation can follow the authoritative specification unconditionally."*

---

### PHASE D: VERIFICATION OF UNAMBIGUOUS IMPLEMENTATION ITEMS

List all technical contracts, data models, functions, and DOM modifications that are completely determined by the specification and require no owner debate:
1. **Module Boundaries & Exports:** Exact functions to export from new or modified modules.
2. **DOM IDs & Classes:** Specific elements to introduce, ensuring no collisions with existing markup.
3. **Storage Keys & Schemas:** Exact `localStorage` or `config.json` keys, with quota-safe try/catch patterns.
4. **Cache & Build Invariants:** Exact `index.html` cache-bust string (`{{target_core_import}}`), `sw.js` `CACHE_NAME` (`{{target_sw_cache}}`), and asset mirroring in `sync-www.js`.

---

### PHASE E: PREPARATION REPORT STRUCTURE (`PREPARATION_REPORT_{{MILESTONE_ID}}.md`)

The preparation run must compile all findings into `~/storage/downloads/Sync/PREPARATION_REPORT_{{MILESTONE_ID}}.md` using this exact 11-section outline:

```markdown
# MILESTONE PREPARATION REPORT: {{MILESTONE_ID}} — {{MILESTONE_TITLE}}

**Target File:** `~/storage/downloads/Sync/PREPARATION_REPORT_{{MILESTONE_ID}}.md`  
**Preparation Date:** [ISO Date / Current Date]  
**Auditor:** AI Planning Pair (agy-termux)  
**Authoritative Spec:** {{master_plan_spec_section}}  
**Execution Status:** STAGE 1 COMPLETE — READY FOR CHATGPT OWNER REVIEW  

---

## 1. EXECUTIVE SUMMARY & READINESS OVERVIEW
- Brief 2-3 paragraph summary of milestone scope and preparation findings.
- Readiness verdict: READY FOR REVIEW | BLOCKED BY PREDECESSOR | DECISIONS PENDING.

## 2. STARTING BASELINE & VERIFIED CODEBASE STATE
- Git branch, HEAD commit, and working tree clean status.
- Verification of active `index.html` import version and `sw.js` cache name.
- Status of prerequisite milestones ({{prerequisite_milestones}}).

## 3. PLAIN-LANGUAGE MILESTONE EXPLANATION & INTENT
- Plain-English explanation of milestone goals.
- Problem solved and user payoff.

## 4. USER INTERACTION FLOW & UI/UX JOURNEY (OR DEVELOPER WORKFLOW)
- Detailed walkthrough of user journey on mobile device.
- Touch interactions, popover behaviors, empty states, and visual indicators.
- (If non-UI milestone, detailed walkthrough of developer/CLI/proxy workflow).
- Before vs. After comparison table.

## 5. EXISTING IMPLEMENTATION VS. PLANNED CHANGES
- Line-by-line audit of existing contracts vs. proposed additions.
- Specific functions, variables, and DOM hooks affected in target files.

## 6. TECHNICAL DEBT, RISKS, EDGE CASES & ANDROID CONSTRAINTS
- LocalStorage 5MB quota considerations on Android Chrome/WebView.
- Network error handling, timeouts, and partial-provider failure isolation.
- Mobile viewport constraints (horizontal table scroll, fixed action bar spacing).
- Analysis of carried-forward defects ({{carried_forward_defects}}).

## 7. OWNER DECISIONS REQUIRED (CHOPPING BLOCK FOR CHATGPT)
- Numbered decision blocks (DEC-{{MILESTONE_ID}}-01, etc.) following the Phase C schema.
- (Or explicit statement if no decisions are needed).

## 8. UNAMBIGUOUS SPECIFICATION ITEMS (READY TO EXECUTE)
- Complete inventory of non-controversial implementation tasks that follow the spec directly.

## 9. LEDGER & CACHE INVALIDATION ALIGNMENT
- Exact cache-bust version bump ({{current_core_import}} -> {{target_core_import}}).
- Exact Service Worker container bump ({{current_sw_cache}} -> {{target_sw_cache}}).
- New precache assets in `sw.js` and sync verification in `sync-www.js`.

## 10. TWO-PARTY VERIFICATION PROTOCOL PREVIEW
- Automated checks to be executed by agent (`node --check`, `npm run build:web`).
- Physical mobile verification steps to be executed by user on Android (`http://localhost:8080`).

## 11. MATTERS TO RESOLVE WITH CHATGPT & FINAL STATEMENT
- Bulleted agenda for the user's discussion with ChatGPT.
- Explicit statement: "No source code in ~/Top_Models/ or planning specs in MASTER_PLAN.md were modified during this preparation run."
```

---

## V. THE HANDOFF LIFECYCLE (POST-PREPARATION WORKFLOW)

Once the preparation prompt runs and generates `PREPARATION_REPORT_{{MILESTONE_ID}}.md`, the operator and AI agents execute the following handoff sequence:

```
+---------------------------------------------------------------------------------------------------+
|                                  STAGE 2 HANDOFF LIFECYCLE                                        |
+---------------------------------------------------------------------------------------------------+
|  1. Review & Upload:                                                                              |
|     - Operator opens `~/storage/downloads/Sync/PREPARATION_REPORT_<MILESTONE_ID>.md`.           |
|     - Operator uploads or pastes the report into ChatGPT.                                         |
|                                                                                                   |
|  2. Collaborative Resolution:                                                                      |
|     - ChatGPT reviews the owner decisions in Section 7 of the report.                             |
|     - Owner and ChatGPT discuss trade-offs and select preferred options for DEC-XX.               |
|                                                                                                   |
|  3. Execution Prompt Refinement:                                                                  |
|     - ChatGPT refines the Milestone Execution Spec from `MASTER_PLAN.md`, injecting the           |
|       owner's settled decisions and resolving any carried-forward defect directives.             |
|     - The resulting text becomes the final Milestone Execution Prompt.                            |
|                                                                                                   |
|  4. Execution Launch:                                                                             |
|     - Owner delivers the finalized Execution Prompt to `agy-termux` in Termux.                    |
|     - `agy-termux` implements code, bumps cache versions, and runs automated checks.              |
|                                                                                                   |
|  5. Verification & Closure:                                                                       |
|     - Owner verifies interactive behavior on Android smartphone (`http://localhost:8080`).        |
|     - `agy-termux` creates a dedicated git commit in `~/Top_Models/`.                             |
|     - `codebase_1.md` is updated with the new factual state.                                      |
|                                                                                                   |
|  6. Sequential Iteration:                                                                        |
|     - Operator copies `PREPARATION_PROMPT_TEMPLATE.md` to create prompt for Milestone N+1.        |
+---------------------------------------------------------------------------------------------------+
```

---

## VI. INSTRUCTIONS FOR SPECIALIZED MILESTONE TYPES

The operator and agent should apply these guidelines when adapting the template to specific milestone categories:

### 6.1 Non-UI / Backend & Custom API Milestones (e.g. 0C-8, 0E-2)
- Do not manufacture artificial DOM or CSS questions.
- Section 4 must focus on developer workflow, authentication token lifecycles, proxy routing, endpoint payloads, and error codes (401, 403, 429, 502).
- Emphasize credential safety (never storing secrets in repo or logs) and network isolation.

### 6.2 Data Ingestion, Benchmarks & Telemetry Milestones (e.g. 0C-2, 0C-7, 0C-9)
- Focus on schema mapping, slug normalization coverage, offline bundled snapshot sizes, and cache hydration.
- Address rate limit handling, missing benchmark scores (null vs 0), and Safeguard #4 (never invent fake metrics).

### 6.3 Architectural Heavy Lift Milestones (e.g. 0D-1: 2-Layer Normalization)
- Focus on cache migration guards (`schema_version: 2`), backward-compatibility of existing facades (`createNormalizedModel`), and memory footprint in `localStorage`.

### 6.4 Release & Tooling Milestones (e.g. 0E-1, 0E-3)
- Focus on CLI cross-platform behavior, Termux clipboard integration, native Capacitor Android APK compilation, signed release assets, and final git push authorization.

---

## VII. TEMPLATE VERIFICATION & REUSABILITY CONTRACT

- **Self-Contained Blueprint:** This template contains all structural contracts required to prepare any of the 12 milestones without referencing external scaffolding.
- **Milestone Neutrality:** The template does not favor any single milestone; it becomes specific only after an operator populates the metadata block in Section II.
- **Planning Directory Anchor:** All derived preparation prompts and generated reports reside in `~/storage/downloads/Sync/` (`anonymous5-coder/sync` repository), keeping planning records completely isolated from the `~/Top_Models/` application source code.
