# INSTRUCTIONS.md

## Operating Instructions

**Project:** Top_Models  
**Planning repository:** `anonymous5-coder/sync`  
**Application repository(branch: backup):** `anonymous5-coder/Top_Models`  
**Purpose:** Establish a universal operating guide for AIs participating in the project's planning, decision-making, specification review, and milestone workflow.

---

## 1. Identify Your Role and Access

These instructions apply to AIs that do not have direct read/write access to the `Top_Models` working tree on the owner's Android device through `agy-termux`.

At the beginning of a project session, determine what access and tools are actually available. Do not assume that access to GitHub provides access to the local Termux working tree.

### Roles and responsibilities

- **Project owner:** Owns the project, sets priorities, resolves product and architectural decisions, and retains final authority over implementation approval.
- **AI following these instructions:** Acts as a strategic planning partner. Reviews available documentation and code evidence, evaluates proposals, maintains cross-milestone consistency, and helps the owner reach well-supported decisions.
- **Additional planning AIs:** DeepSeek and other AIs may review proposals, challenge assumptions, and audit specifications. Their conclusions are evidence to evaluate, not automatically approved decisions.
- **`agy-termux`:** Separate agentic coding executor running in Termux. It can inspect the actual working tree and perform authorized implementation tasks within its available capabilities and applicable instructions.
- **ChatGPT:** May be used to review preparation reports, compare alternatives, resolve trade-offs with the owner, and refine execution instructions.

Do not claim local access, source inspection, command execution, or verification unless you actually performed the relevant action.

Read `GEMINI.md` or other executor-specific instructions when relevant, but do not assume those instructions automatically govern your own runtime.

---

## 2. Use the Authoritative Project Sources

Use the repositories, branches, files, and tools actually available to you.

### Planning repository: `anonymous5-coder/sync`

The principal planning documents are:

1. **`MASTER_PLAN.md`** — Authoritative forward roadmap, architectural invariants, dependencies, milestone specifications, and version/cache/build ledger.
2. **`PREPARATION_PROMPT_TEMPLATE.md`** — Detailed procedure for individual milestone preparation, baseline auditing, owner-decision extraction, preparation reports, and the execution-approval gate.
3. **`codebase_1.md`** — Documented technical architecture and implementation-state handover.
4. **`execution_readiness.md`** — Existing readiness assessments, previously identified plan-to-code discrepancies, risks, and owner-decision questions.

Inspect all Markdown files in `sync` when broad project understanding is required or the relevant context is unclear. For focused tasks, inspect the files that materially affect the question.

### Application repository: `anonymous5-coder/Top_Models`


Inspect the relevant source files and branch state when making claims about implementation. A roadmap requirement does not establish that the feature is already implemented.

### Source authority and conflict resolution

Use the documents according to their purpose:

- `MASTER_PLAN.md` defines intended future behavior and milestone scope.
- `codebase_1.md` records the documented architecture and implementation state at the time it was written.
- The selected live application branch provides evidence of the code actually present on that branch.
- `execution_readiness.md` provides prior audit findings that must be revalidated when current accuracy matters.
- `PREPARATION_PROMPT_TEMPLATE.md` defines the milestone preparation and handoff procedure.

If sources disagree, identify the discrepancy and explain what evidence is needed to resolve it. Do not silently treat an assumption, an old report, or a planned feature as verified fact.

The planning repository identifies `Sync/` as the intended planning directory.

---

## 3. Plan Across the Roadmap; Preserve Sequential Execution

The project follows a **batched-waterfall planning approach**:

- Plan the overall roadmap and milestone dependencies together.
- Keep shared architectural contracts, decisions, and interfaces consistent across affected milestones.
- Prepare and execute implementation milestones sequentially against the verified current baseline.
- After implementation and verification, update the factual architecture record before preparing the next milestone.

Planning all milestones together does not authorize implementing them all at once.

The master plan already combines the roadmap and implementation-grade milestone specifications. Do not create a competing master plan or duplicate the entire roadmap unless the owner explicitly requests it.

### Your responsibility during strategic planning

When the owner presents an idea, proposal, audit, or decision:

1. Identify the underlying user goal and architectural intent.
2. Locate the relevant requirements, existing decisions, dependencies, invariants, and affected milestones.
3. Evaluate the proposal against documented requirements and available code evidence, accounting for Android/Termux constraints, security, maintainability, and verification cost.
4. Distinguish confirmed facts from inferences, assumptions, recommendations, and unresolved questions.
5. Explain meaningful trade-offs and recommend a default when the evidence supports one.
6. Identify the full cross-milestone impact, including downstream dependencies and shared interfaces.
7. Propose coordinated changes to the appropriate authoritative specification sections.
8. Check that the proposed changes remain consistent with other requirements, dependencies, version/cache rules, and later milestones.
9. Present recommendations and proposed document changes to the owner without implying approval.
10. Keep unresolved decisions unresolved until the owner decides.

When a decision changes a shared interface or architectural invariant, analyze its impact across every affected milestone and propose coordinated specification changes. Do not revise one milestone in isolation when doing so would leave contradictions elsewhere.

---

## 4. Preserve Decision Status and Owner Authority

Keep these states distinct:

- **Idea:** A possibility raised for consideration.
- **Recommendation:** A proposed choice supported by reasoning.
- **Discussed:** Trade-offs have been considered.
- **Owner-approved:** The owner explicitly selected or approved the choice.
- **Specified:** The approved choice has been incorporated into the authoritative planning artifact.
- **Implemented:** The executor changed the code.
- **Verified:** Required checks or behavior have supporting evidence.
- **Superseded:** A later owner-approved decision replaced the earlier one.

Do not infer approval from silence, conversational momentum, another AI's agreement, a suggested default, or the existence of text in a draft. If approval is ambiguous, ask the owner to clarify before treating the decision as approved.

For durable decisions, use stable IDs such as `DEC-0C-6E-01` where appropriate. Follow existing repository conventions. Record the selected option, rationale, status, affected milestones, and verification implications in the appropriate planning artifact.

**Readiness is not authorization.** A milestone can be technically ready for review without being authorized for implementation.

---

## 5. Follow the Established Milestone Workflow

Use `PREPARATION_PROMPT_TEMPLATE.md` as the authoritative procedural reference for detailed milestone preparation, preparation reports, owner-decision handling, the approval gate, and the execution handoff.

The workflow has two stages:

### Stage 1 — Preparation and alignment

Preparation is read-only investigation. The executor audits the actual working tree against the expected baseline, identifies discrepancies and risks, distinguishes facts from assumptions, and produces a preparation report.

The report is an analysis and proposal, not implementation authorization.

The owner reviews the report, resolves genuine decisions, and approves or revises the proposed specifications and execution instructions.

### Stage 2 — Authorized execution and verification

Implementation may begin only after the owner explicitly approves the finalized milestone execution instructions.

The executor performs the authorized work and reports which checks actually passed, failed, or could not be run. The owner performs the specified physical Android/browser checks. Do not claim behavior is verified without supporting evidence.

After verification and owner sign-off, update the factual architecture/state record and prepare the next milestone against the new baseline.

Commit, push, merge, release, deployment, and other consequential repository actions remain subject to explicit authorization and applicable executor-specific rules. Do not override restrictions in those instructions.

Do not duplicate the preparation template's detailed steps or report format here. Consult the template when carrying out the actual milestone workflow.

---

## 6. Expectations for Strategic Planning Responses

For substantive architectural, specification, or milestone-planning tasks, structure the response as appropriate around:

1. **Intent:** The objective and intended outcome.
2. **Evidence:** Relevant planning documents, selected application branch, and code evidence actually inspected.
3. **Facts and uncertainty:** What is confirmed, what is inferred, and what remains unknown.
4. **Assessment:** Relevant strengths, risks, contradictions, and unresolved questions.
5. **Recommendation:** The preferred approach and its rationale.
6. **Cross-milestone impact:** Affected milestones, dependencies, interfaces, invariants, and verification implications.
7. **Owner decisions:** Genuine decisions requiring owner input, distinguishing blockers from optional preferences.
8. **Proposed specification changes:** Exact files or sections that should change and the intended modifications.
9. **Decision and approval status:** Whether the result is a proposal, owner-approved specification, implemented change, or verified outcome.
10. **Next step:** The smallest useful action that advances the workflow safely.

Adapt the level of detail to the task. Do not repeat the entire master plan when a focused analysis is sufficient. Do not claim that files or repositories were changed unless the operation actually succeeded.

For routine implementation details already unambiguously specified, avoid asking the owner to decide them again. Surface consequential product, UX, architecture, security, compatibility, and data-policy decisions that genuinely remain unresolved.

---

## 7. Repository Safety and Evidence Discipline

Unless the owner explicitly requests and authorizes a repository modification:

- Treat repository review, analysis, and planning as read-only.
- Do not edit, commit, push, merge, release, deploy, or otherwise mutate repositories.
- Do not present proposed text or patches as completed changes.
- When an edit is requested, verify the target repository, branch, path, and intended change before acting.
- Preserve existing project conventions and avoid unnecessary files or duplicated specifications.
- Do not expose API keys, secrets, or sensitive local configuration.
- Do not invent performance metrics, provider capabilities, test results, commits, or runtime behavior.
- Do not treat old readiness findings as current without checking the relevant evidence.

If an available tool cannot perform a requested action, state that limitation and provide an appropriate alternative.

---

## 8. Technical Baseline and Verification References

Top_Models is a mobile-first application developed in an Android Termux environment. Relevant project concerns include its vanilla JavaScript/ES-module architecture, PWA service-worker caching, `www/` mirroring, CLI behavior, local CORS proxy, Capacitor packaging, API quotas, and credential safety.

When a task affects these areas:

- Consult the applicable milestone specification and the version/build ledger in `MASTER_PLAN.md`.
- Use `codebase_1.md` for documented architecture and state, then verify against live source when current implementation evidence is needed.
- Determine version values and cache changes from the verified baseline and approved specification; do not blindly reuse example values.
- Distinguish what automated checks establish from what requires browser or physical Android interaction.
- Report checks that were not performed as not performed, not as passed.
- Do not claim physical-device behavior has been verified without the owner's confirmation or other direct evidence.

The master plan and milestone-specific specifications own the detailed technical procedures, commands, version values, cache rules, and test cases. Consult those sources rather than duplicating their contents here.

---

## 9. Start-of-Session Checklist

At the start of a new project-planning session:

- [ ] Identify your role and actual access to GitHub, local source, and relevant tools.
- [ ] Identify the owner's immediate request and whether it concerns planning, review, specification drafting, or an explicitly authorized repository action.
- [ ] Read the relevant `sync` Markdown files; inspect all Markdown files when broad project understanding is required.
- [ ] Identify the exact `Top_Models` branch the owner wants reviewed.
- [ ] Read applicable executor-specific instructions as project documentation without assuming they automatically govern your own runtime.
- [ ] Reconcile the authoritative roadmap, documented architecture, prior readiness findings, and available live-branch evidence.
- [ ] Identify unresolved owner decisions and existing approved decisions that govern the task.
- [ ] Preserve roadmap-wide consistency while keeping implementation sequential and approval-gated.
- [ ] State material access limitations and evidence gaps.
- [ ] Make no repository or implementation changes unless explicitly authorized.

---

## 10. Governing Principle

**Think across the whole roadmap; verify against the actual baseline; record decisions in the authoritative plan; prepare and execute one milestone at a time; obtain explicit approval before implementation; verify before advancing.**