# Claim Evidence Register — Unified Theory of Context, Discovery, and Self-Mastery

**Purpose:** source-controlled research register for claim-level audit, evidence traceability, formal qualification and disposition. This is a research artifact, not the governing execution plan and not an assertion that the framework is validated.

**Audit baseline:** `document_master_visual.md` on branch `edition`, blob `123abdbe9ad3e6c24d150e7db2f38e9562d520d5` (2,618 lines; 95 numbered sections). Section line locations below refer to this exact baseline and must be refreshed if the source changes.

**Cumulative claim-level scope at this revision:** Sections 1–95, preserved as seven separately auditable batches: §§1–15, §§16–27, §§28–40, §§41–59, §§60–74, §§75–89 and §§90–95. Each batch retains its own section boundaries, source assessments, findings and historical status. This is a first-pass claim-level source/disposition record, not completion of the full 95-section audit.

## 1. Adjudication conventions

Each entry separates:

- **Claim kind:** question, definition, formal result, mathematical identity, model, empirical/developmental claim, interpretation or methodological proposal.
- **Formal status:** whether the conclusion follows from explicit premises and a stated formal system.
- **Evidence status:** whether empirical or authoritative sources support the claim within a specified domain.
- **Disposition:** retain, revise, split, merge, downgrade, defer or reject.
- **Open dependency:** what must be completed before the claim can be finalized in the treatise.

A source is not treated as support merely because it discusses a neighbouring topic. Formal results are checked against their assumptions; empirical findings are bounded by population, task, method and outcome. A lack of evidence is not automatically a refutation.

## 2. Claim-level register: Sections 1–5

### §1 — The problem to be solved (treatise lines 31–57)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S01-Q01 | Three motivating questions: acquiring a world model; deriving unpresented conclusions; intention–behaviour divergence (L33–40) | Research questions, not factual conclusions. Their disciplinary breadth is legitimate, but each requires separate operational definitions and evidence standards. | Retain as questions; split into independently auditable workstreams. |
| S01-C01 | Four levels—physical, informational, cognitive, recursive-control—can be connected in one framework (L42–53) | This is the programme's organizing hypothesis. No source establishes the proposed integration. The levels overlap and are not necessarily mutually exclusive explanatory categories. | Retain as proposed architecture; do not call it a demonstrated unified mechanism. |
| S01-C02 | A valid theory must connect levels without conflating them (L55–57) | Methodological constraint. Supported by the need to distinguish formal entailment from empirical truth and physical quantities from psychological constructs; it is not itself an empirical discovery. | Retain; use as a cross-document editing rule. |

### §2 — What the theory is—and is not (L58–80)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S02-D01 | Four exact component names (L60–65) | Naming/identity convention supplied by the framework. Names do not establish scientific originality, validity or acceptance. | Retain exactly. |
| S02-C01 | Three epistemic labels: established constraint, derived proposition, research hypothesis (L67–73) | Useful summary labels, but they mix evidential status and logical status; a formally derived proposition may be conditional on unverified assumptions. | Revise only through the pending taxonomy crosswalk; do not silently collapse it into §15. |
| S02-C02 | Naming does not confer scientific status (L65–68) | Correct methodological warning. | Retain. |
| S02-C03 | Physical constraints alone do not explain a particular behaviour (L75–80) | Correct as a causal-explanatory boundary: the physical substrate does not uniquely specify a behavioural explanation without intermediate mechanisms, state and context. | Retain; require explicit bridge premises in §§16–26. |

### §3 — Primitive objects (L81–124)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S03-M01 | System tuple \(\mathcal S_t=(A,M_t,X_t,E_t,\Pi_t,G_t,\Theta_t)\) (L83–93) | A useful conceptual state/context inventory. It is not yet a defined state-space model or a demonstrated Markov state: component spaces, units, observability, transition rules, update ordering, noise and time-step are unspecified. Architecture A may be fixed while other components evolve. | Retain as schematic model; defer formal status until M1 and cross-component schema are resolved. |
| S03-EQ01 | Observation kernel \(O_t\sim P(O_t\mid E_t,X_t)\) (L95–97) | Standard probabilistic notation, but observation space, conditional dependencies, noise and sensor model are not defined. | Revise/specify; not independently testable as written. |
| S03-EQ02 | Internal transition \(X_{t+1}=F_A(X_t,M_t,O_t,a_t,\xi_t)\) (L99–101) | Generic state-transition representation. The disturbance \(\xi_t\), transition function and time interval are unspecified; the tuple is not shown sufficient for Markov prediction. | Retain as schematic; defer parameterization and Markov claim. |
| S03-EQ03 | Policy/action selection \(a_t\sim\Pi_t(\cdot\mid X_t,M_t,G_t)\) (L103–105) | A generic stochastic policy form. Action space, feasible set and policy class are undefined. | Retain as notation; specify when connecting to §§19–20. |
| S03-EQ04 | Memory update \(M_{t+1}=U_M(\cdots)\) (L107–109) | Generic update operator; no memory representation, update semantics or timing is specified. | Retain as placeholder; define before implementation or empirical claims. |
| S03-EQ05 | Parameter update \(\Theta_{t+1}=U_\Theta(\cdots)\) (L111–113) | Generic adaptive update; feedback, objective and constraints are unspecified. | Retain as placeholder; cross-reference the later recursive-controller specification. |

### §4 — Axioms (L125–186)

The eight items are not a homogeneous formal axiom system. They mix physical premises, modelling assumptions, broad generalizations, operational postulates and methodological cautions. No common formal language, consistency argument or derivation from a minimal axiom set is supplied.

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S04-A01 | Physical embodiment (L129–133) | For physically realized computation, physical implementation is a constitutive premise. It does not by itself specify an energy cost for a particular inference or action. | Retain as a physical premise; link to later Landauer scope, not behavioural coefficients. |
| S04-A02 | Structural dependence (L135–141) | The output of a system depends on its architecture/state/input under the chosen system description. Broadly true as a functional modelling statement, but nearly definitional unless the system and output mapping are specified. | Retain as modelling principle; operationalize in each model. |
| S04-A03 | Contextual acquisition (L143–149) | Memory/representations can be updated by observations. This is a general learning architecture, not a universal claim that every system learns from every observation. | Retain with domain qualification. |
| S04-A04 | Internal transformation (L151–157) | Composition, abstraction, simulation and deduction are established computational operations. Their existence does not imply arbitrary inference or discovery of unconstrained facts. | Retain; distinguish operations and their epistemic standards. |
| S04-A05 | Bounded resources (L159–165) | Physical systems are constrained, but the listed resource quantities need domains and intervals. The energy integral requires a clear power definition and accounting boundary. Memory and processing limits are substrate/task-dependent. | Retain as constraint; specify each resource when used quantitatively. |
| S04-A06 | Adaptive selection (L167–171) | Applies to systems with multiple available actions and a selection mechanism. It is not a necessary property of every information-processing system. | Narrow to adaptive agents/controllers; classify as a model premise, not universal axiom. |
| S04-A07 | Recursive accessibility (L173–177) | Some systems can represent aspects of their own operation and use those representations to alter later processing. This is a substantive capability claim; the distinct mechanism and threshold remain unspecified. | Retain as hypothesis/functional capability; defer distinctiveness claim. |
| S04-A08 | Fallible model–world correspondence (L179–186) | Correct epistemic safeguard: internal representations can be incomplete or inaccurate. It is a methodological premise, not a mechanistic axiom. | Retain as epistemic constraint; classify separately from physical/model axioms. |

**Axiom-set disposition:** split the list into (i) physical constraints, (ii) system-model assumptions, (iii) adaptive/recursive capability hypotheses and (iv) epistemic safeguards during the controlled edition. Do not call the current list a formally established or consistency-checked axiom system.

### §5 — Definitions (L187–263)

All eight are framework stipulations, not empirical findings merely by being defined. The key audit is whether the definitions are coherent, non-circular and operationally usable.

| ID | Definition / source location | Assessment and required operational boundary | Disposition |
|---|---|---|---|
| S05-D01 | Context (L191–205) | Very broad: includes observations, memory, bodily state, goals, learned associations, constraints and architecture. This makes “processing depends on context” close to definitional. A narrower analysis must identify which context variables are causally or predictively relevant. | Retain but split context into typed subcategories; avoid using breadth to claim novelty. |
| S05-D02 | Null condition (L207–215) | Correctly requires naming which input class is absent. \(X_{external}=0\) does not imply zero memory/architecture/goals. | Retain; require a specified input channel and interval in every use. |
| S05-D03 | Intelligence (L217–226) | Explicitly operational and non-consciousness-committal. It overlaps broad adaptive-intelligence definitions and does not yet distinguish intelligence from sophisticated control or computation. | Retain as provisional framework definition; require independent tasks and discriminant criteria. |
| S05-D04 | Novelty (L228–234) | Relational to a system's accessible records and reference set. “Accessible” needs a rule for retrieval, latent representation and implicit encoding. | Retain; define reference set and access test. |
| S05-D05 | Discovery (L236–242) | Combines system-relative novelty with justification by derivation, prediction or evidence. These are distinct routes with different epistemic strengths. | Split into deductive discovery, predictive discovery, abductive proposal and empirically corroborated discovery. |
| S05-D06 | Habit (L244–249) | Captures reduced dependence on deliberation but risks conflating automaticity, goal-directedness and cached value. | Retain provisionally; map to distinct habit constructs and validated measures in later sections. |
| S05-D07 | Distraction (L251–256) | Functional displacement is a useful neutral definition, but “limited resources” and “selected objective” need measurable windows and opportunity definitions. | Retain; operationalize by task displacement, duration and recovery. |
| S05-D08 | Self-mastery (L258–263) | Normative/functional construct combining goal maintenance, revision, execution and regulation. It needs separate measures and must not be validated by the same score used to define it. | Retain provisionally; require independent functional outcomes and non-circular criteria. |

## 3. Claim-level register: Sections 6–11

### §6 — Formal statement of Space or Null Theory (L264–274)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S06-C01 | Meaningful processing is conditioned by internal structure and available contexts (L266–269) | As phrased with §5's very broad context definition, the statement risks being true by definition. Situated/embodied cognition and ordinary stateful computation are close neighbours; no distinct mechanism or prediction is supplied. | Downgrade to a general organizing principle; originality remains unestablished. |
| S06-C02 | New external observations can alter a model; internal processing can continue without new external observations (L270–274) | The two cases are logically compatible. The second is conditional on retained state and an active transition process; absence of new input does not guarantee that processing continues. | Retain with explicit conditions; test only in a specified system. |

### §7 — Information-theoretic formulation (L275–316)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S07-EQ01 | \(I(W;O\mid M)=H(W\mid M)-H(W\mid M,O)\) (L282–290) | Standard conditional mutual-information identity for a specified joint distribution, with the usual discrete or continuous regularity/finite-information qualifications. Shannon's information theory supplies the foundational framework; a modern information-theory text is needed for the exact conditional identity and continuous-variable conventions. | Retain as standard identity; define random variables and distribution. |
| S07-C01 | Positive conditional mutual information means an observation reduces uncertainty (L292–299) | Correct only as an expected conditional reduction over the relevant distribution. It does not guarantee that every realized observation reduces posterior entropy or improves a possibly misspecified model. | Revise wording to “positive expected conditional information gain.” |
| S07-P01 | Contextual acquisition can be partial (L301–308) | Follows from the definition of mutual information: information about W need not determine every other variable or fully identify W. | Retain as standard consequence; avoid implying completeness. |
| S07-P02 | No new observation does not imply no computation (L310–316) | Conditional dynamical statement: if internal state and transition rules remain active, state transitions may occur with no fresh observation. The equation does not prove that every system continues processing or that a particular internal transition is meaningful cognition. | Retain as conditional; specify system, interval and transition mechanism. |

### §8 — Newborn and empty-system thought experiment (L317–340)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S08-C01 | A newborn is not a blank machine; inherited organization, development and learning capacity precede postnatal experience (L319–323) | Supported in the narrow sense that prenatal development, sensory exposure and early neural organization contribute to neonatal capacities. DeCasper & Spence (1986) demonstrate a specific prenatal auditory-exposure effect on newborn preference; Weiss et al. (2024) review prenatal/perinatal developmental trajectories; Dehaene-Lambertz & Spelke (2015) review early neural and cognitive capacities. These do not establish adult-like reasoning, comprehensive innate knowledge or the full contents of a newborn's representations. Innate predisposition must be distinguished from prenatal learning. | Retain with narrow developmental wording and sources; do not infer adult-like intelligence. |
| S08-C02 | Artificial neural networks carry architecture and parameters shaped by design/training (L325–327) | Broadly accurate for trained models, but “embody a large amount of structure” is metaphorical unless the representation/parameter claim is made precise. Stored parameters do not guarantee accessible, correct or world-general knowledge. | Retain as a limited analogy; avoid equating learned parameters with explicit propositions. |
| S08-C03 | An empty-space intelligence thought experiment must specify substrate, memory, state, rules, energy, sensors and inherited structure (L329–340) | Correct specification challenge. If all operating substrate/state/rules are removed, no functioning computation is defined. If some remain, the system is not informationally/contextually empty. This is a conceptual argument, not an empirical test. | Retain; specify “absence of external input” rather than absolute nullity. |

### §9 — Central question of Out of Box Theory (L341–362)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S09-C01 | Unobserved propositions can be inferred when available premises constrain possible worlds sufficiently (L347–357) | Standard conditional consequence of deductive logic. The result concerns unobserved consequences of premises, not new information from nothing or arbitrary contingent facts. SEP Logical Consequence distinguishes deductive validity from inductive support; §10's proof assumptions must be explicit. | Retain as a bounded statement; no originality claim. |
| S09-C02 | A proposition independent of all available constraints cannot be uniquely deduced (L359–362) | Correct in the intended classical model-theoretic sense when compatible models of K disagree about p. It does not rule out probabilistic preference, abduction or later evidence. | Retain; state as logical underdetermination, not a limit on all forms of reasoning. |

### §10 — Formal epistemic model and Theorem 1 (L363–410)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S10-M01 | Possible-world model \((\Omega,K)\) and compatible-world set \(\Omega(K)\) (L365–379) | Standard semantic setup, but language, interpretation and model class must be fixed. | Retain; define model class and satisfaction relation. |
| S10-EQ01 | \(K\models p\) iff all K-models satisfy p (L381–389) | Standard model-theoretic consequence under fixed semantics. SEP Logical Consequence explains truth preservation across models and the relationship between model- and proof-theoretic accounts. | Retain as established formal definition/result. |
| S10-TH01 | If K entails p, a sound inference procedure can derive p (L391–410) | The proof currently overreaches: soundness gives derivable ⇒ entailed, not every entailed proposition ⇒ derivable. General derivability requires a proof system complete for the chosen semantics; practical derivation additionally depends on proof-search resources/decidability. K should have at least one model (otherwise classical entailment is vacuous). If the text claims actual-world truth, the actual world must satisfy K. A sound and complete system can derive every semantically entailed p in its formal language, but no computational efficiency is thereby guaranteed. | Revise theorem statement/proof to distinguish soundness, completeness, satisfiability and actual-world truth. |

### §11 — Theorem 2: underdetermination boundary (L411–430)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S11-TH01 | Two K-compatible worlds disagreeing on p imply neither p nor ¬p is entailed (L413–430) | Correct standard countermodel argument, assuming fixed semantics and at least one compatible model. It establishes non-entailment, not equal probability, rational indifference or impossibility of abductive ranking. SEP's underdetermination entry distinguishes different strengths and forms of scientific underdetermination; do not generalize this formal result to all scientific theory choice. | Retain with explicit model-theoretic scope and distinguish logical from evidential underdetermination. |

## 4. Claim-level register: Sections 12–15

### §12 — Upgraded meaning of Out of Box Theory (L431–445)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S12-C01 | Out of Box Theory: conclusions can be generated from architecture, representations, constraints and learned regularities (L433–438) | A broad synthesis of established inference and modelling operations. The phrase “not explicitly contained” must distinguish not explicitly stored from not logically implied or statistically encoded. | Retain as synthesis proposal; define novelty relative to a specified representation and access procedure. |
| S12-C02 | Six modes: combinatorial novelty, structural inference, model-based prediction, abduction, mathematical discovery, empirical anticipation (L440–445) | These are heterogeneous cognitive/epistemic processes, not one mechanism. Deductive validity does not validate abduction or induction. SEP Logical Consequence distinguishes deductive from inductive consequence; SEP Philosophy of Statistics explains that statistical inference is ampliative and model-dependent; SEP Bayesian Epistemology treats posterior updating as conditional on probabilistic norms and priors. | Split into separate claim classes and assign different tests/standards; do not infer all six from Theorem 1. |

### §13 — Information in internal architecture (L446–473)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S13-C01 | Architecture and memory are shaped by evolution, development, design, training and interaction (L448–454) | Broadly plausible but covers very different mechanisms across biological and artificial systems. Each requires a distinct account; “shaped by” does not entail accurate encoding of every world feature. | Retain only as a general hypothesis with system-specific scope. |
| S13-EQ01 | \(I(W;Z)>0\), where Z=(A,M), may hold (L456–462) | Valid only under a specified joint distribution. For a single fixed architecture A, the randomness/ensemble must be defined or A conditioned upon; otherwise the notation can imply a population distribution that is not stated. Positive dependence does not guarantee semantic representation, accessibility, predictive utility, causal relevance, robustness or out-of-distribution generalization. Shannon (1948) formalizes statistical information; it does not establish this particular system–world dependence. | Retain as a conditional modelling hypothesis; define W, Z, sampling process and distribution. |
| S13-C02 | Internal information may support prediction (L464–473) | Requires a predictive target, operational feature representation, accessible inference procedure, calibration and held-out evaluation. Mutual information alone is not a guarantee of useful prediction. | Downgrade to testable hypothesis; require prospective predictive-gain comparison. |

### §14 — Bayesian form (L474–500)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S14-EQ01 | Bayes' rule \(P(H\mid D)=P(D\mid H)P(H)/P(D)\) (L480–485) | Standard probability identity when P(D)>0. It is not a self-sufficient theory of cognition or a guarantee that chosen priors/likelihoods are well specified. | Retain as standard identity; state denominator condition and model assumptions. |
| S14-EQ02 | Posterior predictive \(P(Y\mid D)=\sum_H P(Y\mid H,D)P(H\mid D)\) (L487–492) | Correct for a discrete hypothesis/model partition; continuous parameter spaces require integration. The conditional predictive distribution must incorporate the model's parameter and observation assumptions. | Retain with discrete/continuous qualification. |
| S14-C01 | Predictions depend on prior structure, evidence and a model linking hypotheses to outcomes (L494–500) | Correct conditional description. Bayesian predictions remain model-dependent; priors, likelihoods, model misspecification and prior sensitivity matter. A Bayesian update is not automatically a literal account of brain processing. | Retain with model-adequacy and sensitivity caveats. |

### §15 — Epistemic ladder (L501–521)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S15-F01 | Six-level ladder from imagined possibility to robust explanatory structure (L503–521) | A useful editorial heuristic, not a validated psychometric or universal epistemic scale. Its levels mix logical consistency, deduction, probabilistic calibration, independent corroboration and explanatory robustness; these are not a single monotonic dimension. A claim may be formally proved but empirically irrelevant, or empirically predictive without being deductively entailed. | Retain provisionally as a communication aid; redesign as multiple status dimensions in the taxonomy crosswalk. |

## 5. Source register and exact relevance

### R01 — Shannon, 1948: information theory

Claude E. Shannon, “A Mathematical Theory of Communication,” *Bell System Technical Journal* 27(3), 379–423 (July 1948), DOI: [10.1002/j.1538-7305.1948.tb01338.x](https://doi.org/10.1002/j.1538-7305.1948.tb01338.x). Publisher record: https://onlinelibrary.wiley.com/doi/10.1002/j.1538-7305.1948.tb01338.x.

**Supports:** the mathematical framework of statistical information and communication.  
**Does not support:** that a particular architecture contains useful semantic knowledge about a particular world variable; that positive mutual information guarantees accessible or robust prediction; or that information equals meaning/truth.

### R02 — Stanford Encyclopedia of Philosophy: logical consequence

“Logical Consequence,” *Stanford Encyclopedia of Philosophy*, first published 7 January 2005; substantive revision 17 May 2024. https://plato.stanford.edu/entries/logical-consequence/.

**Relevant locations:** §§1–3, especially the distinction between deductive and inductive consequence, truth preservation over models, and soundness/completeness.  
**Supports:** the semantic/proof-theoretic distinctions used in S09–S11.  
**Does not support:** truth of the treatise's premises, practical proof-search feasibility, or empirical accuracy of predictions.

### R03 — Stanford Encyclopedia of Philosophy: scientific underdetermination

“Underdetermination of Scientific Theory,” *Stanford Encyclopedia of Philosophy*, first published 12 August 2009; substantive revision 4 April 2023. https://plato.stanford.edu/entries/scientific-underdetermination/.

**Relevant locations:** §§1–3; especially the distinction between holist and contrastive underdetermination and the warning that forms of underdetermination vary in strength.  
**Supports:** careful use of the underdetermination concept and the distinction between logical countermodels and broader scientific theory choice.  
**Does not support:** the stronger assertion that evidence can never rationally favour one theory, or that every alternative is equally justified.

### R04 — Stanford Encyclopedia of Philosophy: Bayesian epistemology

“Bayesian Epistemology,” *Stanford Encyclopedia of Philosophy*, first published 13 June 2022. https://plato.stanford.edu/entries/epistemology-bayesian/.

**Relevant locations:** §§1–2 for probabilism, conditionalization and formal Bayesian norms; later sections discuss priors and idealization.  
**Supports:** the conditional probabilistic framework in S14.  
**Does not support:** the claim that a human brain literally computes the displayed equations or that a posterior is reliable under a misspecified model.

### R05 — Stanford Encyclopedia of Philosophy: philosophy of statistics

“Philosophy of Statistics,” *Stanford Encyclopedia of Philosophy*, first published 19 August 2014; substantive revision 1 October 2025. https://plato.stanford.edu/entries/statistics/.

**Relevant locations:** §§1, 4 and 5, especially the relation between data, hypotheses, probability models, Bayesian inference and model evaluation.  
**Supports:** the distinction between deductive consequence and ampliative statistical inference, and the dependence of statistical results on models.  
**Does not support:** any specific prediction made by this treatise without a defined target, likelihood, prior, data and validation.

### R06 — DeCasper & Spence, 1986: prenatal auditory exposure

Anthony J. DeCasper and Melanie J. Spence, “Prenatal maternal speech influences newborns' perception of speech sounds,” *Infant Behavior and Development* 9(2), 133–150 (1986), DOI: [10.1016/0163-6383(86)90025-1](https://doi.org/10.1016/0163-6383(86)90025-1).

**Study scope:** pregnant participants recited a passage during the final six weeks of pregnancy; newborns showed a preference for the familiar passage compared with a novel passage, relative to a matched control condition.  
**Supports:** a narrow claim that prenatal auditory exposure can affect postnatal auditory preference.  
**Does not support:** adult-like reasoning in newborns, a comprehensive innate knowledge base, or the claim that all neonatal capacities are innate rather than learned prenatally.

### R07 — Weiss et al., 2024: prenatal and perinatal development

Staci Meredith Weiss, Ezra Aydin, Sarah Lloyd-Fox and Mark H. Johnson, “Trajectories of brain and behaviour development in the womb, at birth and through infancy,” *Nature Human Behaviour* 8, 1251–1262 (2024), DOI: [10.1038/s41562-024-01896-7](https://doi.org/10.1038/s41562-024-01896-7).

**Source type:** review.  
**Supports:** developmental continuity across prenatal, birth and infant periods, including prenatal environment and early brain/behaviour trajectories.  
**Does not support:** a specific innate reasoning capacity without a domain-specific primary study.

### R08 — Dehaene-Lambertz & Spelke, 2015: early infant brain and cognition

Ghislaine Dehaene-Lambertz and Elizabeth S. Spelke, “The Infancy of the Human Brain,” *Neuron* 88(1), 93–109 (2015), DOI: [10.1016/j.neuron.2015.09.026](https://doi.org/10.1016/j.neuron.2015.09.026).

**Source type:** review.  
**Supports:** evidence of early neural organization and early-emerging cognitive capacities, with developmental and methodological qualifications.  
**Does not support:** adult-equivalent cognition or unrestricted innate knowledge.

## 6. Consolidated findings for this batch

1. **Space or Null Theory:** its strongest defensible content in §§1–8 is a general systems observation: internal processing can continue without fresh external input when state and transition structure remain. The very broad definition of context risks making contextual dependence definitional. A distinct theoretical contribution is not yet demonstrated.
2. **Out of Box Theory:** the deductive core in §§9–11 is standard model-theoretic reasoning. It correctly rejects deduction of arbitrary facts unconstrained by premises, once the model-theoretic assumptions are stated. The six modes in §12 extend beyond deduction and need separate standards.
3. **Internal architecture and information:** the mutual-information expression in §13 is conditional on a joint distribution and is weaker than semantic knowledge or predictive utility. The latter requires independent held-out evaluation.
4. **Bayesian prediction:** §14 states standard conditional updating and prediction, not a new inference mechanism. Priors, likelihoods, model adequacy and sensitivity remain material.
5. **Epistemic taxonomy:** §2 and §15 are not safely reducible to one ordinal ladder. Claim kind, formal validity, empirical/predictive/causal support and disposition should be represented as separate dimensions in a later controlled revision.
6. **Developmental example:** §8's “not a blank machine” analogy is supportable only in a narrow developmental sense; prenatal learning and early neural organization do not establish adult-like reasoning.
7. **Originality:** no claim in this batch has yet demonstrated incremental predictive advantage over ordinary stateful computation, formal logic, information theory or Bayesian inference. This is a provisional comparative disposition, not a final rejection of the overall synthesis.

## 7. Historical first-batch dependency snapshot — §§1–15

This section preserves the dependencies recorded when the §§1–15 register was first completed. It is a historical status snapshot, not the current execution queue. Later work is reconciled below without erasing the original batch boundary or its audit history.

**Original first-batch dependencies (preserved):**

- Complete the source-to-claim map for §§16–27, then §§28–40, and continue in baseline section order.
- Add primary-source locations where reviews currently provide only contextual support.
- Reconcile §2's three labels with §1's claim categories and §15's multidimensional evidence ladder without silently rewriting the treatise.
- Complete the full formal premise map and cross-reference the detailed M1–M18 audit.
- Preserve the distinction between “not explicitly stored,” “not logically entailed,” “statistically predictable” and “empirically corroborated.”
- Reopen S08 if new developmental evidence changes the scope of the newborn example.
- Do not mark Section 12.2, 12.5, 12.6 or Section 13.1 complete on the basis of this first batch alone.

### Reconciliation against subsequent work through §§28–40

| Original dependency | Current assessment | Later work / remaining boundary |
|---|---|---|
| Source-to-claim mapping for §§16–40 | **Partially addressed** | Claim-level entries and evidence assessments now cover §§16–40 in Sections 8, 11 and their associated source registers. The three batch histories remain distinct. This does not complete exact source-side pinpointing, full primary-source verification or all claim-to-source links. See the batch records and commits `78038513a90cd763b8b65784730ca1894cf8f6a8` and `9c19a49eb1e18bcac37247d0f8a8a44bdd115837`. |
| Primary-source locations where reviews provide contextual support | **Partially addressed; still open** | Primary and authoritative sources have been added for selected consequential claims, including physical/neural energetics, learning, habit, interventions and control. Exact pages, sections, equations, tables, figures or result locations remain to be verified claim by claim; contextual reviews must not be presented as direct experimental support. |
| Epistemic taxonomy crosswalk | **Open** | The mismatch among §1, §2 and §15 remains unresolved. Preserve the independent dimensions of claim kind, formal validity, empirical/evidential support, disposition and unresolved dependency. No taxonomy has been silently replaced. |
| Full formal premise map and M1–M18 cross-reference | **Partially addressed; still open** | A first-pass theorem/proposition premise map and M1–M18 audits exist in the governing-plan history. Their assumptions, proof corrections, cross-section dependencies and final claim dispositions still require integrated verification. |
| Distinguish stored, entailed, predictable and corroborated information | **Partially addressed** | The §§1–15 findings and §§28–40 information/inference assessments distinguish logical entailment, statistical dependence/prediction and empirical corroboration. The distinction must still be applied consistently across the remaining claims and final synthesis. |
| Reopen S08 if developmental evidence changes its scope | **No reopening trigger established in the subsequent pass** | The narrow prenatal auditory-learning qualification remains; no adult-like neonatal reasoning claim is supported. Retain the conditional reopening rule rather than treating it as a resolved universal question. |
| Sections 12.2, 12.5, 12.6 and 13.1 | **Open** | Section coverage and first-pass claim batches do not satisfy exhaustive claim coverage, source pinpointing, final knowledge-status adjudication or completion review. These gates remain active. |

**Historical first-batch status:** §§1–15 received a first claim-level source/disposition pass. Subsequent work through §§16–40 improves cumulative coverage but does not complete the 95-section audit, validate the framework, or promote any provisional claim to empirical establishment.


## 8. Claim-level register: Sections 16–27

### §16 — Physical–cognitive bridge (treatise lines 522–558)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S16-C01 | Physical resource constraints connect bounded computation, cost-sensitive control, action selection and habit persistence (L524–550) | The sequence is a mechanistic research hypothesis, not a derivation from physical embodiment alone. Each arrow requires an independently supported bridge: substrate energetics → task-relevant resource constraints → subjective/control costs → arbitration → learned cue-policy persistence. The neural-energy literature supports physical signalling costs, but does not establish that an individual's task avoidance is caused by energy expenditure. | Downgrade “derived” to “proposed mechanistic bridge”; assess each link separately. |
| S16-C02 | Thermodynamic entropy, Shannon entropy, distraction and mental effort are distinct constructs (L528–535) | Correct category boundary. They may be connected by models but are not interchangeable quantities. | Retain as a governing safeguard. |
| S16-EQ01 | Psychological distraction is not identical to thermodynamic entropy (L537–541) | Correct rejection of a category identity; no formal mapping or empirical identity is supplied. | Retain. |
| S16-EQ02 | Six-stage physical-to-behavioural bridge (L543–550) | A proposed causal/mechanistic chain. The arrows are not mathematical implications and need separate evidence and possible falsifiers. | Retain as a research model; label each arrow as proposed until tested. |

### §17 — Physical computation and energy (L559–588)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S17-C01 | Computation is physically implemented through substrate state changes (L561–565) | Established physical-computation premise at this level of abstraction. It does not determine a universal energy cost for each logical operation. | Retain; keep the claim at the physical-implementation level. |
| S17-EQ01 | First-law accounting \(\Delta U=Q+W\) (L567–577) | Correct under the stated convention if Q is heat added to the system and W is work done on the system. Other sign conventions reverse one or both signs. The current text says “chosen sign convention” but should explicitly name it. | Retain with sign convention defined. |
| S17-EQ02 | Landauer bound \(Q_{min}=k_BT\ln2\) for erasure of one unbiased bit (L579–585) | Established conditional result for logically irreversible erasure under the relevant thermal assumptions; not a universal lower bound on every logical operation, not the actual energy of a human thought, and not an estimate of neural task cost. Landauer (1961) states the principle; Bérut et al. (2012) experimentally approached the bound in a controlled one-bit colloidal-memory system. Practical erasure commonly dissipates more. | Retain with exact operation, bit-state assumptions and thermal conditions; do not use as a neural-energy conversion factor. |
| S17-C02 | Information processing has energetic and temporal implementation costs (L587–588) | Broad physical statement is defensible; the magnitude and relevant resource cost are substrate-, operation- and timescale-dependent. | Retain with scope qualification. |

### §18 — Brain as an open non-equilibrium system (L589–623)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S18-C01 | Brain is an open, non-equilibrium biological system (L591–594) | Well-established physiological description. | Retain. |
| S18-EQ01 | Decomposed brain-power budget \(P_{brain}=P_{baseline}+P_{signalling}+P_{plasticity}+P_{regulation}\) (L596–603) | A conceptual bookkeeping decomposition, not a validated additive partition with independently measurable, non-overlapping terms. Neural energy use is distributed and measurement-dependent. Attwell & Laughlin (2001) estimate components of excitatory signalling from anatomical/physiological data in rodent grey matter; this is a model-based budget, not a direct human task experiment. Raichle & Gusnard (2002) emphasize the substantial baseline energy budget. Kondrakiewicz & Nawrocka (2025) review evidence that cognitive tasks typically produce minimal or no increase in whole-body energy expenditure, while neural signalling remains metabolically costly. | Retain as conceptual decomposition; do not present terms as separately identified measurements. |
| S18-C02 | The brain allocates limited metabolic resources across listed processes (L605–615) | The brain's energy use supports multiple concurrent physiological and neural functions, but the list does not demonstrate a single centrally allocated budget or a direct trade-off for every task. | Narrow to distributed metabolic demands; defer claims of specific allocation mechanisms. |
| S18-C03 | Difficult tasks may impose different control demands than familiar routines (L617–623) | Plausible and consistent with cognitive-control research, but “control demand” is not equivalent to incremental whole-brain energy expenditure. Otto et al. (2026) review competing information-theoretic, psychological and biological accounts of experienced effort and identify unresolved mechanisms. | Retain as a task-demand hypothesis; measure subjective effort, performance and physiology separately. |

### §19 — Action score and softmax (L624–665)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S19-M01 | Additive action score \(Q(a)=R+L-\rho E-\gamma C_{ctrl}-\delta D-\kappa K\) (L626–649) | A candidate decision model, not an established neural law. Terms must refer to the same decision horizon and be commensurate after weighting. E (metabolic energy), subjective effort, control demand, delay and switching costs are distinct quantities; the coefficients need units, identification, estimation and sensitivity analysis. Double counting between R/L and immediate/delayed costs is possible. | Retain as a provisional model specification; do not infer biological coefficients or causal mechanisms from the equation alone. |
| S19-M02 | Softmax action-selection distribution (L651–663) | Standard stochastic choice rule for a finite nonempty feasible action set. The inverse-temperature parameter β has reciprocal score units; a higher-scoring action is more probable when β>0, not certain. The model requires a defined feasible set and empirical fit. | Retain as a candidate choice model; specify action set, score scale and β. |
| S19-C01 | The score is not a literal claim about a central brain computation (L664–665) | Appropriate model/implementation boundary. | Retain. |

### §20 — Local action advantage and Proposition 3 (L666–725)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S20-C01 | A familiar competing action can outrank a long-term goal under current local conditions (L668–692) | A plausible consequence of the proposed score if immediate value and cost advantages outweigh the long-term-value difference. It is not a universal explanation for intention–execution gaps. | Retain conditionally; tie to a specified choice model and measured context. |
| S20-P03 | Inequality in the derivation implies \(Q(a_h)>Q(a_f)\) (L694–725) | Algebraically valid under the stated additive score definitions. Under softmax with β>0 the higher-scoring action has higher selection probability; under a greedy selector it is selected if uniquely maximal. The derivation does not establish that real habits have the stipulated scores or that learning strengthens the policy. | Retain as a conditional algebraic proposition; separate score ordering from empirical behaviour. |

### §21 — Habit as cached policy (L726–755)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S21-C01 | Habit as a cached policy reducing repeated deliberation (L728–740) | Useful computational analogy, but not a complete or universally accepted definition of habit. Model-free reinforcement learning is one influential operationalization, not interchangeable with every behavioural/neuroscientific habit construct. Habit expression is context-sensitive and can be dissociated from model-free task performance; Sjoerds et al. (2016) and later human-habit methodology reviews caution against treating tasks as interchangeable. | Retain as one candidate computational account; distinguish automaticity, outcome insensitivity, stimulus-response learning and model-free value. |
| S21-EQ01 | \(C_h<C_m\) (L742–746) | This is an assumption defining the proposed efficiency advantage, not an established universal inequality for all habits and contexts. | Recast as a testable, context-specific hypothesis. |
| S21-C02 | Cached responses can become maladaptive when goals or contexts change (L748–755) | Plausible and supported by neighbouring habit/control accounts, but depends on context, outcome sensitivity and availability of alternative action. | Retain as a conditional explanatory hypothesis. |

### §22 — Cue learning and temporal-difference update (L756–780)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S22-EQ01 | \(V_{t+1}(c,a)=V_t(c,a)+\alpha[r_t+\gamma V_t(s_{t+1})-V_t(c,a)]\) (L760–771) | The expression is TD-like but mixes an action-value term indexed by (c,a) with a state-value term indexed by s'. It is not a fully specified standard SARSA or Q-learning update. For state-value TD(0), the updated quantity is V(s_t) with target r+γV(s_{t+1}); for SARSA, Q(s_t,a_t) uses Q(s_{t+1},a_{t+1}); for Q-learning, Q(s_t,a_t) uses max over next actions. These algorithms have different policy and target semantics. Sutton & Barto (2018), *Reinforcement Learning: An Introduction*, §§6.1, 6.4–6.5, provide the standard definitions. | Do not silently repair; specify whether V is state value or action value, define state/cue/action mapping, reward timing and chosen algorithm. Reconcile with the separate §34 and §56 recurrences before edition. |
| S22-C01 | Repeated cue–action–outcome pairings can bias later action selection (L773–780) | Broad learning claim is supported by reinforcement-learning and associative-learning research, but the particular update and neural implementation are not established by this paragraph. | Retain as a general learning hypothesis; connect to a correctly specified model. |

### §23 — Relief and negative reinforcement (L781–810)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S23-C01 | Avoidance can be strengthened when it produces relief from an aversive state (L783–799) | Correct only when the reduction/removal is contingent on the response and increases the future probability/rate of that response. APA's definition explicitly includes the consequence and subsequent increase. A momentary fall in discomfort alone does not establish negative reinforcement. | Retain with explicit contingency and future-response criterion. |
| S23-EQ01 | \(u_t>u_{t+1}\) (L789–793) | Describes a reduction in the measured discomfort variable; it is not sufficient evidence of reinforcement without a response–consequence contingency and subsequent behavioural strengthening. | Retain only as a relief descriptor; do not label it a reinforcement equation. |
| S23-C02 | Avoidance may be maintained by relief from task discomfort (L801–810) | Plausible functional hypothesis, but the relevant aversive condition, response and consequence must be measured. The same behaviour may be maintained by positive reinforcement, habit, fatigue, social context or other causes. | Retain as a candidate mechanism; require individual-level functional assessment. |

### §24 — Thermodynamic entropy and psychological disorder (L811–830)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S24-C01 | The second law does not imply that a brain locally seeks disorder or that distraction is entropy maximization (L813–822) | Correct rejection of an unsupported explanatory shortcut. The second law constrains total entropy production for the relevant system and environment; it does not by itself predict a person's choice among actions. | Retain. |
| S24-C02 | Biological organization is maintained through energy/material exchange and entropy export (L824–830) | Broad non-equilibrium thermodynamic description is defensible, but it does not explain any particular behavioural pattern without intermediate mechanisms. | Retain as physical background, not a behavioural cause. |

### §25 — Helmholtz and variational free energy (L831–846)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S25-EQ01 | Helmholtz free energy \(F=U-TS\) (L833–838) | Standard thermodynamic potential with its applicable equilibrium/thermodynamic conditions and variables. | Retain with thermodynamic system and conditions identified. |
| S25-C01 | Helmholtz free energy and variational free energy are not interchangeable (L840–846) | Correct conceptual safeguard. Variational free energy in Bayesian/statistical inference is a functional/bound used under specified probabilistic assumptions; the shared name does not make it the physical Helmholtz potential or establish that a brain literally minimizes thermodynamic F. Friston (2009) is a review of the variational/free-energy formulation in theoretical neuroscience. | Retain; explicitly name which free-energy quantity is meant at every occurrence. |

### §26 — Formal synthesis and Theorem 3 (L847–885)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S26-M01 | Six-stage physical–cognitive bridge chain (L849–865) | Restates S16-EQ02 at a more formal level. It is not a derivation from Axioms 1–5 alone; bridge premises are required for finite control capacity, cost-sensitive allocation, cached policy formation, cue-dependent execution and conflict with reflective objectives. | Merge conceptually with the canonical bridge claim; retain one full explanation and cross-reference repetitions. |
| S26-TH03 | A cost-sensitive controller may select a locally favoured habitual response that conflicts with a higher-order goal (L867–885) | Conditional result under the stipulated local objective and choice rule. Steps 1–5 can establish a score/selection conflict if the relevant score inequality and selector are specified. Step 6's claim that repetition strengthens the cue-policy association requires a learning update and is not proved by the preceding score inequality. “Rationally” means locally optimal relative to the specified objective, not globally wise or endorsed. | Split the algebraic/choice result from the learning-persistence hypothesis; supply the missing update rule before claiming the full theorem. |

### §27 — Predictions of the physical bridge (L886–900)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S27-H01–H07 | Accessibility, initiation cost, task uncertainty/effort, fatigue/stress, delayed reward and immediate relief/stimulation may shift action selection toward a competing habit (L888 onward) | These are testable hypotheses, not established universal predictors. Existing evidence supports selected mechanisms: task-specific cost-benefit arbitration (Kool et al., 2017), model-based/model-free learning as neighbouring accounts, and unresolved subjective effort mechanisms (Otto et al., 2026). This evidence does not validate the treatise's complete additive score or imply all listed factors have independent causal effects. | Retain as hypotheses; specify each predictor, outcome, time window, confound and disconfirming result. |
| S27-H08 | Environmental change may improve behaviour before urge disappears (L?; final sentence of §27) | Plausible intervention prediction: action accessibility and opportunity structure can change while urge intensity remains. It requires separate measures of urge, eligible opportunities, action selection and functional outcome; no cited source here establishes it as a universal effect. | Retain as a falsifiable hypothesis; defer empirical status. |

## 9. Additional source register: Sections 16–27

### R09 — Landauer, 1961: logical irreversibility and heat

Rolf Landauer, “Irreversibility and Heat Generation in the Computing Process,” *IBM Journal of Research and Development* 5(3), 183–191 (1961), DOI: [10.1147/rd.53.0183](https://doi.org/10.1147/rd.53.0183).

**Supports:** the relation between logically irreversible operations and physical dissipation, including the minimum heat associated with erasure under the principle's assumptions.  
**Does not support:** an energy-per-thought estimate or a behavioural action-selection coefficient.

### R10 — Bérut et al., 2012: experimental Landauer test

Antoine Bérut, Artak Arakelyan, Artyom Petrosyan, Sergio Ciliberto, Raoul Dillenschneider and Eric Lutz, “Experimental verification of Landauer's principle linking information and thermodynamics,” *Nature* 483, 187–189 (2012), DOI: [10.1038/nature10872](https://doi.org/10.1038/nature10872).

**Study scope:** controlled erasure of a one-bit colloidal memory in a modulated double-well potential; mean dissipated heat approached the Landauer bound in the long-erasure-cycle limit.  
**Supports:** experimental realization of the bound in a controlled physical memory system.  
**Does not support:** neural energy accounting or direct cognitive/behavioural applications.

### R11 — Attwell & Laughlin, 2001: neural signalling energy budget

David Attwell and Simon B. Laughlin, “An energy budget for signaling in the grey matter of the brain,” *Journal of Cerebral Blood Flow & Metabolism* 21(10), 1133–1145 (2001), DOI: [10.1097/00004647-200110000-00001](https://doi.org/10.1097/00004647-200110000-00001).

**Source type and scope:** model-based energy budget derived from anatomical and physiological data for excitatory signalling in rodent grey matter.  
**Supports:** substantial metabolic costs of neural signalling and the need for energy-efficient neural codes.  
**Does not support:** a direct human per-thought cost, a universal energy difference between difficult and easy tasks, or the treatise's action-score coefficients.

### R12 — Raichle & Gusnard, 2002: brain energy budget

Marcus E. Raichle and Debra A. Gusnard, “Appraising the brain's energy budget,” *Proceedings of the National Academy of Sciences* 99(16), 10237–10239 (2002), DOI: [10.1073/pnas.172399499](https://doi.org/10.1073/pnas.172399499).

**Supports:** the importance of the brain's baseline energy budget and the need to interpret task-related changes against substantial ongoing metabolism.  
**Does not support:** a universal mapping from subjective effort to global metabolic expenditure.

### R13 — Kondrakiewicz & Nawrocka, 2025: cognitive tasks and whole-body energy

Kacper Kondrakiewicz and Jagoda Nawrocka, “Brains are expensive, but cognition is often cheap,” *Neuroscience & Biobehavioral Reviews* 179, 106450 (2025), DOI: [10.1016/j.neubiorev.2025.106450](https://doi.org/10.1016/j.neubiorev.2025.106450).

**Source type:** review of brain-imaging and whole-body measurement evidence.  
**Supports:** cognitive tasks are typically accompanied by minimal or no change in overall energy expenditure in the evidence reviewed; resting brain activity is itself metabolically expensive.  
**Does not support:** absence of local neural signalling costs, absence of subjective effort, or a claim that every task has identical energy demands.

### R14 — Otto, Westbrook & Daunizeau, 2026: subjective cognitive effort

A. Ross Otto, Andrew Westbrook and Jean Daunizeau, “Why is cognitive effort experienced as costly?” *Trends in Cognitive Sciences* 30(7), 632–645 (2026), DOI: [10.1016/j.tics.2025.10.012](https://doi.org/10.1016/j.tics.2025.10.012).

**Source type:** review of information-theoretic, psychological and biological accounts.  
**Supports:** the subjective cost of effort is an active theoretical question with competing accounts and unresolved mechanisms.  
**Does not support:** a single established mechanism or the treatise's scalar control-cost term.

### R15 — Kool, Gershman & Cushman, 2017: cost-benefit arbitration

Wouter Kool, Samuel J. Gershman and Fiery A. Cushman, “Cost-Benefit Arbitration Between Multiple Reinforcement-Learning Systems,” *Psychological Science* 28(9), 1321–1333 (2017), DOI: [10.1177/0956797617708288](https://doi.org/10.1177/0956797617708288).

**Study scope:** two experiments testing model-based versus model-free control under task-specific accuracy and reward manipulations.  
**Supports:** adaptive allocation of model-based control in the tested tasks in response to task-specific cost-benefit structure.  
**Does not support:** a universal single arbitration mechanism, the treatise's exact additive Q(a) formula, thermodynamic-energy coefficients or a general causal account of personal distraction.

### R16 — Sutton & Barto, 2018: temporal-difference and control algorithms

Richard S. Sutton and Andrew G. Barto, *Reinforcement Learning: An Introduction*, 2nd ed. (MIT Press, 2018), especially §§6.1, 6.4–6.5. Publisher: https://mitpress.mit.edu/9780262039246/reinforcement-learning/.

**Supports:** the standard distinctions among state-value TD prediction, SARSA action-value control and Q-learning.  
**Does not support:** treating the current §22 hybrid notation as a valid named algorithm.

### R17 — APA Dictionary: negative reinforcement

American Psychological Association, “Negative reinforcement,” APA Dictionary of Psychology, updated 19 April 2018. https://dictionary.apa.org/negative-reinforcement.

**Supports:** negative reinforcement requires removal, prevention or postponement of an aversive stimulus contingent on a response, followed by an increase in the probability of that response.  
**Does not support:** classifying every momentary reduction in discomfort as reinforcement.

### R18 — O'Doherty, Cockburn & Pauli, 2017: learning, reward and decision making

John P. O'Doherty, Jeffrey Cockburn and Wolfgang M. Pauli, “Learning, Reward, and Decision Making,” *Annual Review of Psychology* 68, 73–100 (2017), DOI: [10.1146/annurev-psych-010416-044216](https://doi.org/10.1146/annurev-psych-010416-044216).

**Source type:** review.  
**Supports:** evidence for multiple reward-related behavioural strategies, model-based/model-free distinctions, interactions and arbitration mechanisms.  
**Does not support:** treating the two systems as a universal, anatomically isolated binary or proving the treatise's specific habit model.

### R19 — Nebe et al., 2024: characterizing human habits in the laboratory

Stephan Nebe, André Kretzschmar, Maike C. Brandt and Philippe N. Tobler, “Characterizing Human Habits in the Lab,” *Collabra: Psychology* 10(1), 92949 (2024), Registered Report, DOI: [10.1525/collabra.92949](https://doi.org/10.1525/collabra.92949).

**Study scope and findings:** the study compared six laboratory habit paradigms and self-report measures of real-life habits. Choice frequency influenced later choice/habit-related measures in two tasks, including a task without external reinforcement. However, the laboratory paradigms did not converge on a single common habit construct, and the task measures showed no criterion validity against the real-life self-report measures in this sample. The authors call for reassessment of laboratory habit measurement.
**Supports:** the need to distinguish repetition-based learning, reinforcement-based model-free learning, outcome-devaluation insensitivity and self-reported real-life habit; it provides direct evidence against treating the tested paradigms as interchangeable.  
**Does not support:** a universal one-dimensional habit trait, or the claim that all habits are simply cached model-free policies.

### R20 — Friston, 2009: variational free-energy formulation

Karl Friston, “The free-energy principle: a rough guide to the brain?” *Trends in Cognitive Sciences* 13(7), 293–301 (2009), DOI: [10.1016/j.tics.2009.04.005](https://doi.org/10.1016/j.tics.2009.04.005).

**Supports:** a theoretical neuroscience formulation of variational free energy in relation to inference and brain function.  
**Does not support:** identifying variational free energy with the thermodynamic Helmholtz potential \(U-TS\) in the treatise's simple action-selection model.

## 10. Consolidated findings for §§16–27

1. **Physical computation:** Landauer's principle is a real physical constraint for logically irreversible erasure under specified assumptions. It is not a human thought-energy formula.
2. **Neural energetics:** neural signalling is metabolically costly, but this does not imply that difficult cognitive tasks produce large increases in whole-body energy expenditure. The baseline/task distinction must be explicit.
3. **Subjective effort:** the mechanism of experienced cognitive effort remains unsettled; it must not be equated with measured metabolic expenditure.
4. **Action score:** the additive Q(a) and softmax are candidate decision models. Dimensional/scale consistency, parameter identification, action-set definition and empirical comparison remain open.
5. **Habit and learning:** model-free RL is a neighbouring computational account, not a complete definition of habit. §22's update is currently not a well-specified standard TD algorithm.
6. **Negative reinforcement:** discomfort reduction alone is not reinforcement; response contingency and future response strengthening are essential.
7. **Entropy/free energy:** the treatise's explicit distinction among thermodynamic entropy, Shannon entropy, psychological distraction and variational free energy is correct and should be preserved.
8. **Bridge theorem:** the physical-to-behavioural chain is conditional and incomplete; the learning-strengthening step needs a specified update rule.
9. **Predictions:** §27 contains testable hypotheses, not established universal predictors. They require opportunity-based measures, confound control and disconfirmation criteria.

**Status:** §§16–27 now have a first claim-level source/disposition register. The action-score, habit-learning and bridge claims remain provisional; the full 95-section audit is not complete.


## 11. Claim-level register: Sections 28–40

### §28 — Context as a transition-relevant condition (treatise lines 906–948)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S28-C01 | Context is any information- or constraint-bearing condition that changes interpretations or transitions (L908–930) | Useful operational proposal, but “changes the distribution” must distinguish causal intervention from observational association. A conditional distribution \(P(X_{t+1}\mid X_t,A,M_t,C_t)\) alone does not prove that manipulating C changes outcomes. A causal claim requires a defined intervention/structural causal model or suitable design. | Retain as a candidate definition; specify whether relevance is causal, predictive or computational in each application. |
| S28-EQ01 | Conditional transition distribution (L910–916) | Standard probabilistic notation, but state, action, memory and context variables, temporal index and transition assumptions remain unspecified. | Retain as schematic; define variables and causal assumptions before empirical use. |
| S28-EQ02 | Four-part context decomposition (L932–948) | Useful categories, but they are not mutually exclusive: an internal representation may encode external information; goals can be architecturally represented; social context may be both external and remembered. | Retain as a taxonomy, not a partition; define overlap and provenance rules. |

### §29 — Inference without new external input (L949–976)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S29-C01 | Inference can occur without a new external observation when internal state and rules remain available (L951–966) | Correct for ordinary computation and formal inference. It establishes neither semantic meaningfulness nor external truth. “Zero input” must be defined relative to a channel and interval; retained internal state is itself information-bearing input to the operation. | Retain with this scope; do not describe as inference from literal nothing. |
| S29-EQ01 | \(Y=\mathcal I(Z)\) (L958–962) | Generic function application, not a substantive theorem or evidence of intelligence. | Retain as notation only. |
| S29-P04 | Internal inference requires structure, not fresh sensory input (L968–976) | Follows from the specified definition of computation; it is close to definitional and does not establish that the output is valid, true, useful or novel to an external community. | Retain as a bounded proposition; remove any implication of empirical discovery. |

### §30 — Prior information and inferential novelty (L977–1010)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S30-C01 | Newly represented, deducible, probabilistically supported, empirically new and information-independent are distinct notions (L979–990) | Correct and important taxonomy. “Empirically new” needs a reference population/community and date; “information-independent” needs a defined information model. | Retain; align with §5 D04–D05 and §15's multidimensional epistemic status. |
| S30-C02 | Deterministic computation can expose implicit consequences without generating information about arbitrary unconstrained facts (L992–1006) | The data-processing inequality gives a precise Shannon-information boundary: if \(W\to Z\to Y\) is a Markov chain and Y is computed from Z, then \(I(W;Y)\le I(W;Z)\). This does not prevent a computation from making an implicit consequence explicit, changing representation, or improving practical access. The short-program/long-output example belongs to algorithmic information theory; output complexity is bounded relative to the program, input and reference machine, not necessarily “zero information.” | Retain with the Shannon data-processing condition and a separate algorithmic-information explanation. |
| S30-EQ01 | “Novel output” does not imply information from nothing (L1002–1008) | Sound as a caution, but “information” must name its measure: Shannon mutual information, algorithmic description length, semantic content or an agent's accessible knowledge are not interchangeable. | Retain; state the information notion in every formal use. |
| S30-EQ02 | “Implicit consequence” does not imply explicit prior representation (L1008–1010) | Correct distinction between explicit storage and logical entailment. | Retain. |

### §31 — Physical limits and resource vector (L1011–1056)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S31-C01 | Energy, time, memory, noise, communication, error correction and causal access constrain physical information processing (L1013–1033) | Broad engineering/physics categories are legitimate, but each has different formal bounds and operating assumptions. Landauer applies to specified logically irreversible erasure; Shannon capacity applies to a defined channel; memory capacity depends on distinguishable states, noise and error tolerance; causal access depends on the physical spacetime and sensor system. They are not one scalar limit. | Retain as a list of distinct constraints; attach the appropriate theorem/measurement to each. |
| S31-EQ01 | Landauer erasure inequality (L1035–1041) | Repeats S17-EQ02; no need for a second derivation. | Cross-reference S17-EQ02 and R09–R10. |
| S31-M01 | Resource vector \(\mathcal R=(E,T_m,B,M_c,\varepsilon)\) (L1043–1051) | Candidate engineering abstraction. E, time, bandwidth and memory are capacities/budgets; ε is a tolerated error constraint, not a resource of the same type. Units, available/consumed distinction and coupling among dimensions are unspecified. | Retain as a vector of constraints after separating capacities from quality constraints. |
| S31-EQ02 | \(\mathcal P_{max}=\Phi(\mathcal R,A,task)\) (L1053–1056) | Generic function declaration, not a derived quantitative law. Φ is unspecified and must depend on algorithm, noise, operating domain and performance metric. | Retain as schematic; do not present as a quantified result. |

### §32 — Intelligence versus computation and proposed functional (L1057–1104)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S32-C01 | Adaptive intelligence requires additional functional properties beyond fixed state transformation (L1059–1080) | A defensible operational distinction chosen by the framework, not a universally accepted necessary-and-sufficient definition. Different theories weight generalization, learning, goal pursuit, transfer and self-monitoring differently. | Retain explicitly as the framework's chosen definition; compare with established operational constructs before claiming novelty. |
| S32-EQ01 | Computation as state transformation (L1082–1086) | Broad abstraction; not a complete definition of every computational theory or physical computation. | Retain as shorthand with scope. |
| S32-EQ02 | Intelligence as adaptive use of state transformation (L1088–1092) | Stipulative functional definition. It overlaps adaptive control, learning systems and existing intelligence frameworks. | Retain as provisional definition; add discriminant criteria. |
| S32-M01 | Weighted intelligence functional \(\mathcal I=w_1G+w_2A_d+w_3P+w_4T_r+w_5R_c\) (L1094–1104) | Candidate composite index, not a validated measure. The components need operational tasks, reliability, population norms, weighting rationale, measurement invariance, convergent/discriminant validity and criterion/predictive validity. Weights must not be selected to maximize the same outcome used to validate the index. The AERA/APA/NCME Standards (2014) require validity evidence for the intended interpretation and use of test scores. | Retain as a research proposal; do not report it as an intelligence metric until independently validated. |

### §33 — Investigation A summary (L1105–1120)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S33-C01 | Investigation A is “resolved at the level of a formal framework” (L1107–1120) | The section summarizes definitions and conceptual answers, but the context criterion, resource function, intelligence functional and empirical predictions remain operationally unresolved. “Resolved” can be read as stronger than the work supports. | Downgrade to “a provisional formal outline has been stated”; retain empirical and operational questions as open. |

### §34 — Cue-response learning (L1121–1158)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S34-EQ01 | \(\Delta V_t=\alpha[r_t+\gamma V_{t+1}-V_t]\), followed by \(V_{t+1}=V_t+\Delta V_t\) (L1127–1142) | Generic TD-like update, but V is not indexed by state or action, and V_{t+1} is not defined as a next-state estimate. It cannot be independently classified as TD(0), SARSA or Q-learning. If V is a state-value function, use a state-indexed update; if Q is an action-value function, specify the next action or maximization target. Reconcile with S22-EQ01 and the separate §56 habit-strength recurrence. | Defer equation approval until one canonical algorithm, state/action indexing, reward timing and update semantics are selected. |
| S34-C01 | Cue–action–outcome learning can increase later response readiness (L1123–1158) | Broadly supported by associative and reinforcement-learning research, but cue–outcome Pavlovian learning, action–outcome instrumental learning and stimulus–response habit formation are distinct processes. The displayed TD-like update covers only a subset of these. | Split into distinct learning mechanisms; do not label them all cue-response association. |

### §35 — Reward anticipation and model-based/model-free control (L1159–1208)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S35-C01 | Anticipatory motivation and learned policy can persist despite modest experienced pleasure (L1161–1175) | The wanting/liking distinction has substantial support in incentive-salience research, particularly in addiction-related mechanisms; it should not be generalized into a universal explanation of ordinary habits. Berridge & Robinson (2016) support a dissociation between incentive “wanting” and hedonic “liking.” | Retain with domain qualification; do not equate all urges with sensitized incentive salience. |
| S35-EQ01 | Model-based value \(Q_{MB}(s,a)\) (L1177–1183) | Standard planning/RL abstraction if the transition model \(\widehat T\), reward distribution, horizon and expectation over next states are specified. | Retain as a standard model-based value form; define its model and horizon. |
| S35-EQ02 | Model-free value \(Q_{MF}(s,a)\) (L1185–1187) | Standard action-value notation, but no update rule or training assumptions are supplied. | Retain as a placeholder; do not equate it automatically with a psychological habit. |
| S35-EQ03 | Weighted arbitration \(Q_{combined}=\omega(s)Q_{MB}+[1-\omega(s)]Q_{MF}\) (L1189–1197) | Candidate mixture model. Requires \(0\le\omega(s)\le1\), comparable value scales, a defined estimator and a task-specific arbitration mechanism. Evidence supports multiple strategies and arbitration in some tasks, not a universal single-switch architecture. | Retain as one candidate model; compare with alternative arbitration formulations and task-specific evidence. |
| S35-C02 | Arbitration weight may depend on uncertainty, effort, fatigue, reliability and task demand (L1199–1208) | Plausible covariates, but their direction and relative contributions are context-dependent and need separate measurement. | Retain as hypotheses, not established determinants. |

### §36 — Cognitive-control arbitration (L1209–1250)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S36-C01 | Deliberative and automatic control can be compared by benefits and costs (L1211–1227) | This is a general normative decision rule. Shenhav, Botvinick & Cohen's Expected Value of Control framework is a close neighbour: it proposes allocating control based on expected payoff, amount of control and effort cost. Kool et al. (2017) provide task-specific experimental support for arbitration between model-based and model-free control. Neither validates the treatise's exact U/C variables or a universal neural mechanism. | Retain as a synthesis of established neighbouring models; make the relation to EVC explicit and do not claim a distinct mechanism yet. |
| S36-EQ01 | Net-utility inequality for choosing model-based versus cached control (L1229–1239) | Algebraically straightforward once U and C are defined on common scales. It does not establish that biological controllers compute this inequality literally. | Retain as a conditional decision rule. |
| S36-P01 | Allocate more deliberative control when uncertainty, changed environment, high consequences or expected error costs justify it (L1241–1250) | Normative control-design principle consistent with EVC, but requires expected-benefit and burden estimates; “more control” can itself increase cost or reduce flexibility. | Retain as design guidance with empirical qualification. |

### §37 — Sleep, stress and environment (L1251–1277)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S37-C01 | Physiological state and environment can alter action selection and control demands (L1253–1277) | Supported in selected domains, but the listed effects are not uniform. Lim & Dinges (2010) meta-analyzed 70 articles/147 tests of short-term total sleep deprivation and found domain-varying effects, including large effects on simple-attention lapses; this does not establish all effects of chronic sleep restriction or sleep disorders. Schwabe & Wolf (2009) found stress promoted habitual responding in a specific human instrumental-learning paradigm; a later study also tested stress effects in a specific task. These do not establish that all stress shifts every person toward habits. | Retain as state-variable hypotheses; specify exposure, task, population, dose and outcome. |
| S37-EQ01 | State-dependent score \(Q(a\mid s,z_t)=R(a\mid s,z_t)-C(a\mid s,z_t)\) (L1265–1273) | Generic state-conditioned decision score; z_t is not yet operationally defined and the R/C terms inherit the scaling/identification problems in S19-M01. | Retain as schematic; align z_t with canonical state schema. |

### §38 — Multi-timescale model (L1278–1293)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S38-C01 | Behavioural loops span milliseconds-to-years timescales (L1280–1293) | Useful heuristic decomposition, but the listed boundaries are illustrative rather than empirically established thresholds. Processes overlap and can operate concurrently; a cue event, learning update, habit trajectory and identity-level goal do not share one time index. | Retain as conceptual guide; label bands illustrative and define time aggregation for any study. |

### §39 — Logistic behavioural-loop model (L1294–1326)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S39-M01 | Six-variable state \(s_t=(g_t,c_t,u_t,f_t,z_t,h_t)\) (L1296–1307) | Candidate behavioural state, not shown sufficient for a Markov process or complete causal model. z_t combines task difficulty and uncertainty; f_t is fatigue/physiological state. The same symbols and constructs need alignment with §37 and the seven-variable ROOT state in §52. | Retain as a reduced behavioural state; create an explicit crosswalk and preserve abstraction-level differences. |
| S39-EQ01 | Logistic probability of competing action (L1309–1324) | Standard logistic regression form, but it assumes a linear predictor on log-odds unless nonlinear terms/interactions are added. Coefficients b_i are not estimated, predictor signs are not established, and predictors may interact or be collinear. Repeated episodes are nested within people/days and may be serially dependent; ordinary independent-observation logistic regression would be inadequate for many proposed datasets. | Retain as a candidate statistical model; define opportunity-level outcome, sampling unit, random effects/time dependence, interactions and validation procedure. |
| S39-C01 | Unwanted action is a state-dependent outcome, not a character judgement (L1324–1326) | Appropriate interpretive framing, but the proposed state model does not exhaust all biological, social, clinical or situational explanations. | Retain as a non-moralizing modelling principle, not a complete causal account. |

### §40 — Investigation B summary (L1327–1340)

| ID | Claim / source location | Assessment and evidence relation | Disposition |
|---|---|---|---|
| S40-C01 | Five-point summary of cue learning, wanting/liking, habits, arbitration and state effects (L1329–1340) | Summary of preceding sections, not independent evidence. Several points remain provisional: model-free control is not identical to habit; the arbitration model is task-specific; sleep/stress effects are not universal. | Retain as summary after qualifying these boundaries; do not mark Investigation B empirically resolved. |

## 12. Additional source register: Sections 28–40

### R21 — Cover & Thomas, 2006: data-processing inequality

Thomas M. Cover and Joy A. Thomas, *Elements of Information Theory*, 2nd ed. (Wiley, 2006), Chapter 2, especially §2.8, “Data-Processing Inequality.” Chapter DOI: [10.1002/047174882X.ch2](https://doi.org/10.1002/047174882X.ch2).

**Supports:** if \(W\to Z\to Y\) forms a Markov chain, then \(I(W;Y)\le I(W;Z)\); deterministic functions of Z cannot increase Shannon mutual information about W.  
**Does not support:** the claim that useful computation is impossible, or that deriving an explicit consequence is not a discovery relative to an observer.

### R22 — Cover & Thomas, 2001: Kolmogorov complexity

Thomas M. Cover and Joy A. Thomas, *Elements of Information Theory*, Chapter 7, “Kolmogorov Complexity,” DOI: [10.1002/0471200611.ch7](https://doi.org/10.1002/0471200611.ch7).

**Supports:** algorithmic/descriptive complexity as the length of a shortest program describing an object, relative to a reference universal machine.  
**Does not support:** equating algorithmic complexity with Shannon mutual information or semantic knowledge.

### R23 — Berridge & Robinson, 2016: wanting and liking

Kent C. Berridge and Terry E. Robinson, “Liking, wanting, and the incentive-sensitization theory of addiction,” *American Psychologist* 71(8), 670–679 (2016), DOI: [10.1037/amp0000059](https://doi.org/10.1037/amp0000059).

**Supports:** incentive “wanting” and hedonic “liking” can dissociate; cue-triggered incentive salience can be amplified without a matching increase in pleasure in the theory's relevant domains.  
**Does not support:** treating every ordinary urge, habit or phone check as addiction or incentive sensitization.

### R24 — Shenhav, Botvinick & Cohen, 2013: expected value of control

Amitai Shenhav, Matthew M. Botvinick and Jonathan D. Cohen, “The expected value of control: An integrative theory of anterior cingulate cortex function,” *Neuron* 79(2), 217–240 (2013), DOI: [10.1016/j.neuron.2013.07.007](https://doi.org/10.1016/j.neuron.2013.07.007).

**Source type:** theoretical review/model.  
**Supports:** a normative account in which control allocation considers expected payoff, required control investment and cognitive-effort cost.  
**Does not support:** a fully settled neural mechanism or the treatise's exact model-based/model-free mixture.

### R25 — Lim & Dinges, 2010: short-term sleep deprivation

Julian Lim and David F. Dinges, “A meta-analysis of the impact of short-term sleep deprivation on cognitive variables,” *Psychological Bulletin* 136(3), 375–389 (2010), DOI: [10.1037/a0018883](https://doi.org/10.1037/a0018883).

**Scope:** meta-analysis of 70 articles and 147 cognitive tests of short-term total sleep deprivation (less than 48 hours).  
**Supports:** sleep loss can impair cognitive performance, with effect sizes differing substantially by domain; lapses in simple attention showed a large effect in the analyzed studies.  
**Does not support:** all effects of chronic partial sleep restriction, every clinical sleep disorder, or a universal mechanism for distraction.

### R26 — Schwabe & Wolf, 2009: stress and habitual responding

Lars Schwabe and Oliver T. Wolf, “Stress prompts habit behavior in humans,” *Journal of Neuroscience* 29(22), 7191–7198 (2009), DOI: [10.1523/JNEUROSCI.0979-09.2009](https://doi.org/10.1523/JNEUROSCI.0979-09.2009).

**Study scope:** human instrumental-learning experiment testing the effect of stress on goal-directed versus habitual responding.  
**Supports:** stress can shift responding toward habit-like control in the tested paradigm.  
**Does not support:** a universal effect across stressors, tasks, populations or chronic stress exposure.

### R27 — AERA, APA & NCME, 2014: testing standards

American Educational Research Association, American Psychological Association and National Council on Measurement in Education, *Standards for Educational and Psychological Testing* (2014). Publisher/standards information: https://www.apa.org/science/programs/testing/standards and https://ncme.org/resources/books/testing-standards/.

**Supports:** validity, reliability and fairness standards for interpretations and uses of test scores; validation must match the intended population, construct and use.  
**Does not support:** the validity of the proposed \(\mathcal I\) score without actual validation evidence.

## 13. Consolidated findings for §§28–40

1. **Context:** the four-part decomposition is useful but overlapping; a transition-distribution association is not automatically a causal effect.
2. **Inference:** internal computation without fresh sensory input is ordinary conditional computation, not knowledge from nothing.
3. **Information:** the data-processing inequality gives a precise Shannon-information boundary; explicit derivation can expose implicit consequences without increasing mutual information about an external target.
4. **Intelligence:** the functional definition and weighted score are proposals. Construct validity, reliability, task sampling and independent criterion validity are still absent.
5. **Cue learning:** §34 repeats and does not resolve the state/action-value ambiguity in §22; Pavlovian, instrumental and habit-learning processes must be distinguished.
6. **Reward and habit:** wanting/liking dissociation is supported in defined domains; model-free RL is not interchangeable with the full habit construct.
7. **Control allocation:** EVC and model-based/model-free arbitration are established neighbouring theories with task-specific evidence, not validation of the treatise's exact equations.
8. **Sleep and stress:** selected experimental and meta-analytic evidence supports effects on attention/control, but does not establish universal effects or the full state-conditioned Q model.
9. **Behavioural model:** the logistic equation is a candidate statistical model; it needs opportunity-level outcomes, repeated-measures structure, parameter estimation and out-of-sample validation.
10. **Summary status:** Investigation A's “resolved” wording and Investigation B's summary must not imply empirical resolution.

**Status:** §§28–40 now have a first claim-level source/disposition register. The context definition, intelligence measure, TD update, habit/arbitration models and behavioural state remain provisional.


## 14. Claim-level register: Sections 41–59

**Baseline:** document_master_visual.md, branch edition, blob 123abdbe9ad3e6c24d150e7db2f38e9562d520d5. The section locations below refer to this unchanged 2,618-line, 95-section baseline.

This is the first claim-level evidence/disposition pass for §§41–59. It extends the earlier claim inventory (commit 965d637ad36d9e56f3b4cc6afbb701056d1e35c6) and does not authorize or report execution of experiments A–F. No treatise or tracker edits are made by this register entry.

The table makes the five assessment dimensions independently visible: claim kind, formal validity, empirical/evidential support, disposition and unresolved dependency. “Not established” is not treated as refutation. Sources support only the specific domains, populations, tasks and outcomes stated below.

| ID | Claim / exact treatise location | Claim kind | Formal validity | Empirical / evidential support | Disposition | Unresolved dependency |
|---|---|---|---|---|---|---|
| S41-C01 / S41-M01 / S41-C02 | Trigger-specific interventions may improve sustained attention; Qh=Rh−Ch, Qg=Rg−Cg, four intervention classes (L1341–1386) | Empirical hypothesis; decision-model heuristic; intervention taxonomy | Qg−Qh>0 is a score comparison only. It predicts greater selection only after a choice rule, feasible action set, common score horizon and commensurate terms are specified. | If–then planning has meta-analytic support (R31); cue accessibility and cue–response linkage have mechanism evidence (R32). Design-friction experiments report reduced screen time in some settings (R33–R34), but neither this evidence nor the implementation-intention evidence establishes sustained-attention improvement or ROOT-package efficacy. | Retain as a testable, context-bounded intervention hypothesis; do not state “yes” as an empirical answer. | Define sustained attention, eligible trigger/opportunity, target behaviour, intervention dose, comparator, fidelity, independent outcome and adverse/burden measures. Separate antecedent, interruption, consequence and retraining effects. |
| S42-C01 / S42-M01 | No universal habit-acquisition time; saturating recurrence H(t+1)=H(t)+alpha(1−H(t))R(t)−beta H(t)N(t) (L1387–1420) | Empirical generalization; proposed dynamical model | The recurrence is not a validated law. A sufficient boundedness condition is H,R,N in [0,1] and 0≤alpha,beta≤1; the treatise does not state these domains/constraints. R(t) and N(t) conflate rehearsal, non-reinforcement and competing learning. | Lally et al. (R28) observed large individual variation in self-reported automaticity; a 2024 systematic review (R29) found substantial variability and high risk of bias in many included studies. A randomized context-planning study (R30) supports a causal role for consistent context in automaticity for walking, but not a universal time law. None validates this recurrence. | Retain only as a candidate bounded model; keep the no-universal-duration statement narrowly qualified. | Define time step, scale, opportunity, cue/context, R(t), N(t), missing opportunities, extinction versus competing learning, parameter estimation and transfer. Reconcile with §56 before selecting any canonical equation. |
| S43-C01 / S43-EQ01 | Environmental leverage and Lambda=reduction in unwanted-action probability / implementation cost (L1421–1450) | Proposed metric / personal measurement convention | The ratio is definable only after numerator and denominator are operationalized. A before/after probability difference is not a causal effect without a defensible counterfactual; the ratio is not a standardized effect size. | Environmental-friction interventions provide limited, task-specific evidence (R33–R34). No source validates this ratio or its cross-intervention comparability. | Retain as a provisional within-person heuristic, not a universal leverage measure. | Define opportunity denominator, baseline risk, time horizon, counterfactual, setup and maintenance burden, side effects, zero/negative denominator cases, uncertainty and scale normalization. Report benefit and burden separately as primary quantities. |
| S44-C01 / S44-M01 | Recovery metrics and weighted composite C=w1Ag−w2Fd−w3Dd−w4Lr+w5Sc (L1451–1483) | Measurement proposal; composite heuristic | The weighted sum is algebraically valid but not interpretable until units, direction, normalization and weights are defined. Proportions, event rates, durations and latencies are not directly commensurate. Sleep regularity is listed as a metric but is not included in the displayed composite. | Task-resumption studies support measuring latency and accuracy jointly; Brumby et al. (R38) found a speed–accuracy trade-off in interruption recovery. This is not validation of the proposed composite or a universal “lower latency is better” rule. | Retain raw outcomes as primary; defer composite interpretation. | Fix opportunity windows and denominators for Ag,Fd,Sc; define episode and recovery boundaries, missingness, units, normalization, weights and sensitivity. Pair latency with resumed-task accuracy and functional output. |
| S45-C01 / S45-EQ01 / S45-C02 | Individualized observe–estimate–intervene–measure–update loop (L1484–1514) | Operational architecture; personalization hypothesis | The loop is a generic feedback schema, not a specified estimator or adaptive controller. It supplies no policy class, update rule, intervention-assignment method or stability condition. | Individual differences and contextual moderators appear in habit/intervention research (R29–R30), but do not validate this particular loop or prove that individualized adaptation outperforms fixed rules. | Retain as a workflow proposal; do not call it a validated adaptive protocol. | Specify observation model, state estimator, intervention policy, update cadence, exploration constraints, safety limits, outcomes, within-person validation and comparison against fixed/simple baselines. |
| S46-M01 / S46-EQ01–EQ03 | Self-model S_hat=M(S,observations), parameter update Theta(t+1)=Theta(t)+DeltaTheta(S_hat,G,error), and transition S(t+1)=F_Theta(t+1)(S,I) (L1515–1547) | Proposed mathematical architecture / modelling assumptions | The equations are schematic. The estimator appears to receive the true S, which is generally latent; observations/history and an observation model should be specified. DeltaTheta, objective, parameter domain, error, constraints, uncertainty and transition law are undefined. | Self-evaluation and confidence are established metacognitive topics (R36–R37); monitoring and regulation of control parameters are explicitly described as meta-control (R35). A human sequential-decision experiment also operationalized meta-control as adaptive switching between model-based and model-free strategies under manipulated reward stakes and task-transition stability (R39). These are close established neighbours, not evidence for a distinct Recursive Intelligence mechanism. | Retain as a candidate architecture, but downgrade any implication that the equations define a novel or validated mechanism. | Define what is represented about the system itself, what is merely estimated, which parameters are updated, the meta-level target and update rule, and a discriminating prediction versus metacognition, meta-control and adaptive control. |
| S47-M01 / S47-C01 | Recursive feedback loop in which an outcome modifies future parameters/policy (L1548–1571) | Conceptual model / explanatory claim | A feedback loop that changes future parameters is standard adaptive feedback; the diagram alone does not establish a distinct recursion level or a new formal result. | Established feedback, adaptive-control and meta-control literatures already contain monitoring and parameter/policy adjustment (R35–R37); R39 provides a primary human experiment of strategy adaptation to changing task demands. No incremental contribution is demonstrated here. | Merge conceptually with §§45–46 and §59 in later edition; preserve any genuinely distinct meta-level operation only if specified. | Identify the additional represented object or update level, define interfaces and compare against ordinary feedback/adaptive-control baselines. |
| S48-C01 / S48-C02 | Self-models are fallible; explanations should be judged by prospective predictions under controlled change (L1572–1590) | Methodological principle; empirical validation proposal | The principle is sound as a safeguard, but “best explanation” requires explicit competing models, predictions and a valid comparison design. A retrospective narrative is not a test. | Metacognitive judgments can diverge from objective task performance because confidence depends on fallible models of the world and cognitive system (R36–R37). This supports the need for calibration, not the accuracy of any particular self-model. | Retain as a methodological safeguard; operationalize before using it as evidence of self-model validity. | Register predictions before outcomes; use independent behavioural measures, calibration, time-ordered holdouts, alternative explanations and controlled/counterbalanced changes where safe. |
| S49-M01 / S49-EQ01–EQ02 / S49-C01 | Discounted objective J(pi) and update pi(t+1)=Update(pi(t),estimated gradient,feedback) (L1591–1625) | Reinforcement-learning objective; conceptual policy-update model | Expected discounted return is standard under a specified trajectory distribution and decision process. The update is not an algorithm: a gradient may not exist for a discrete policy or may require a parameterization; reward, cost, harm, weights, discount and horizon are unspecified. | RL and adaptive-control methods are established neighbouring frameworks. Their existence does not validate the human objective, selected weights or the claim that people literally perform gradient updates. | Retain as a schematic objective only; explicitly distinguish standard RL mathematics from a hypothesis about human cognition. | Specify MDP/POMDP assumptions, state/action spaces, reward and harm semantics, time horizon, risk constraints, parameterization, estimator and update algorithm. Test against simpler policy-learning baselines. |
| S50-M01 / S50-C01 | Ordered goal hierarchy G0≺G1≺G2≺G3 and revisable higher-level constraints (L1626–1653) | Conceptual hierarchy / normative proposal | The relation is undefined: priority, abstraction, temporal horizon and normative authority are different orderings. A total order is not justified where goals can be incomparable or mutually constraining. | Goal conflict and strategy regulation are studied in metacognition/meta-control (R35–R37); no evidence here validates this exact four-level hierarchy. | Retain as a proposed organizing model, not a universal structure of human goals. | Define ordering semantics, conflict resolution, partial/incomparable goals, legitimate goal revision and constraints against metric/goal gaming. |
| S51-C01 | ROOT Control Protocol as seven stages: Recognise, Obstruct, Override, Train, Correct, Optimise, Learn (L1654–1671) | Framework definition / operational proposal | A seven-stage list is a definition, not a demonstrated controller. Its initials spell ROOTCOL; if ROOT is intended to name only the first four stages, explain the status of Correct, Optimise and Learn. Sequence, iteration and concurrency are not specified. | Evidence for individual components exists (R28–R34), but there is no package-level efficacy evidence for this seven-stage protocol. | Retain as the named operational proposal; clarify acronym and architecture before edition. | Define stage inputs/outputs, order, feedback links, required/optional stages, fidelity, burden, adverse effects and stopping criteria. |
| S52-M01 / S52-C01 | Seven-variable ROOT state s=(c,u,f,d,g,h,e) (L1672–1691) | State-vector definition / measurement model | The vector is not a specified Markov state or a validated sufficient state. Treating it as “measured state” conflates latent constructs with subjective/observable indicators. Shared time index and ordinal ratings need operational semantics. | No validation study is supplied for this vector or its sufficiency. Existing evidence on habit and metacognition does not validate the seven-variable construct. | Retain as a provisional bookkeeping vector, not a validated state representation. | Define each construct and indicator, ordinal scale anchors, sampling window, reliability, missingness, latent/observed distinction, omitted variables and relation to the broader and six-variable states. |
| S53-M01 / S53-C01 | Trigger record E=(c,s,a,r,tau) and distinction between trigger and action (L1692–1711) | Event-schema definition / operational claim | The tuple is definitional but incomplete. Since s already includes c, cue information is duplicated unless the two fields have distinct meanings. tau is described as duration but event boundaries and duration type are not specified. | No direct evidence validates this event schema. It is a reasonable logging proposal only. | Retain provisionally; revise schema only after event-boundary and state definitions are fixed. | Define cue versus state cue indicator, event start/end, whether tau is action duration or recovery latency, consequence timing and eligible-opportunity denominator. |
| S54-C01 / S54-EQ01–EQ02 | Obstruction lowers accessibility e'<e and is expected to lower p_h(s|e) (L1712–1739) | Causal hypothesis; inequality | The accessibility inequality is a proposed intervention condition. The probability inequality does not follow algebraically from lower accessibility; it requires a monotonic response model and assumptions about substitution, competing actions and context. | Design-friction studies show context-specific changes in screen use (R33–R34), including awareness/control-group effects. This is partial support for some friction interventions, not a universal monotonic law. | Retain as a falsifiable, context-specific causal hypothesis; remove any unconditional implication. | Measure accessibility, eligible opportunities, target action and substitutions; define comparator, exposure, carryover, side effects and task output. |
| S55-C01 | If–then implementation intention maps a specified cue to a concrete alternative action (L1740–1755) | Intervention definition / empirical component claim | The cue–response mapping is a clear operational definition. It does not logically guarantee that the response will be executed. | Gollwitzer & Sheeran's meta-analysis of 94 tests found a medium-to-large average effect on goal attainment (R31). Webb & Sheeran's mechanism study found effects mediated by cue accessibility and cue–response association (R32). This supports implementation intentions as a component, not ROOT as a whole. | Retain with scope qualification and source-level support; avoid universal efficacy language. | Specify goal intention, cue specificity, response feasibility, rehearsal, opportunity, adherence and outcome. Pinpoint included study contexts and moderators before generalizing. |
| S56-M01 | Alternative-response update H_alt(t+1)=H_alt(t)+alpha S(t)−beta F(t) (L1756–1781) | Proposed learning model | Without domains or projection, the update is unbounded and can leave any intended [0,1] range. A single failure can erase or reverse a small value if beta F(t)≥H_alt(t); the prose does not follow for all parameter values. | Habit-formation evidence supports repetition/context effects but does not validate this additive recurrence (R28–R30). | Retain only as a conceptual heuristic; do not use for quantitative prediction. | Define S(t), F(t), their ranges, opportunity and reward semantics, parameter bounds, clipping/projection, decay and context dependence. Reconcile with the distinct saturating recurrence in §42. |
| S57-EQ01 / S57-C01 | Signed error e=y*−y and correction based on outcome deviation (L1782–1802) | Mathematical definition; controller proposal | The signed difference is valid if target and observation share units, scale and time window. No controller gain, update map, delay model, noise model or stability condition is supplied. The symbol e conflicts with environmental accessibility e in §52. | No source validates the proposed ROOT correction rule; standard feedback-control theory does not establish its human implementation. | Retain the error definition conditionally; defer claims of a functioning controller. | Rename one colliding symbol; define outcome vector, units, sampling, target, controller/update rule, constraints, delay and stability/overshoot checks. |
| S58-C01 | Optimisation across sleep, activity, nutrition, workload, environment, task difficulty and recovery (L1803–1819) | Broad intervention domain / normative safeguard | This is a list of candidate moderators and intervention domains, not a causal prescription or optimization algorithm. “Optimise” has no objective function or constraints here. | Evidence is domain-specific; the habit, implementation-intention and interruption sources above do not establish a universal combined recipe. | Retain as candidate contextual factors and a non-maximization safeguard; avoid implying a single intervention formula. | Define target outcomes, individual context, safe bounds, burden, adverse effects and evidence for each proposed intervention; do not infer diagnosis from tracker data. |
| S59-M01 / S59-C01 | ROOT feedback cycle; cycle output becomes context for the next cycle (L1820–1852) | Framework synthesis / feedback-model claim | The cycle repeats the seven-stage list in §51 and the generic recursive loop in §§45 and 47. It is not a formal dynamical system until state transitions, stage operators, update order and timescales are specified. | No package-level study or independent evidence for the integrated cycle is identified. Component evidence does not validate the composition. | Consolidate with §§45, 47 and 51 during a later evidence-led edition; retain the integrated-cycle hypothesis as provisional. | Define typed stage interfaces, concurrency/order, state and policy updates, feedback timing, error handling, missing data, versioning, fidelity and incremental benefit over simpler baselines. |

### Cross-section dependencies and integration findings — §§41–59

1. **Intervention and measurement layer (§§41–45):** depends on the action-score and habit constructs assessed earlier (M6, M12), and introduces leverage/composite conventions (M16, M13). The tracker retains a six-term Q(a) score in §2.2, whereas §41 reduces the comparison to reward minus cost; no mapping of delayed value, energy, control, delay and switching terms into the reduced cost is specified. These metrics do not independently establish causal intervention effects.
2. **Habit acquisition conflict (§§42 and 56):** the saturating recurrence in §42 and additive recurrence in §56 have different state bounds and learning semantics. They cannot both be treated as the canonical update for one habit-strength variable without a defined distinction or reconciliation.
3. **Recursive-control overlap (§§45–50):** §§45, 47 and 59 repeat feedback/update structures. §46's parameter update does not identify a meta-level representation or operation beyond ordinary adaptive control. Current material does not distinguish Recursive Intelligence from metacognition, meta-control or adaptive control; the primary human meta-control study R39 makes this comparator concrete rather than merely terminological.
4. **ROOT structure (§§51–59):** §51 lists seven stages, while §§47 and 59 repeat the feedback cycle. The initials form ROOTCOL; the intended acronym boundary is unresolved.
5. **State/event notation (§§52–57):** e denotes accessibility in §52 and signed outcome error in §57. The event tuple in §53 repeats cue information already contained in s. These are substantive interface/notation defects, not merely stylistic differences.
6. **Recovery measurement (§44):** return-to-task latency cannot be optimized in isolation; accuracy and functional output must be considered because task-resumption research finds speed–accuracy trade-offs. The tracker’s RTL definition is notice-to-resumption, whereas the task-resumption literature commonly measures the post-interruption interval from the end of the interruption to the first resumed primary-task action; these are not interchangeable.
7. **No empirical package conclusion:** sources support selected components under narrow conditions. They do not establish sustained-attention efficacy, ROOT package efficacy, a unique recursive mechanism, the proposed coefficients, or incremental predictive value of the integrated framework.
8. **Tracker alignment:** ROOT_Protocol_Tracker §2.3 defines RTL as t_resume−t_notice, and §14 lists shorter RTL among success criteria. Preserve it as a local notice-to-resumption measure; if comparing with post-interruption resumption lag, define and log that second interval separately. The tracker also says to retain raw measures and functional output, which is necessary given the speed–accuracy trade-off. No tracker edits were made.

### Consolidated findings for §§41–59

- Trigger-specific intervention, environmental friction and implementation intentions have evidence at component level. The effects are task- and context-dependent; no source establishes the full ROOT package or a universal sustained-attention effect.
- Habit automaticity develops with substantial individual variability. Consistent context can causally support automaticity in a specific walking intervention, but habit automaticity and behavioural maintenance are not identical outcomes.
- The two habit equations are provisional and inconsistent. Neither should be presented as a validated acquisition law.
- The leverage ratio and recovery composite are personal/model conventions. Raw rates, opportunities, durations, latencies, accuracy and functional output should remain visible.
- The self-model and policy-update equations are under-specified. Current definitions overlap established metacognition, meta-control and adaptive control; uniqueness remains unestablished, not disproved.
- ROOT is a proposed seven-stage operational architecture. Its stage interfaces, acronym, sequence, state model and quantitative correction/training rules remain unresolved.
- No experiments were executed. Protocol A–F execution gates remain open, and this evidence review does not authorize their execution.

**Status:** §§41–59 have a first claim-level assessment and source-qualification pass. Exact source-page/table/figure pinpointing is incomplete where publisher abstracts or review summaries were the accessible material; those locations are explicitly not claimed as verified. Final dispositions, full source-side verification, cross-component integration and any treatise/tracker edits remain open.

## 15. Additional source register: Sections 41–59

### R28 — Lally et al., 2010: habit formation in everyday life

Phillippa Lally, Cornelia H. M. van Jaarsveld, Henry W. W. Potts and Jane Wardle, “How are habits formed: Modelling habit formation in the real world,” *European Journal of Social Psychology* 40(6), 998–1009 (2010), DOI: [10.1002/ejsp.674](https://doi.org/10.1002/ejsp.674).

**Evidence type and design:** longitudinal real-world self-report study. Ninety-six volunteers selected an eating, drinking or activity behaviour to repeat daily in a consistent context for 12 weeks; 82 supplied sufficient data. Automaticity was measured daily using a subset of SRHI items. Individual asymptotic curves were fitted for 62 participants, with good fit for 39.

**Relevant result:** among the fitted cases, time to 95% of the modelled automaticity asymptote ranged from 18 to 254 days. Missing one opportunity did not materially affect the fitted habit-formation process.

**Supports:** repeated behaviour in a consistent context can be associated with increasing automaticity; individual trajectories vary substantially.

**Does not support:** a universal number of days, a universal latent habit-strength equation, adult attention recovery, or the §42/§56 recurrence. Automaticity is the measured outcome; it should not be treated as interchangeable with every definition of habit.

**Pinpointing status:** publisher abstract and bibliographic pages verified; exact page-level location of the detailed methods/results and any table/figure not independently verified in the accessible text. Do not invent a more precise locator.

### R29 — Singh et al., 2024: systematic review and meta-analysis of habit formation

Ben Singh, Andrew Murphy, Carol Maher and Ashleigh E. Smith, “Time to Form a Habit: A Systematic Review and Meta-Analysis of Health Behaviour Habit Formation and Its Determinants,” *Healthcare* 12(23), 2488 (9 December 2024), DOI: [10.3390/healthcare12232488](https://doi.org/10.3390/healthcare12232488).

**Evidence type and scope:** systematic review/meta-analysis of 20 studies involving 2,601 participants and health behaviours including physical activity, diet, water consumption, flossing and sedentary-behaviour reduction. Eleven studies were rated at high risk of bias. Four studies reported time-to-formation estimates.

**Relevant result:** reported habit-formation times varied widely (approximately 4–335 days); reported median estimates in the included studies were 59–66 days and means 106–154 days. Habit-strength scores improved on average, but measurement, behaviour and study quality varied.

**Supports:** substantial between-person and between-behaviour variability; frequency, timing, context and individual factors matter.

**Does not support:** a universal 66-day rule, the treatise's exact recurrence, or extrapolation from health habits to every cognitive/attention behaviour.

**Pinpointing status:** abstract and review scope/results verified; individual-study tables and exact page/table references not independently checked in the accessible full text.

### R30 — Ebert & Lin, 2024: randomized test of consistent context

Jane E. J. Ebert and Xin Yao Lin, “Confirming the Causal Role of Consistent Contexts in Developing a Walking Habit: A Randomized Comparison With Varied Contexts,” *Annals of Behavioral Medicine* 58(11), 741–751 (2024), DOI: [10.1093/abm/kaae045](https://doi.org/10.1093/abm/kaae045).

**Evidence type and design:** randomized planning intervention in 127 insufficiently active, working, midlife adults. Consistent-context planners were compared with varied-context planners and a no-planning control. Daily steps were measured by accelerometer and habit automaticity assessed over a four-week intervention and four-week follow-up.

**Relevant result:** consistent and varied context planners increased walking during intervention; only consistent-context planners developed and maintained greater habit automaticity. Contrary to expectation, the consistent-context group did not show walking maintenance. Routine daily schedules moderated some effects.

**Supports:** consistent context can causally promote automaticity in the tested walking-habit setting.

**Does not support:** that automaticity guarantees behavioural maintenance, that all behaviours share the same effect, or that context consistency alone improves sustained attention.

**Pinpointing status:** PubMed/publisher abstract and article pages verified; exact result-table and figure locations not independently checked in the accessible text.

### R31 — Gollwitzer & Sheeran, 2006: implementation-intention meta-analysis

Peter M. Gollwitzer and Paschal Sheeran, “Implementation Intentions and Goal Achievement: A Meta-analysis of Effects and Processes,” *Advances in Experimental Social Psychology* 38, 69–119 (2006), DOI: [10.1016/S0065-2601(06)38002-1](https://doi.org/10.1016/S0065-2601(06)38002-1).

**Evidence type and scope:** meta-analysis of 94 independent tests of if–then plans linking specified situational cues to intended responses.

**Relevant result:** reported a medium-to-large average effect on goal attainment (d = 0.65), with effects across initiation, shielding ongoing goal pursuit and disengagement from failing courses of action.

**Supports:** implementation intentions can improve goal attainment on average across the included tasks and contexts.

**Does not support:** guaranteed execution, universal effects, a specific ROOT protocol, or a unique Recursive Intelligence mechanism. The average does not replace examination of task, population, moderator and publication-bias limitations.

**Pinpointing status:** article metadata and abstract-level result verified; exact page/table for the pooled estimate and moderator analyses not independently checked in the accessible source.

### R32 — Webb & Sheeran, 2008: implementation-intention mechanism

Thomas L. Webb and Paschal Sheeran, “Mechanisms of implementation intention effects: The role of goal intentions, self-efficacy, and accessibility of plan components,” *British Journal of Social Psychology* 47(3), 373–395 (2008), DOI: [10.1348/014466607X267010](https://doi.org/10.1348/014466607X267010).

**Evidence type and design:** Study 1 meta-analyzed 66 tests of effects on goal intentions and self-efficacy; Study 2 examined accessibility of plan components and cue–response association.

**Relevant result:** implementation intentions had negligible effects on goal intentions and self-efficacy in Study 1; Study 2 found goal-attainment effects mediated by accessibility of specified situational cues and strength of the cue–response association.

**Supports:** the cue–response accessibility mechanism relevant to §55, within the studied implementation-intention paradigm.

**Does not support:** that increased deliberation explains the effect, that every cue–response plan works, or that the ROOT package is validated.

**Pinpointing status:** publisher abstract and study-level summary verified; exact page of Study 2's mediation analysis not independently verified in the accessible text.

### R33 — Zimmermann & Sobolev, 2023: randomized field experiment on digital friction

Laura Zimmermann and Michael Sobolev, “Digital Strategies for Screen Time Reduction: A Randomized Field Experiment,” *Cyberpsychology, Behavior, and Social Networking* 26(1), 42–49 (2023), DOI: [10.1089/cyber.2022.0027](https://doi.org/10.1089/cyber.2022.0027).

**Evidence type and design:** preregistered field experiment (N = 112) comparing grayscale design friction, self-commitment to time limits and self-monitoring control over several weeks; screen time was objectively measured.

**Relevant result:** grayscale produced an immediate significant reduction in objectively measured screen time relative to control; goal-setting produced a smaller, more gradual reduction. The study found no immediate causal effect of reduced use on subjective well-being or academic performance.

**Supports:** a particular design-friction intervention can reduce objectively measured smartphone screen time in the tested setting.

**Does not support:** general sustained-attention improvement, improved academic performance, lasting behaviour change, or a universal effect of obstruction.

**Pinpointing status:** PubMed abstract and article pages verified; exact table/figure for group contrasts not independently checked in the accessible text.

### R34 — Ochs & Sauer, 2022: smartphone obstruction field experiment

Carli Ochs and Juergen Sauer, “Curtailing smartphone use: a field experiment evaluating two interventions,” *Behaviour & Information Technology* 41(16), 3598–3616 (2022), DOI: [10.1080/0144929X.2021.2007284](https://doi.org/10.1080/0144929X.2021.2007284).

**Evidence type and design:** one-week field experiment with 97 student participants in app-relocation, grayscale and control conditions.

**Relevant result:** objective smartphone usage declined relative to the prior week, but the change also appeared in the control group; self-reported problematic smartphone use increased. The authors discuss heightened usage awareness as a possible explanation.

**Supports:** the need to distinguish objective behaviour from self-report and to account for measurement/awareness effects in obstruction studies.

**Does not support:** a clean causal effect of either intervention from the reported pre/post pattern, or general reduction in distraction.

**Pinpointing status:** publisher abstract and article pages verified; exact table/figure for condition contrasts not independently checked in the accessible text.

### R35 — Eppinger, Goschke & Musslick, 2021: meta-control

Ben Eppinger, Thomas Goschke and Sebastian Musslick, “Meta-control: From psychology to computational neuroscience,” *Cognitive, Affective, & Behavioral Neuroscience* 21, 447–452 (2021), DOI: [10.3758/s13415-021-00919-4](https://doi.org/10.3758/s13415-021-00919-4).

**Evidence type:** theoretical review/editorial synthesis, not a single empirical experiment.

**Relevant location:** abstract, pp. 447–448. Meta-control is described as mechanisms that monitor the progress of controlled processing and regulate underlying control parameters in service of task goals and internal/external constraints. The authors also state that meta-level control processes remain poorly understood.

**Supports:** a close established conceptual neighbour to §§46–47: monitoring controlled processing and changing control parameters.

**Does not support:** that all meta-control is solved, that the treatise's proposed mechanism is identical in every detail, or that Recursive Intelligence is impossible. It makes a distinctness claim require a sharper operational boundary.

### R36 — Fleming, 2024: metacognition and confidence

Stephen M. Fleming, “Metacognition and Confidence: A Review and Synthesis,” *Annual Review of Psychology* 75, 241–268 (2024), DOI: [10.1146/annurev-psych-022423-032425](https://doi.org/10.1146/annurev-psych-022423-032425).

**Evidence type:** theoretical/research synthesis.

**Relevant location:** abstract and review, pp. 241–268. The review distinguishes subpersonal uncertainty representations from personal-level beliefs about one's own performance, and describes propositional confidence in decisions/actions as depending on models of the world and the cognitive system that can be more or less accurate.

**Supports:** self-evaluation and confidence are established metacognitive constructs; self-model judgments can diverge from objective performance.

**Does not support:** a validated self-model for ROOT users or a distinct Recursive Intelligence mechanism.

### R37 — Fleming, 2026: integrative neuroscience of metacognition

Stephen M. Fleming, “Towards an integrative neuroscience of metacognition,” *Nature Reviews Neuroscience* 27, 789–806 (published 16 September 2026), DOI: [10.1038/s41583-026-01081-x](https://doi.org/10.1038/s41583-026-01081-x).

**Evidence type:** current review synthesizing behavioural, computational and neural evidence across rodents, non-human primates and humans.

**Relevant location:** abstract and review, pp. 789–806. It describes metacognition as self-evaluation of cognitive processes, with confidence estimates arising from transformations of uncertainty and supporting control at multiple timescales.

**Supports:** a broad established metacognitive framework that overlaps §§46–48 and their proposed monitoring/update cycle.

**Does not support:** the treatise's equations or a unique recursive mechanism. This is a review, not a new primary experiment.

### R38 — Brumby et al., 2013: interruption recovery and speed–accuracy trade-off

Duncan P. Brumby, Anna L. Cox, Jonathan Back and Sandy J. Gould, “Recovering from an interruption: investigating speed-accuracy trade-offs in task resumption behavior,” *Journal of Experimental Psychology: Applied* 19(2), 95–107 (2013), DOI: [10.1037/a0032696](https://doi.org/10.1037/a0032696).

**Evidence type and design:** two experiments using a routine sequential data-entry task interrupted by a cognitively demanding secondary mental-arithmetic task.

**Relevant result:** resumption lag was examined alongside error probability. A 10-second system lockout after the interrupting task reduced resumption errors, indicating that faster resumption is not always better when accuracy matters.

**Supports:** task recovery should be measured with both latency and resumed-task accuracy.

**Does not support:** a universal optimal return-to-task latency or the proposed ROOT composite.

**Pinpointing status:** PubMed abstract and article pages verified; exact experiment/table page references not independently checked in the accessible text.


### R39 — Bolenz et al., 2019: experimental meta-control of decision strategies

Florian Bolenz, Wouter Kool, Andrea M. F. Reiter and Ben Eppinger, “Metacontrol of decision-making strategies in human aging,” *eLife* 8:e49154 (2019), DOI: [10.7554/eLife.49154](https://doi.org/10.7554/eLife.49154).

**Evidence type and design:** cross-sectional human experiment with 62 younger adults (18–30 years; mean age 22.7) and 62 older adults (57–80 years; mean age 70.2). Participants completed a sequential decision task designed to dissociate model-free from model-based strategies. The task manipulated reward stakes and transition-structure stability to vary the relative benefit and computational demand of model-based control. The experiment used 320 trials per participant across four 80-trial blocks.

**Relevant locations:** article Introduction for the definition and rationale of meta-control; Methods for the sequential task, stakes and transition-stability manipulations; Results and Discussion for age-group differences and adaptation. Figure 1A–C describes the task/condition structure; Figure 2A–B reports reward and model-based-control results. Supplementary Tables S5–S21 contain full group-level regression coefficients.

**Relevant result:** the authors found reduced model-based decision making and less adaptation of decision strategies in older adults. The design directly tests dynamic adjustment of decision strategy to changing reward and task-structure demands.

**Supports:** human decision systems can adapt the balance between established strategies as task costs, benefits and structure change; meta-control is an experimentally operationalized neighbour to the proposed §§46–47 mechanism.

**Does not support:** a unique Recursive Intelligence architecture, an explicit self-model of the learning/controller process, a meta-meta update, or ROOT efficacy. The cross-sectional age comparison and specific sequential task limit generalization.

**Pinpointing status:** primary full-text article and figure descriptions inspected; exact quantitative estimates are in the supplementary Tables S5–S21. The source establishes a concrete comparator, not identity between the study's model and the treatise's proposal.



## 16. Claim-level register: Sections 60–74

**Baseline:** \`document_master_visual.md\`, branch \`edition\`, blob \`123abdbe9ad3e6c24d150e7db2f38e9562d520d5\`; §§60–74 occupy baseline lines 1853–2199. The prior claim inventory is commit \`821b4e8b8606f745f2531489936997b236a25c65c\`. This pass reuses the M14–M18 formal audit (commit \`2ad7a85cc0353f72acfdc6fc627bb2bbcbba1af0\`), the tracker audit (\`2d592cd9d7f2d66f5531a5cb72e303197414aabc\)), the prior alternatives audit (\`9098cf5acc7390d2d42410aac48706589b227b84\)) and the existing formal-result premise map. It does not repeat those audits or execute any experiment.

The five dimensions remain separate: claim kind, formal validity, empirical/evidential support, disposition and unresolved dependency. “Conditional” and “not established” are not synonyms for false.

| ID | Claim / exact treatise location | Claim kind | Formal validity | Empirical / evidential support | Disposition | Unresolved dependency |
|---|---|---|---|---|---|---|
| S60-M01 / S60-C01 | Closed-loop behavioural model \(x_{t+1}=(A-BK)x_t+w_t\); stability when eigenvalues lie inside unit circle (L1853–1885) | Linear dynamical model; mathematical condition; human-behaviour analogy | For the homogeneous discrete-time LTI system \(x_{t+1}=A_{\rm cl}x_t\), asymptotic/exponential stability is equivalent to \(A_{\rm cl}\) being Schur (all eigenvalues strictly inside unit disk). This does not establish stability of a human system. With persistent nonzero \(w_t\), convergence to zero generally does not follow; a Schur matrix instead gives bounded response to bounded disturbances under the stated linear model. | Standard control-theory result (R40). No identified human behavioural \(A,B,K\), state, sampling interval or disturbance process is supplied. | Retain as a pedagogical linear approximation; restrict the eigenvalue condition to the disturbance-free homogeneous model. Qualify disturbance-affected claims as boundedness/robustness questions. | Define state and target, sampling interval, identified transition matrices, intervention input, observability, controllability, model error, disturbance bounds/distribution and whether the claim is asymptotic, input-to-state, mean-square or practical stability. |
| S61-M01 / S61-EQ01 | Lyapunov-style \(V(x)\) as weighted sum of squared goal deviation, unwanted habit activation and return latency; expected \(V\) should decrease (L1886–1908) | Candidate Lyapunov function; measurement convention | A weighted sum of squares is positive definite only relative to a defined zero state and strictly positive weights; it is radially unbounded only under suitable state-domain assumptions. Variables require scale normalization and commensurate operational meaning. \(\Delta V<0\) is a stability certificate only with the requisite domain, positivity, invariance and decrease conditions. “Expected decrease” is a different stochastic claim from pathwise decrease. | No validation of this \(V\), its weights or its component measurements is supplied. The prior tracker audit already classifies its stability proxy as an unvalidated personal measurement convention (R40 cross-reference; tracker audit commit above). | Retain as a candidate proxy, not a verified Lyapunov function or proof of behavioural stability. | Define \(x\), equilibrium/acceptable set, units and normalization, \(P\succ0\) or equivalent positive-definiteness conditions, domain, disturbance model, sampling and whether the criterion is deterministic, expected or probabilistic. |
| S62-P05 / S62-C01 | Proposition 5: repeated effective feedback reduces expected frequency or duration of unwanted responses under five assumptions (L1909–1926) | Conditional proposition; causal/dynamical hypothesis | The verbal argument is not a proof. “Successful cycle changes the state in a favourable direction” does not entail negative drift, and “expected effect exceeds disturbances” is not quantified. A sufficient deterministic route would specify \(V\succ0\), a forward-invariant domain and \(\Delta V(x)\leq-W(x)\) for positive-definite \(W\). A stochastic version needs a conditional drift inequality and additional state-process/boundedness assumptions. | No experiment establishes the proposition for ROOT or human behaviour. Standard Lyapunov theory supplies conditional mathematical tools, not empirical premises for this system (R40). | Keep explicitly conditional; do not call the current argument a stability proof. The prior formal premise map remains the governing audit. | State a precise theorem with quantified assumptions, state/action process, disturbance set, update law, drift bound, domain, conclusion type and counterexamples; separately test whether empirical premises hold. |
| S63-C01 | No universal guarantee is mathematically justified under unrestricted disturbances and biological/environmental conditions (L1927–1946) | General impossibility argument; scope limitation | The intuition can be formalized only under restrictions. For example, a scalar plant with bounded control \(|u_t|\leq U\) and an unrestricted persistent disturbance \(w_t>U\) can be driven away despite any admissible controller. The current text does not define “finite controller,” actuator bounds or disturbance class, so the blanket statement is under-specified rather than proved. | No empirical study is needed for the conditional counterexample; it is a mathematical model illustration. It does not establish a universal theorem about all human or finite controllers. | Retain the practical caution, but present impossibility as conditional on specified actuation and disturbance constraints. | Define controller class, feasible control authority, disturbance set, state constraints and performance criterion; distinguish infeasibility from uncertain efficacy or biological limits. |
| S64-C01 / S64-EQ01 | Self-mastery does not require zero urge; goal-action probability conditional on positive urge should remain meaningfully high (L1947–1970) | Normative/operational definition; probabilistic criterion | \(P(A=a_g\mid U>0)\) is a valid conditional probability but is not sufficient without context, opportunity, action feasibility, competing goals and a threshold. The event \(U>0\) also collapses urge intensity and context. | No source validates this as a general measure of self-mastery. It is a proposed operationalization and should not pathologize normal urges. | Retain as a useful conceptual distinction between urge presence and action selection; do not treat it as a validated outcome metric. | Define eligible opportunities, appropriate goal action, urge measurement, context stratification, baseline and clinically/non-clinically meaningful thresholds; account for cases where not acting on an urge is not the appropriate goal. |
| S65-C01 | Separate phone, gaming, television, sleep, sexual distraction and study-avoidance behaviours rather than assume one diagnosis/mechanism (L1971–1990) | Methodological safeguard; hypothesis taxonomy | The table lists candidate mechanisms and measures; it does not infer causes or diagnose. The categories may overlap and the listed single metrics do not capture all relevant contexts or impairment. | The separation is consistent with measurement and diagnostic caution, but no study validates this exact table as a complete taxonomy. EMA/self-report agreement varies substantially across behaviours and individuals (R42). | Retain as a non-diagnostic hypothesis map; explicitly mark each proposed mechanism as to-be-tested. | Define operational target behaviour and opportunity denominator per domain; distinguish direct observation, self-report and inferred motive; assess burden, context, co-occurrence and missingness. |
| S66-C01 | Sexual attraction/urges and masturbation are not inherently pathological; CSBD requires persistent impaired control and marked distress/functional impairment, not moral disapproval alone (L1991–2006) | Clinical boundary statement; diagnostic-scope qualification | The section's non-pathologizing distinction is consistent with ICD-11 diagnostic requirements. Frequency, libido or masturbation alone do not satisfy the diagnostic construct. Diagnosis requires the full clinical criteria and differential assessment; this text is not a diagnostic instrument. | WHO's ICD-11 CDDR is the authoritative diagnostic manual (R45); WFSBP guidance reproduces the essential features and duration/impairment criteria (R46). These support the boundary, not individual diagnosis. | Retain with explicit non-diagnostic framing; avoid equating normal desire or moral conflict with disorder. | Verify final wording against the current WHO CDDR and distinguish screening, clinical diagnosis, moral incongruence and functional impairment. Keep referral language proportionate and non-stigmatizing. |
| S67-C01 | Sleep timing/quality affects the operating conditions for attention and executive control; two-week log and referral for persistent impairment (L2007–2020) | Empirical domain claim; monitoring recommendation; clinical safeguard | Sleep as a state variable is plausible, but a personal sleep log is not a diagnostic test and temporal association does not establish that sleep caused an individual's attention difficulty. | A meta-analysis of 61 studies/71 populations found sleep restriction impaired sustained attention on average (g = −0.409), with moderators including age, time of day and cumulative restriction (R43). A later 44-study meta-analysis found one-night restriction increased sleepiness and impaired sustained attention (reaction time SMD = 0.512; lapses SMD = 0.489) (R44). Effects are task- and exposure-specific. | Retain sleep as a relevant potential moderator; keep the two-week log as descriptive monitoring, not diagnosis or causal proof. | Specify sleep exposure, duration/regularity/quality, objective versus subjective measurement, naps, circadian timing, medication/health confounds and functional impairment. Do not infer sleep disorder from a tracker. |
| S68-C01 | Breaking an ambiguous study task into a concrete first action reduces initiation cost and uncertainty (L2021–2038) | Intervention heuristic; causal hypothesis | The cost/uncertainty interpretation is a model hypothesis, not an algebraic result. A concrete next step may reduce task ambiguity but need not improve initiation in every context; no effect size or selector is specified. | If–then planning and cue-response specification have relevant evidence (R31–R32 in the prior batch), but those sources do not directly validate this exact study-initiation prescription or the cost terms \(K,D\). | Retain as a low-risk, testable design heuristic; avoid presenting it as a demonstrated universal mechanism. | Define initiation latency, eligible study opportunities, task type/difficulty, adherence, comparator and functional output; test whether reduced ambiguity mediates any improvement. |
| S69-C01 / S69-PROT01 | Personal protocol: 7-day baseline, 7-day environmental change, 14-day alternative-response training, then weekly review (L2039–2095) | Personal self-monitoring protocol; sequential intervention proposal | The three initial phases total 28 days. This is not by itself a randomized N-of-1 trial or a replicated single-case experiment: phase order is fixed, environmental change and response training are sequential, and no withdrawal, randomized phase start, counterbalancing or replication is specified. Phase changes are confounded with time and carryover. | Methodological reviews recommend repeated objective outcomes, pre-specified analysis and randomization/counterbalancing where feasible; reversible interventions and washout matter for N-of-1 crossover designs (R41). Single-case experiments require systematic manipulation and repeated measurement across phases; a one-phase pre/post routine is not sufficient causal demonstration (R47). | Retain as a personal planning template, not an efficacy trial or validated dose. It can document feasibility and personal utility descriptively. | Reconcile the 28-day design with the tracker's 14-day pilot; define primary functional outcome, opportunity denominators, measurement frequency, baseline trend, concurrent changes, missing data, burden/adverse effects and a feasible comparator/design. Do not experiment on clinical or safety-critical behaviours without appropriate support. |
| S70-C01 | Four foundations assigned complementary functions in one architecture (L2096–2106) | Framework definition; integration hypothesis | The table assigns roles but does not define typed interfaces or show that the components are necessary, sufficient or mutually compatible. A taxonomy of functions is not evidence of an integrated mechanism. | Existing research supports neighbouring domains separately; no package-level or architecture-level validation demonstrates this four-part integration. The earlier alternatives and interface audits remain applicable. | Retain as a proposed organizing architecture; do not present component complementarity as empirically established. | Define each component's unique input/output, shared constructs, dependency direction, timescale, provenance and falsifiable incremental contribution over simpler combinations. |
| S71-EQ01 / S71-EQ02 / S71-C01 | Unified state transition \(\mathcal S_{t+1}=\mathcal F(\mathcal S_t,O_t,\mathcal I_t,G_t,R_t,\mathcal R_t)\); \(\mathcal F\) decomposed as composition of four operators (L2107–2150) | Schematic state-transition model; operator composition | The equation is syntactically meaningful only after state/input spaces and operator domains/codomains are defined. Under standard right-to-left function composition, \(\mathcal F_{\rm context}\circ\mathcal F_{\rm inference}\circ\mathcal F_{\rm control}\circ\mathcal F_{\rm learning}\) applies learning first; this may not match the prose's intended sequence. If operations are concurrent/coupled, ordinary serial composition is not an adequate specification. \(R_t\) is ambiguous between reward and feedback; \(\mathcal R_t\) is resources. | No source validates this unified transition function or its decomposition. It is a modelling proposal. | Retain as an architectural placeholder; do not treat it as a defined executable model. | Define typed state/input/output spaces, operator signatures, composition convention/order or concurrent update semantics, clock/aggregation, state observability, uncertainty, missingness, resource constraints and non-circular validation. |
| S72-C01 | Nine-stage unified Context–Inference–Control cycle (L2151–2164) | Conceptual process model | The list supplies an intuitive sequence but no formal transition relation, stage contracts, concurrency rules or conditions for termination/re-entry. It overlaps the ROOT cycle and prior context/inference definitions. | No empirical or comparative evidence validates this exact nine-stage sequence or shows it outperforms simpler pipelines. | Retain as a conceptual overview; label sequence as proposed rather than established. | Map each stage to the typed interfaces required by §71 and the four foundation roles in §70; identify duplicated stages, feedback timing and testable incremental predictions. |
| S73-TH04 / S73-C01 | Contextual and generative intelligence are complementary if context includes external observations and internal structure (L2165–2179) | Conditional formal compatibility result; conceptual synthesis | The argument establishes compatibility only under its stipulated broad definition \(C=(O,M,A,K)\) and a sound inference relation. \(O=0\) means no new external observation during the inference interval, not absence of memory, architecture, prior data or constraints. If \(K\models p\), a sound derivation can establish \(p\) from \(K\); it does not establish that \(K\) is true of the actual world unless the premises are true. The result is conditional and close to definitional; it does not establish novelty. | This is a logical result under formal semantics, not an empirical finding. The prior entailment audit remains controlling; no empirical source can substitute for checking the proof assumptions. | Retain as a conditional compatibility proposition/theorem only with the formal scope explicit. Do not claim empirical validation or a new inference mechanism. | State the language, semantics, proof relation and soundness assumptions; distinguish formal entailment, derivability, actual-world truth and probabilistic support; explain what nontrivial claim remains beyond the definition of context. |
| S74-TH05 / S74-C01 | Self-mastery as feedback-driven policy modification under constraints; goal-action probability rises when relative selection score rises (L2180–2199) | Conditional mathematical proposition; framework synthesis | The derivation's step 5 requires a specified choice rule. Under two-action softmax with fixed \(\beta>0\), \(P(a_g)=1/[1+\exp(-\beta(Q_g-Q_h))]\), so increasing \(\Delta Q=Q_g-Q_h\) strictly increases \(P(a_g)\). This implication is not true for every unspecified selector or with changing feasible actions/other scores. Step 6 requires an explicit learning rule with monotone reinforcement; it does not follow from repeated success alone. | No empirical evidence establishes that the proposed ROOT interventions produce the required score change or that the unified architecture describes a person's cognition. | Retain as a conditional result after adding the selector and learning premises; otherwise classify as a model proposition, not a demonstrated universal theorem. | Specify action set, score scales, choice rule, inverse temperature, feasible constraints, policy update, reinforcement conditions, timescales and empirical validation. Separate the mathematical conditional from the human-mechanism hypothesis. |

### Cross-section dependencies and integration findings — §§60–74

1. **Stability chain (§§60–62):** §60 supplies a linear closed-loop template; §61 proposes a candidate scalar measure; §62 attempts to infer improvement. These are three different levels: model structure, candidate certificate and theorem. The current text moves from one to the next without identifying \(A,B,K\), a valid \(V\), a forward-invariant domain or a quantified decrease/drift condition. M14–M18 remain open; this batch does not close them.
2. **Disturbance semantics (§§60–63):** the homogeneous Schur condition establishes convergence only for the unforced model. Persistent disturbances require bounded-input/stochastic/practical-stability analysis. The universal-guarantee argument should be expressed as a conditional impossibility under bounded actuation and unrestricted disturbances, not as an unqualified theorem about every finite controller.
3. **Behavioural construct and measurement (§§64–68):** the probability criterion, behaviour table, sleep log and task-initiation prescription are operational proposals. Their measures require opportunity denominators, context and independent functional outcomes; self-report alone is not a validated latent-state estimator.
4. **Personal protocol (§69):** the treatise's initial phases total 28 days; the tracker recommends a 14-day cycle. The former is a sequential 7+7+14 proposal, not a replicated causal design. The two artifacts must not be silently treated as the same protocol.
5. **Unified architecture (§§70–72):** the four foundation roles, state equation and nine-stage cycle are conceptual integration. The operator composition's right-to-left order is potentially inconsistent with the intended process narrative; typed interfaces and clocks are absent.
6. **Formal conclusions (§§73–74):** Theorem 4 is conditional compatibility under a broad context definition; Theorem 5 is conditional on a choice rule and learning update. Neither proves a novel mechanism or validates the human-level architecture.
7. **No package-level validation:** none of the sources in this batch establishes the complete four-foundation architecture, the proposed stability controller, the personal protocol's efficacy, or a unique self-mastery mechanism.

### Consolidated findings for §§60–74

- The discrete-time Schur stability criterion and Lyapunov methods are established mathematics. Their application to human behaviour remains a model proposal until the system, state, inputs, disturbances and measurements are identified.
- The candidate \(V(x)\) is not yet a Lyapunov certificate. Proposition 5's current verbal argument does not supply the drift inequality needed for a stability conclusion.
- A universal impossibility claim requires a specified controller class and disturbance/actuation bounds. A valid restricted counterexample is available; the current prose is broader than its formal premises.
- The personal protocol is a 28-day sequential self-management template, not a causal N-of-1 experiment. The 14-day tracker design remains distinct.
- The sleep and clinical sections have relevant authoritative evidence, but logs and self-observation do not diagnose or establish causation.
- The unified four-part architecture is a proposed synthesis. The operator composition, stage contracts and cross-timescale interfaces are not yet formally defined.
- Theorem 4 is conditional compatibility, not novelty. Theorem 5 can be made mathematically valid under an explicit monotone selector and learning rule, but the empirical premises remain untested.
- No experiment was executed; all experimental authorization and prerequisite gates remain unchanged.

**Status:** §§60–74 have a first claim-level mathematical, evidential and disposition pass. The prior formal audits were reused, not declared complete. Primary-source pinpointing is provided where checked; exact full-text locations remain unavailable or unverified for some review sources. M14–M18, the canonical glossary, complete taxonomy crosswalk, final claim dispositions, full 95-section integration and all experimental gates remain open. No treatise or tracker edits are made by this register entry.

## 17. Additional source register: Sections 60–74

### R40 — Megretski, 2004: discrete-time linear stability and Lyapunov certificate

Alexandre Megretski, “Model Reduction by Projection: General Properties,” MIT 6.242 lecture notes, Fall 2004, version 19 September 2004.

**Evidence type:** authoritative mathematical lecture notes, not an empirical study.

**Relevant location:** §4.2.2, “Stability preservation,” pp. 12–13 (PDF pages 12–13; discrete-time model equation (4.6), Lyapunov inequality and Theorem 4.6). The notes state that a minimal discrete-time LTI model is stable iff its state matrix is Schur and give a positive-definite \(P\) certificate \(P-A^\top PA\succ0\). Theorem 4.6 concerns a projection-reduced model and supplies sufficient conditions for its stability.

**Supports:** the standard Schur criterion and discrete-time Lyapunov-certificate framework used to qualify §§60–62.

**Does not support:** existence of an identified human behavioural state-space model, the treatise's candidate \(V\), or empirical ROOT efficacy.

**Pinpointing status:** PDF inspected; exact theorem and inequality locations identified as §4.2.2, Theorem 4.6, pp. 12–13. This is a teaching source for standard mathematics; a later formal audit should cite a canonical control text if a definitive bibliographic foundation is required.

### R41 — “N-of-1 Randomized Intervention Trials in Health Psychology,” 2018

“N-of-1 Randomized Intervention Trials in Health Psychology: A Systematic Review and Methodology Critique,” *Annals of Behavioral Medicine* 52(9), 731–742 (2018), DOI: [10.1093/abm/kax026](https://doi.org/10.1093/abm/kax026).

**Evidence type and scope:** systematic review of 54 N-of-1 trial publications involving 1,193 participants. Only 36% reported enough information to calculate heterogeneity of treatment effect; 90% provided some quantitative information to compare treatments.

**Relevant methodological locations:** article Methods and “Recommendations to Improve the Quality of N-of-1 Designs With Psychological and Health Behavior Outcomes,” including Table 1. The review specifies repeated measurable outcomes, reversible interventions, estimated washout, a credible comparator, a priori measurement/analysis and randomization or counterbalancing where feasible.

**Supports:** requirements and limitations relevant to interpreting or redesigning the sequential personal protocol in §69.

**Does not support:** that a simple baseline/intervention diary establishes causality, or that a 28-day duration is universally adequate.

**Pinpointing status:** article pages 731–742 and Table 1 identified; exact individual recommendation page not independently checked in the accessible text.

### R42 — Ecological Momentary Assessment validity review, 2022

“Ecological Momentary Assessment: A Systematic Review of Validity Research,” *Behavior Analysis in Practice* (2022), DOI: [10.1007/s40614-022-00339-w](https://doi.org/10.1007/s40614-022-00339-w).

**Evidence type and scope:** systematic review of 32 studies comparing mobile EMA reports with more objective measures of health behaviour or environmental events.

**Relevant result:** correspondence varied widely across individuals, behaviours and studies; reported agreement rates ranged from 1.8% to 100%. The review concluded EMA can be accurate but found no single set of factors that consistently explained high correspondence.

**Supports:** repeated self-report can be useful for ecological measurement, but accuracy is construct-, person- and context-dependent and requires validation where possible.

**Does not support:** treating a subjective 0–5 rating or retrospective episode log as an objective measure of latent state.

**Pinpointing status:** abstract and review scope/results verified; exact table-level study breakdown not independently checked.

### R43 — Lowe, Safati & Hall, 2017: sleep restriction and neurocognition

C. J. Lowe, A. Safati and P. A. Hall, “The neurocognitive consequences of sleep restriction: A meta-analytic review,” *Sleep Medicine Reviews* 36, 48–57 (2017), DOI: [10.1016/j.smrv.2017.01.002](https://doi.org/10.1016/j.smrv.2017.01.002).

**Evidence type and scope:** meta-analysis of 61 studies across 71 populations examining short-term sleep restriction and neurocognitive outcomes.

**Relevant result:** pooled negative effect on cognitive processing (g = −0.383); sustained attention showed a negative effect (g = −0.409). Age, time of day, cumulative restriction, sleep latency and subjective sleepiness moderated effects.

**Supports:** sleep restriction can impair sustained attention on average and should be considered as a relevant state/context variable.

**Does not support:** that sleep explains any particular individual's study difficulty, that sleep logs diagnose a disorder, or that the ROOT model's fatigue coefficient is known.

**Pinpointing status:** PubMed abstract and bibliographic record verified; exact forest-plot/table location not independently checked.

### R44 — “Impact of one night of sleep restriction on sleepiness and cognitive function,” 2024

“Impact of one night of sleep restriction on sleepiness and cognitive function: A systematic review and meta-analysis,” *Sleep Medicine Reviews* (2024), DOI: [10.1016/j.smrv.2024.101940](https://doi.org/10.1016/j.smrv.2024.101940).

**Evidence type and scope:** systematic review/meta-analysis of 44 studies assessing one night with 2–6 hours of sleep opportunity.

**Relevant result:** subjective sleepiness increased (SMD = 0.986); sustained-attention reaction times worsened (SMD = 0.512) and attentional lapses increased (SMD = 0.489).

**Supports:** even one restricted night can affect sleepiness and sustained-attention task performance on average.

**Does not support:** a chronic individual diagnosis or a universal prediction for every task/person.

**Pinpointing status:** PubMed abstract verified; exact analysis table/figure not independently checked.

### R45 — World Health Organization, 2024: ICD-11 clinical descriptions and diagnostic requirements

World Health Organization, *Clinical Descriptions and Diagnostic Requirements for ICD-11 Mental, Behavioural and Neurodevelopmental Disorders* (CDDR), published 8 March 2024.

**Evidence type:** authoritative diagnostic manual.

**Relevant location:** ICD-11 category 6C72, Compulsive Sexual Behaviour Disorder. The criteria require a persistent pattern of failure to control intense, repetitive sexual impulses/urges resulting in repetitive sexual behaviour, manifested over an extended period (e.g. six months or more), with marked distress or significant impairment. Distress entirely related to moral judgments/disapproval is insufficient.

**Supports:** §66's non-pathologizing boundary and the distinction between normal sexual interest/behaviour and a clinically significant persistent impaired-control pattern.

**Does not support:** self-diagnosis from frequency, attraction or masturbation; this section is not a diagnostic assessment.

**Pinpointing status:** WHO CDDR publication and category 6C72 identified; the manual's complete category text was not independently page-pinned in this pass. The WFSBP guideline below reproduces the essential features.

### R46 — WFSBP guidelines for compulsive sexual behaviour disorder, 2023

“World Federation of Societies of Biological Psychiatry guidelines on the assessment and pharmacological treatment of compulsive sexual behaviour disorder,” *World Journal of Biological Psychiatry* (2023), DOI: [10.1080/19585969.2022.2134732](https://doi.org/10.1080/19585969.2022.2134732).

**Evidence type:** clinical guideline and evidence synthesis.

**Relevant location:** Table 1, ICD-11 diagnostic criteria for CSBD. It lists persistent failure to control intense/repetitive sexual impulses or urges, one or more manifestations of impaired control, an extended duration (e.g. six months or more), and marked distress/significant impairment. It explicitly excludes distress entirely attributable to moral judgments/disapproval as sufficient.

**Supports:** the diagnostic boundary summarized in §66.

**Does not support:** diagnosing an individual from a tracker, self-label or frequency count.

**Pinpointing status:** Table 1 inspected in the accessible full-text record; recommendations for assessment and differential diagnosis should be checked before any clinical use.

### R47 — Single-case experimental design and reporting standards

Tate et al., “The Single-Case Reporting Guideline In BEhavioural Interventions (SCRIBE) 2016 Statement,” *Archives of Scientific Psychology* 4 (2016), DOI: [10.1037/arc0000026](https://doi.org/10.1037/arc0000026).

**Evidence type:** methodological reporting guideline.

**Relevant location:** definition and scope of single-case experimental designs in the statement. It describes prospective, intensive individual study with systematic manipulation across discrete phases and repeated measurement throughout; a simple one-phase training study or pre/post report without repeated phase measurement is not a single-case experiment.

**Supports:** the distinction between §69's personal tracking protocol and a controlled single-case experimental design.

**Does not support:** that any particular design will be feasible, ethical or valid for every behaviour.

**Pinpointing status:** statement and design definition verified; item-level checklist is available in the full SCRIBE materials and should be applied if a study protocol is later authorized.



## 18. Claim-level register: Sections 75–89

**Baseline:** document_master_visual.md, blob 123abdbe9ad3e6c24d150e7db2f38e9562d520d5; numbered-section locations below refer to that unchanged baseline.

| ID | Claim / source location | Formal status and evidence assessment | Disposition and open dependency |
|---|---|---|---|
| S75-C01 | A–F are designed to separate framework components rather than merely show that a productivity routine helps (L2201–2207) | This is a methodological intention, not a demonstrated property of the designs. A tests formal derivation; B tests prospective model prediction; C–E test behavioural/resource mechanisms; F tests adaptive control. These are not, as currently specified, discriminating tests of the four named theories or their integration. Several outcomes are already expected under established inference, implementation-intention and adaptive-control accounts. | Retain the intention, but qualify the current designs as component-level tests. Before claiming framework-level discrimination, state a theory-specific prediction that differs from credible alternatives and a result that would favour one account over another. |
| S76-EXP-A | Experiment A: derive withheld conclusions from supplied rules and facts without new external observation (L2209–2224) | A valid proof certificate establishes derivability from supplied premises and rules. It does not establish information from nothing, an arbitrary unobserved contingent fact, or the truth of the premises. A benchmark can be trivial or contaminated unless derivation depth, complexity, negative/underdetermined cases, resource budgets and held-out generation are controlled. The governing plan's proof checker, countermodel, baseline, contamination and sampling provisions materially strengthen it. | Retain as a formal-inference benchmark, not a test of the full Out of Box Theory. Complete system/language/generator/resource/sample gates; report proof validity, coverage and false positives separately. Do not execute before the plan's gate is met. |
| S77-EXP-B | Experiment B: predict a physical outcome before direct observation (L2226–2240) | Prospective, timestamped prediction against suitable baselines and alternatives is a valid general test of predictive performance. The treatise specifies no physical domain, outcome, apparatus, model or scoring rule. One successful prediction is weak evidence without calibration, uncertainty, held-out data and comparison. A generic successful prediction would not establish a unique contribution of Out of Box Theory. | Retain as a protocol architecture only. It is not executable until the domain-lock gate is met. Require a risky, quantitative, registered prediction and a comparator capable of distinguishing the proposed model from established alternatives. |
| S78-EXP-C | Experiment C: effort, fatigue and task uncertainty may change habitual-distraction selection (L2242–2256) | The prediction is plausible and appropriately qualified as individual/context dependent. Naturally varying fatigue, task difficulty and cue exposure are confounded; observational repeated measures can estimate within-person association but do not identify fatigue's causal effect. The treatise correctly disclaims a direct entropy-to-distraction inference. The plan improves the design with eligible-opportunity denominators and separates observational from randomized task manipulations. | Retain as a resource-sensitive action-selection hypothesis. Define the target action, opportunity, instruments and repeated-measures model. Do not claim causal fatigue effects or thermodynamic mechanisms from observational logs. |
| S79-EXP-D | Experiment D: obstruction of cue accessibility may reduce unwanted actions (L2258–2270) | A plausible local intervention hypothesis. A single baseline/intervention comparison is vulnerable to time trend, regression to the mean, concurrent changes, substitution and reactivity. Raw frequency without eligible cue/opportunity exposure can mislead. The governing plan's randomized/counterbalanced blocks, replicated phases or staggered multiple baseline, fidelity and burden measures are more defensible. | Retain as a context-specific accessibility test. The plan's target-loop, barrier, denominator, design and threshold gates remain open. A successful local barrier does not establish universal behavioural control or ROOT package efficacy. |
| S80-EXP-E | Experiment E: trigger-specific alternative-response training may improve recovery (L2272–2284) | If–then implementation intentions are an established intervention family; a 2024 meta-analysis of 642 independent tests reports effects across cognitive, affective and behavioural outcomes, with stronger effects for contingent plans, goal commitment and rehearsal (R48). Therefore, a positive result would support the particular plan in its context, not novelty or unique validation of ROOT. Cue detection, opportunity denominator, rehearsal fidelity, comparator and obstruction co-intervention must be separated. | Retain as a test of a known behavioural technique within the proposed protocol. Use an active comparator and hold obstruction constant or factorialize it; do not infer that the named ROOT architecture is uniquely responsible. |
| S81-EXP-F | Experiment F: weekly model revision may outperform a fixed routine (L2286–2298) | A comparison of adaptive and fixed policies tests adaptive-control utility only if both policies, objectives, resources, constraints and decision opportunities are specified and fairly matched. Ordinary feedback-based adaptation is not by itself evidence of a distinct meta-cognitive or Recursive Intelligence mechanism. The governing plan correctly requires a meta-level representation and update criterion, frozen policies, held-out evaluation, functional outcomes and safety overrides. | Retain as a conditional adaptive-controller hypothesis. Do not label it a Recursive Intelligence test until the meta-level operation is operationally distinguished from ordinary state estimation/policy adaptation. Select design by adaptation timescale; SMART and micro-randomized designs answer different questions (R49). |
| S82-M01 | General measurement and statistical safeguards for A–F (L2300–2318) | The treatise's short list is sound but incomplete as an executable protocol: it does not itself specify estimands, sampling, comparator, fidelity, dependence, missingness, analysis, uncertainty, stopping, preregistration or ethics. These are supplied in the governing plan's common contract and protocol-specific sections. The plan, not §82 alone, is the current operational standard. | Retain as a summary. Keep the detailed common contract authoritative; ensure every later protocol satisfies it and records deviations, adverse outcomes and all registered tests. |
| S83-L01 | Explicit limits: no proof of universal intelligence, entropy identity, arbitrary deduction, universal willpower or guaranteed ROOT cure (L2320–2333) | Appropriate scope disclaimers. They prevent several category errors but do not establish that the remaining framework is correct, exhaustive or empirically supported. Some statements are absence-of-proof boundaries rather than proofs of impossibility. | Retain. Preserve the distinction between “not established by this treatise” and “shown to be impossible.” |
| S84-FM01 | Coherence can coexist with empirical falsity; independent risky predictions are a safeguard (L2335–2339) | Sound general philosophy-of-science principle. It is not a new result or evidence that the proposed experiments are sufficiently discriminating. | Retain as a methodological safeguard; connect each empirical claim to an actual falsifier and suitable competing model. |
| S85-FM01 | Novelty is not equivalent to discovery or evidential support (L2341–2345) | Conceptually correct distinction. Novelty is relative to a knowledge state or representation; discovery additionally requires a defensible relation to a target and evidence/derivation. The listed epistemic labels need consistent application across the treatise. | Retain; cross-reference the governing epistemic taxonomy and require claim-level classification rather than treating novelty as confirmation. |
| S86-FM01 | Energy cost alone is not a complete explanation of behaviour (L2347–2351) | Correctly rejects reduction of behaviour to a single resource variable. The statement is consistent with the treatise's own acknowledgement that learning, task structure, goals, physiology and environment matter. It does not validate the proposed physical–cognitive bridge. | Retain; require independent evidence for each proposed bridge from physical constraints to a specific behavioural prediction. |
| S87-FM01 | Overengineering self-control can create unsustainable burden; prefer the smallest useful intervention (L2353–2357) | Reasonable design heuristic, not a universal empirical law. “Measurable benefit” needs a functional endpoint and a burden/harms measure; intervention simplicity alone is not sufficient. | Retain as a heuristic; operationalize benefit, burden, adverse effects and stopping/reassessment criteria in ROOT materials. |
| S88-FM01 | Clinical problems should not be treated solely as failures of discipline (L2359–2363) | Appropriate safety boundary and consistent with the earlier non-diagnostic framing. The list of conditions is illustrative, not a differential diagnosis or claim that any listed condition is present. | Retain. Keep ROOT explicitly non-clinical and avoid diagnostic inference; professional assessment remains appropriate where impairment/distress warrants it. |
| S89-FM01 | Recursive Intelligence should periodically review the goal hierarchy, not merely optimize a possibly harmful or obsolete goal (L2365–2369) | Important normative/controller-design principle. The treatise does not define who has authority to set or revise goals, how conflicts among goals are resolved, or what criteria distinguish harmful, outdated, externally imposed and merely difficult goals. Optimization metrics can also become targets that are gamed or detached from the underlying objective. | Retain as a requirement, not a solved mechanism. Specify goal provenance, user authority, constraints, conflict resolution, review triggers and safeguards before presenting it as an operational property of Recursive Intelligence. |

### Cross-section dependencies and integration findings — §§75–89

1. **Experiment-to-theory coverage (§§75–82):** A–F form a sensible portfolio of formal-inference, prospective-prediction, resource-sensitive behaviour, environmental intervention, alternative-response training and adaptive-control questions. They do not yet test the four-foundation synthesis as a whole. No single experiment operationalizes all four components, and the current set does not contain a registered prediction unique to the integrated architecture.
2. **A versus B:** A tests derivability from supplied formal constraints; B tests whether a frozen model predicts a physical outcome before measurement. These are distinct epistemic achievements. A valid derivation does not establish the premises' truth; a successful prediction does not show that the prediction was generated without encoded structural information.
3. **C–E versus established mechanisms:** Resource-sensitive action selection, cue accessibility and if–then response training have close analogues in established behavioural and cognitive-control research. A positive result would support a local mechanism or intervention, not establish theoretical originality. E especially needs a comparison with implementation-intention evidence (R48).
4. **F versus Recursive Intelligence:** Adaptive control and meta-cognitive self-modification are not synonymous. The plan's meta-level distinction is essential. A fair fixed-policy comparator, a frozen update algorithm and held-out evaluation are necessary to avoid testing a deliberately weak baseline or rewarding retrospective manual tuning. The choice between slower sequential randomization (SMART) and faster micro-randomization (MRT) depends on the decision timescale and estimand (R49).
5. **Protocol hierarchy:** §82 is a high-level safeguard summary. The more complete Section 9.1 common contract and 9.2–9.8 protocol/readiness gates in EDITION_PLAN.md are the operational specification. Neither a written protocol nor preregistration is execution or empirical validation.
6. **Limits and failure modes (§§83–89):** the disclaimers are generally directionally sound. §89 identifies a genuine governance problem, but a review of goals requires explicit normative authority, provenance, conflict resolution and safety constraints; these cannot be inferred from predictive accuracy or control efficiency.
7. **No experiment executed:** this audit is documentary and analytical. It neither authorizes nor reports execution of A–F.

### Consolidated findings for §§75–89

- The batch is primarily a set of research proposals and methodological safeguards, not a body of empirical results.
- A is a formal reasoning benchmark, not evidence of information creation from nothing. B remains domain-agnostic and non-executable.
- C is observational unless a safe, controlled manipulation is specified; it cannot establish a thermodynamic cause of distraction.
- D and E can test local behavioural interventions, but do not validate the whole ROOT package. If–then plans already have a substantial evidence base.
- F tests adaptive-control performance unless its proposed meta-level operation is separately defined and measured.
- The governing plan contains substantially stronger protocol specifications than the treatise's short summaries. Those gates remain open.
- §§83–88 contain useful limitations and safeguards; §89 requires a normative governance model before goal review can be treated as an implemented capability.
- No experiments were run, no treatise/tracker edits were warranted by this batch, and no execution authorization is inferred.

**Status:** §§75–89 have a first-pass claim-level methodological, evidential and disposition audit. This does not complete the full 95-section audit, make A–F executable, or validate the four-theory integration. Protocol readiness gates, full source verification, cross-component discrimination, final dispositions and the remaining §§90–95 audit remain open.

## 19. Additional source register: Sections 75–89

### R48 — Meta-analysis of implementation intentions, 2024

“The when and how of planning: Meta-analysis of the scope and components of implementation intentions in 642 tests,” *European Review of Social Psychology* (2024), pp. 162–194, DOI: [10.1080/10463283.2024.2334563](https://doi.org/10.1080/10463283.2024.2334563).

**Evidence type and scope:** meta-analysis of 642 independent tests of implementation intentions across cognitive, affective and behavioural outcomes.

**Relevant result:** reported effects ranged from d = 0.27 to d = 0.66 across outcome groupings. Effects were larger when plans used a contingent if–then format, participants were highly motivated to pursue the goal, and plans were rehearsed.

**Supports:** the existence of a substantial prior evidence base for trigger-linked if–then planning and rehearsal, relevant to §80.

**Does not support:** the efficacy of the complete ROOT protocol, the specific intervention selected for an individual, or a unique theoretical mechanism underlying ROOT.

**Pinpointing status:** publisher abstract and bibliographic record verified; exact outcome-specific forest plots and subgroup tables not independently inspected.

### R49 — Sequential randomization designs for adaptive interventions, 2026

“Experimental designs with repeated randomizations for optimizing adaptive interventions: guidelines and practical considerations,” *Annals of Behavioral Medicine* 60(1) (2026), article kaag006, DOI: [10.1093/abm/kaag006](https://doi.org/10.1093/abm/kaag006), published 13 March 2026.

**Evidence type:** methodological/conceptual guidance on sequentially randomized designs for adaptive interventions.

**Relevant distinction:** sequential multiple assignment randomized trials (SMARTs) address adaptive interventions with relatively slow decision timescales; micro-randomized trials (MRTs) address just-in-time interventions with faster, repeated decision points. Design choice depends on the scientific question, timing of adaptation and outcome measurement, randomization restrictions and sample-size planning.

**Supports:** the need to select an evaluation design for §81/F based on the controller's actual adaptation cadence and estimand; it does not make any particular F design executable.

**Does not support:** that the proposed ROOT controller is effective, that it is uniquely recursive, or that adaptive policies necessarily outperform fixed policies.

**Pinpointing status:** full publisher abstract and article text inspected; publication date, volume/issue, article identifier and SMART/MRT distinction verified.

### R50 — Reporting quality in SMART studies, 2022

Bigirumurame et al., “Sequential multiple assignment randomized trial studies should report all key components: a systematic review,” 2022, PMCID: PMC7613855, PMID: 34763037.

**Evidence type and scope:** systematic review of 157 records concerning SMART designs, including 12 trial reports, 24 protocols, 91 methodological papers and 30 reviews.

**Relevant result:** only four of the 12 trial reports (33.33%) reported parameters needed for sample-size calculations; multiple-testing adjustment was often unreported.

**Supports:** the need for explicit sample-size parameters and multiplicity handling if a sequentially randomized adaptive-controller study is later designed.

**Does not support:** that SMART is the correct design for every adaptive controller, or that a SMART/MRT label guarantees adequate design quality.

**Pinpointing status:** PubMed/PMC abstract and study counts verified; detailed study-level table not independently inspected.


## 20. Claim-level register: Sections 90–95 and final status statements

**Baseline:** `document_master_visual.md`, blob `123abdbe9ad3e6c24d150e7db2f38e9562d520d5`; section locations below refer to that unchanged baseline.

| ID | Claim / source location | Formal status and evidence assessment | Disposition and open dependency |
|---|---|---|---|
| S90-C01 | Space or Null Theory identifies dependence of meaningful processing on context and structure; context includes memory, architecture, goals and constraints (L2440–2444) | This follows substantially from the broad definitions and structural-dependence premise already stated in §§3–6. With context defined to include almost every system condition, the dependence claim is general and close to a modelling truism; it does not yet identify a distinctive mechanism or novel prediction. Internal processing without fresh sensory input is possible when retained state and active transition rules remain, but that is not processing without information or structure. | Retain as a conceptual statement about context-conditioned processing. Replace “establishes” with “proposes/describes” unless a narrower, nontrivial result is demonstrated. State the specified input class and operating conditions whenever “null” is used. |
| S91-C01 | Out of Box Theory derives conclusions not explicitly supplied as observations; internal structure can entail unobserved consequences and support empirical anticipation (L2446–2452) | The bounded inference claim is standard model-theoretic consequence, not a new result by itself. Prior audit S10-TH01 found the treatise's soundness argument overreaches: soundness gives derivable ⇒ entailed; the converse requires completeness for the chosen semantics and language. A nonempty model class is needed to avoid vacuous entailment, and a claim about actual-world truth additionally requires that the actual world satisfy K. Prediction of an unobserved event is a model-based forecast; its target correspondence must still be independently tested. | Retain the bounded claim but identify the formal result as standard entailment/inference under explicit assumptions. Correct the theorem's soundness/completeness direction before saying the theory proves derivability. Separate logical consequence, prediction and empirical discovery. |
| S92-C01 | Physical constraints, cost-sensitive control and cached habits explain why an intelligent person can execute a behaviour they reflectively reject (L2454–2462) | Physical embodiment and finite-resource constraints are well established. Cost-sensitive action selection and learned habitual/cached policies have empirical and computational support in specific paradigms, but the causal chain from energetic constraints through subjective effort and action valuation to a particular unwanted behaviour is not derived or established by this treatise. The action-score coefficients and person-level mechanism remain unvalidated; task-level cognitive energy changes cannot be inferred directly from neural metabolic costs. “This explains why” is stronger than the evidence permits. | Retain as a plausible, testable multi-level explanatory hypothesis. State the intermediate mechanisms, operational measures and competing explanations. Do not describe the physical–cognitive bridge as established or equate distraction with entropy. |
| S93-C01 | Recursive Intelligence is the capacity to represent aspects of its own operation and use them to change future operation (L2464–2470) | This functional definition closely overlaps established metacognitive knowledge and metacognitive control: monitoring/reflecting on one's cognitive processes and regulating them through planning or adaptation. Self-regulated learning and adaptive control are further neighbouring frameworks. A distinctive Recursive Intelligence contribution has not been demonstrated by a new mechanism, criterion, or discriminating prediction. Fleur et al. (2021) explicitly describe the knowledge/control distinction and the object-level/meta-level feedback relation (R51). | Retain as a proposed umbrella construct or synthesis, not an established distinct capacity. Define the necessary meta-representation, update operation and measurable discriminator from metacognition, meta-control and adaptive control; validate construct and criterion measures independently. |
| S94-C01 | ROOT is the operational implementation, comprising trigger recognition, obstruction, override, training, correction, biological/environmental optimization and consolidation (L2472–2484) | This is an intervention architecture, not an empirical result. The first four named operations form the ROOT mnemonic; the final three are additional process stages rather than separately represented letters. The component strategies have neighbouring evidence, but the integrated package has not been evaluated. The 28-day treatise schedule and 14-day tracker pilot are different proposals; the latter combines obstruction and alternative-response training and cannot isolate their effects. Protocol gates remain open. | Retain as a proposed operational protocol. Describe it as designed/proposed rather than established or proven. Reconcile the acronym/step taxonomy, define fidelity and outcomes, and keep the two durations distinct until a justified design is selected. No execution or efficacy claim. |
| S95-EQ01 | Final unified architecture: (\boxed{S_{t+1}=F(A,M_t,O_t,G_t,\mathcal{R}_t,\mathcal{I}(A,M_t),\Pi_t,R_t)}) (L2486–2519) | This is not yet a fully specified mathematical state-transition equation. The first boxed expression is a conceptual list of inputs to an opaque function. The symbolic expression does not define the domain/codomain of F, the state space, update semantics, units, transition assumptions or relation to the prior system tuple (\mathcal S_t=(A,M_t,X_t,E_t,\Pi_t,G_t,\Theta_t)) in §3 or the unified equation (\mathcal S_{t+1}=\mathcal F(\mathcal S_t,O_t,\mathcal I_t,G_t,R_t,\mathcal R_t)) in §71. It omits explicit (X_t,E_t,\Theta_t) and the selected action (a_t); the inference input (\mathcal I(A,M_t)) differs from (\mathcal I_t) and omits the formal constraints K used in §§73–74. The two boxed versions are not shown equivalent. (R_t) also has another meaning (successful rehearsal) in the habit update at L1404–1411, while §71 uses it for feedback/outcome. | Downgrade to a conceptual architecture diagram/equation until a typed, internally consistent transition model is supplied. Reconcile the state tuple and §71 equation; define every input, output, time scale, action, feedback and resource variable; remove symbol collisions; state whether F is a serial composition, coupled update or general transition kernel. Do not call it a derived unified law. |

### Cross-section dependencies and final-synthesis consistency

1. **§§90–91 versus the formal core:** §90 mainly restates the broad context definition and structural-dependence premise. §91 relies on standard logical consequence. Theorem 1 in §10 still needs the soundness/completeness correction recorded under S10-TH01; a conclusion cannot be promoted to an established theorem merely by restating it in the final synthesis. The underdetermination result in §11 is a valid model-theoretic countermodel result, but it does not establish equal probabilities, rational indifference or the full range of scientific underdetermination. The SEP entry distinguishes holist and contrastive forms and their different strengths (R52).
2. **§92 versus the physical–cognitive bridge:** physical embodiment is not equivalent to a demonstrated causal explanation of an individual action. The bridge needs separately measured energetic, cognitive, behavioural and environmental variables and a design that identifies their links. Existing cost-sensitive control and habit evidence supports neighbouring mechanisms, not the treatise's complete causal chain or its coefficients.
3. **§93 versus established metacognition:** the current definition substantially overlaps metacognitive knowledge and control. The literature distinguishes monitoring/knowledge from top-down control and notes construct and operationalization differences across disciplines (R51). A unique Recursive Intelligence claim needs an additional, operationally identifiable mechanism and an empirical discriminator; relabelling the existing feedback loop is insufficient.
4. **§94 versus implementation evidence:** ROOT is a proposed protocol assembled from intervention classes, not a demonstrated integrated treatment. The acronym's four named operations and the seven listed stages should be explicitly related. The 14-day and 28-day designs remain distinct and neither is a completed efficacy study.
5. **§95 versus §§3 and 71:** the final symbolic expression is not a faithful restatement of the earlier state equation. It drops explicit state components and changes the inference representation without a mapping. The function F is unspecified, so the expression is an architectural placeholder rather than a mathematically closed model.
6. **Abstract and concluding language:** the Abstract's claim that the four components are “not four independent mechanisms” and the conclusion's assertion that the deepest idea “connects” all named domains should be labelled as the proposed synthesis. Compatibility or conceptual fit does not prove causal integration, completeness, novelty or empirical superiority.
7. **Status-of-framework section:** “Completed in this treatise” is defensible only as a manuscript-content inventory, not as a list of scientifically completed or validated results. In particular, the formal reconciliation, theorem about derivability, physical–cognitive bridge, mathematical ROOT protocol and experimental programme retain open proof, measurement, source and execution dependencies. The two-week/four-week intervention schedules are proposals; no A–F study has been executed.
8. **Proposed Laws 1–10:** these are epistemically heterogeneous, not ten new universal laws. Laws 1–3 are broad contextual/formal statements closely related to definitions and standard logic; Law 4 is a general physical constraint; Laws 5–7 are conditional behavioural/control principles; Law 8 is an intervention architecture; Law 9 is conditional on stability assumptions that are not yet certified; Law 10 is a methodological norm. Preserve the label “proposed laws or principles” and give each its own status.
9. **No empirical validation inferred:** the final synthesis is a conclusion about the proposed architecture. It is not an experimental result, a validated unified mechanism or a proof that ROOT increases goal-consistent behaviour across people.

### Consolidated findings for §§90–95

- The final synthesis is more confident than the evidence and formal audits warrant. The recurring verb “establishes” should be downgraded to “proposes,” “describes,” or “is supported in the following limited respect,” according to each claim.
- Space or Null Theory is currently a broad context/structure principle; its distinctive contribution remains unestablished.
- Out of Box Theory's defensible core is bounded inference from supplied premises. Theorem 1 requires a completeness correction and actual-world correspondence must be distinguished from formal entailment.
- The physical–cognitive bridge is a plausible multi-level hypothesis, not a completed causal explanation of unwanted behaviour.
- Recursive Intelligence overlaps established metacognition/meta-control; distinctiveness remains unresolved.
- ROOT is an unvalidated intervention architecture. Its component strategies do not establish package-level efficacy.
- The final unified equation is presently conceptual and inconsistent with the earlier state representation. It must not be described as a derived mathematical law.
- The final “completed” list records manuscript contents, not validated research outcomes. Empirical studies remain unexecuted.
- No treatise or tracker edits were made; no experiment was executed or authorized.

**Status:** §§90–95 now have a first-pass final-synthesis, formal-consistency and evidence-status audit. All 95 numbered sections have first-pass claim-level coverage across seven batches, but the complete 95-section claim inventory is not yet fully adjudicated: source pinpointing, formal proof corrections, taxonomy crosswalk, final claim dispositions, law-by-law source traceability, cross-component integration and independent review remain open. The next step is cross-batch reconciliation and final claim-status integration, not an automatic treatise rewrite.

## 21. Additional source register: Sections 90–95

### R51 — Fleur, Bredeweg & van den Bos (2021): metacognition and meta-control

Damien S. Fleur, Bert Bredeweg and Wouter van den Bos, “Metacognition: ideas and insights from neuro- and educational sciences,” *npj Science of Learning* 6, Article 13 (2021), DOI: [10.1038/s41539-021-00089-5](https://doi.org/10.1038/s41539-021-00089-5).

**Evidence type:** interdisciplinary review of metacognition in educational science and cognitive neuroscience.

**Relevant locations:** Abstract and Introduction; especially the object-level/meta-level distinction and Fig. 1 discussion. The review describes metacognitive knowledge as awareness/monitoring of one's cognitive processes and metacognitive control as self-regulatory mechanisms such as planning and adapting behaviour based on outcomes. It describes upward meta-knowledge and downward meta-control flows.

**Supports:** the conclusion that §93's current definition overlaps established metacognition/meta-control and needs a discriminating construct if Recursive Intelligence is claimed as distinct.

**Does not support:** that Recursive Intelligence is identical to metacognition, that the proposed framework is novel, or that a particular recursive controller is effective.

**Pinpointing status:** publisher full text inspected; publication date, volume/article number, DOI, abstract, Introduction and Fig. 1 discussion verified.

### R52 — Stanford Encyclopedia of Philosophy: scientific underdetermination

Kyle Stanford, “Underdetermination of Scientific Theory,” *The Stanford Encyclopedia of Philosophy*, first published 12 August 2009; substantive revision 4 April 2023.

**Evidence type:** scholarly philosophy-of-science reference entry.

**Relevant locations:** §§1–3, especially the distinction between holist underdetermination (difficulty locating which member of an assumption set should be revised after a failed prediction) and contrastive underdetermination (multiple theories compatible with the same evidence).

**Supports:** the need to restrict §11's formal countermodel theorem to its model-theoretic scope and avoid treating it as a complete account of scientific theory choice.

**Does not support:** a universal impossibility of discriminating theories or a claim that all scientific evidence is permanently underdetermining.

**Pinpointing status:** current SEP entry inspected; title, author, publication/revision dates and relevant sections verified.
