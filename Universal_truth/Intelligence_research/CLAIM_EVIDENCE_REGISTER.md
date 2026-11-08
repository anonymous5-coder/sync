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

**Study scope and access:** full article PDF inspected. Experiment 1 recruited 101 participants and analysed 98 after preregistered response-time exclusions; Experiment 2 recruited 100 participants. Both used two-step reinforcement-learning tasks, but the task structures differed in whether model-based control delivered a reward/accuracy advantage (Experiment 1: lines 97–113, 127–140, 168–225; Experiment 2: lines 748–755, 773–806).

**Results and boundary:** increased stakes increased model-based control in Experiment 1, where model-based control could improve performance. In Experiment 2, where model-based control did not produce a reward advantage, the stakes manipulation did not increase model-based control (t(99) = −0.72, p = .470, d = −0.07; lines 952–960). The authors note that the two task structures differed in several respects and that incidental task differences could moderate the result (lines 1004–1014). Their conclusion is therefore a task-specific cost-benefit arbitration result, not a universal law of action selection (lines 1015–1037).

**Supports:** a bounded experimental case that model-based/model-free control allocation responds to task-specific performance advantages and incentives.

**Does not support:** the treatise's exact additive Q(a) formula, its coefficients, thermodynamic-energy terms, a single universal arbitration mechanism, or a causal account of any particular person's distraction.

**Pinpointing status:** full PDF inspected; participant/method and results/discussion locators above are verified.

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

**Study scope and access:** full open-access article PDF inspected. The full sample was N = 220; after task-specific exclusions, N = 213 for the two frequency-based tasks and N = 208 for cross-paradigm validity analyses (Results—Participants, lines 621–626). The convenience sample was relatively young and mostly university students; the authors identify limited generalizability and possible restricted variance as limitations (lines 1599–1604).

**Positive result:** choice frequency during training increased later frequency-based choice/habit-related measures in the Reward Pairs and Unrewarded Habits tasks; the latter suggests that a frequency-related effect can arise without external reinforcement as operationalized in that task (abstract/introduction, lines 39–41; design and hypotheses, lines 73–90).

**Contrary/limiting results:** there was no convergent validity across the six habit paradigms: correlations were near zero or negative, and the one-dimensional measurement model did not fit (lines 958–960, 1047–1053; Table 2, lines 1063–1106). The tasks also showed no criterion validity against the real-life habit questionnaires for choices, response times, stimulus ratings or computational parameters (lines 1195–1230). The authors conclude that habits appear more stimulus- and situation-specific than a single common laboratory measure suggests (lines 1550–1555, 1588–1604).

**Supports:** a frequency-based learning effect in the two studied paradigms, alongside direct evidence that these six operationalizations did not behave as interchangeable indicators of one latent habit construct in this sample.

**Does not support:** a universal one-dimensional habit trait, criterion-valid measurement of real-life habits by these laboratory tasks, or the claim that all habits are simply cached model-free policies. It also does not settle whether instructed responding in the unrewarded task was wholly free of internal reinforcement.

**Pinpointing status:** full article inspected; sample, positive effect scope, cross-paradigm non-convergence, criterion-validity findings and limitations are located above.

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

**Evidence type and design:** preregistered field experiment (N = 112) comparing grayscale design friction (n = 40), self-commitment to time limits (n = 33) and self-monitoring control (n = 39) over several weeks; screen time was measured from device records/screenshots (full PDF: lines 11–20, 96–103, 131–164).

**Relevant result:** grayscale reduced average screen time relative to control (233.19 vs 283.20 minutes/day; t(77) = 2.39, p = .019), approximately 50 minutes/day; the goal-setting group did not differ significantly from control (lines 191–201). The study found no immediate causal effect of reduced use on subjective well-being or academic performance (abstract, lines 11–20).

**Supports:** a particular design-friction intervention can reduce objectively measured smartphone screen time in the tested student setting over the observed period.

**Does not support:** general sustained-attention improvement, improved academic performance, lasting behaviour change, or a universal effect of obstruction. The trial's outcome was screen time, not a general attention or distraction measure.

**Pinpointing status:** full PDF inspected; design, sample, measurement and group contrasts located above.

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

### R46 — WFSBP guidelines for compulsive sexual behaviour disorder, 2022

Daniel Turner, Peer Briken, Joshua Grubbs, Leo Malandain, Gemma Mestre-Bach, Marc N. Potenza and Florence Thibaut, “The World Federation of Societies of Biological Psychiatry guidelines on the assessment and pharmacological treatment of compulsive sexual behaviour disorder,” *Dialogues in Clinical Neuroscience* 24(1), 10–69 (2022), DOI: [10.1080/19585969.2022.2134739](https://doi.org/10.1080/19585969.2022.2134739).

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


## 22. Cross-batch reconciliation and integrated claim-status adjudication

**Purpose and status.** This section consolidates the seven existing first-pass batches (§§1–95), the stable-ID inventory, source clusters E01–E18, the formal-result premise map, the alternatives audit and the provisional cross-component interface map. It is an integrated documentary adjudication, not independent peer review, completed source pinpointing, empirical validation or authorization to execute Experiments A–F. Existing batch histories and claim IDs are preserved.

**Inventory check.** The unchanged treatise baseline contains 95 numbered sections. The register contains 204 distinct section-scoped stable IDs: 198 conventional typed IDs plus six experiment IDs S76-EXP-A through S81-EXP-F. The final-synthesis IDs run from S90-C01 through S95-EQ01. The seven batch boundaries remain §§1–15, 16–27, 28–40, 41–59, 60–74, 75–89 and 90–95. Stable-ID coverage is an inventory result; it does not mean that all claims have final source pinpoints, validated measures, complete proofs or closed dependencies.

### 22.1 Integrated epistemic taxonomy crosswalk

The three schemes in the treatise must not be collapsed into one ordinal scale.

| Treatise scheme | What it actually classifies | Reconciled interpretation | Required treatment |
|---|---|---|---|
| Part I, four levels (physical, informational, cognitive, recursive-control) | Explanatory domain / level of analysis | These are domains or levels, not epistemic statuses. A claim at any level may be definitional, formal, empirical, model-based or normative. | Retain as a domain map; do not treat the four levels as a seven-category claim taxonomy. |
| §2, three labels (established constraint, derived proposition, research hypothesis) | A compressed summary mixing evidential and logical status | “Established constraint” can be empirical or formal; “derived proposition” is conditional on premises and proof system; “research hypothesis” concerns unresolved empirical or mechanistic support. These labels are not mutually exclusive across the independent dimensions. | Retain only as shorthand after adding the independent fields below. Never infer that a derived proposition has true premises or that an established constraint validates a whole theory. |
| §15, levels 0–5 (imagined possibility, internally consistent hypothesis, deductive consequence, probabilistic prediction, independently corroborated discovery, robust explanatory structure) | A suggested development path for generated claims | The stages are heterogeneous: logical derivation, probabilistic prediction, empirical corroboration and explanatory robustness are different achievements and need not form one linear sequence. A deductive consequence can be conditional on false premises; prediction and corroboration are not the same dimension. | Retain as a non-universal heuristic only. Record the actual achievement and its support independently; do not promote a claim automatically by moving up the ladder. |
| §85 labels (possibility, hypothesis, deduction, prediction, corroborated result) | Short-form epistemic reminders | These overlap the §15 ladder but still mix claim type, formal status and evidence status. | Use only as prose reminders, not as the canonical register schema. |

**Correction to a prior ledger description:** an earlier progress entry described “§1's seven categories.” Reinspection of the exact treatise baseline shows that Part I presents four explanatory levels (physical, informational, cognitive and recursive-control), not seven epistemic categories. The earlier wording is inaccurate and is corrected here. The four levels are retained as domains; the crosswalk is based on the actual §2 and §15 schemes and the independent dimensions below.

**Canonical claim record for subsequent adjudication:**

1. **Claim kind:** question; definition; physical premise/constraint; mathematical identity; formal theorem/proposition; model/equation; empirical or developmental claim; causal/mechanistic hypothesis; prediction; methodological or normative principle; intervention/protocol.
2. **Formal validity:** not applicable; standard identity/result under stated conditions; follows from explicit premises; conditionally follows with missing/unstated premises; schematic/undefined; invalid as stated. Formal validity is not empirical truth.
3. **Evidence status:** established within a specified domain; directly supported but bounded; indirectly supported or supported by neighbouring evidence; mixed/contested; untested/unverified; not an empirical claim. State population, task, measurement and source quality where relevant.
4. **Disposition:** retain; retain with qualification; split; merge/cross-reference; revise; downgrade; defer pending dependency; reject only when evidence or proof warrants rejection. “Not established” is not synonymous with “false.”
5. **Open dependency:** exact source pinpoint; proof correction; operational definition; parameter identification; measurement validation; comparator/falsifier; protocol gate; typed interface; independent review; or none.

These dimensions are deliberately non-ordinal. A claim can be a valid formal result, have no empirical status, and still require revision because its premises are not established. A model can be empirically useful in one domain while remaining only a schematic representation elsewhere.

### 22.2 Integrated status matrix by claim family

| Claim family / representative stable IDs | Claim kind | Formal status | Evidence status | Integrated disposition and remaining dependency |
|---|---|---|---|---|
| Four-part programme and integration: S01-C01, S02-D01, S70-C01, S72-C01, S73-TH04 | Organizing architecture / synthesis | Compatibility is conditional; no theorem establishes the necessity or unique order of all four components | No integrated-system validation or incremental predictive advantage demonstrated | **Retain as proposed architecture.** Do not call the four foundations independently validated mechanisms or a demonstrated unified causal system. Require typed interfaces, competing integrated baselines, ablations and held-out incremental prediction. |
| Context and internal processing: S03-M01, S05-D01–D08, S06-C01–02, S28-C01, S29-C01/P04, S90-C01, LAW01 | Definitions, general computational principle, conceptual model | Broad dependence follows largely from the expansive context definition; internal computation without fresh external input is standard for systems retaining state and active transition rules | General computational fact; no distinct mechanism or novel prediction established | **Retain with narrowed scope.** Specify the absent input channel and interval; distinguish no new sensory input from no information/state. Identify a narrower transition-relevant context and a discriminator from ordinary stateful computation. |
| Information, deduction and underdetermination: S07-EQ01/P01/P02, S10-M01/EQ01/TH01, S11-TH01, S12-C01–02, S14-EQ01–02, S30-C01–02, S91-C01, LAW02–03 | Information-theoretic identities, semantic results, epistemic claims | CMI and Bayesian identities are standard under specified distributions; Theorem 2 is a valid countermodel result; Theorem 1's entailment-to-derivability direction requires completeness, not soundness alone | Supports logical possibility of deriving consequences from supplied structure; does not show arbitrary facts can be inferred or premises are true | **Retain standard results with explicit conditions; revise Theorem 1.** Specify a sound and complete proof system for the chosen language, satisfiable K/nonempty model class and, for actual-world truth, that the actual world satisfies K. Keep derivability, prediction, truth and corroboration separate. |
| Physical embodiment and resource limits: S04-A01/A05, S17-C01/EQ01–02, S18-C01/EQ01, S31-C01/EQ01–02, LAW04 | Physical premise and resource model | Physical implementation and Landauer's bound are established within their respective physical conditions; resource vector and performance function are schematic | Neural signalling is metabolically costly; task-level whole-body energy changes and subjective effort mechanisms are not reducible to that fact | **Retain physical constraints; split resource dimensions.** Landauer applies to specified logically irreversible erasure, not energy per thought. Define accounting boundary, time, bandwidth, memory, noise/error and task-specific capacity separately. |
| Physical–cognitive bridge and action arbitration: S16-C01/EQ02, S19-M01–02/C01, S20-P03, S26-M01/TH03, S92-C01, LAW05 | Multilevel causal hypothesis, score model, conditional proposition | The score inequality is algebraic under definitions; preference needs a specified greedy/softmax selector; the bridge chain is not derivable from physical embodiment alone; the final repetition/learning step in Theorem 3 needs an update rule | Cost-benefit arbitration has task-specific experimental support; it does not validate the treatise's coefficients or causal story from neural energetics to an individual's unwanted behaviour | **Retain as a testable hypothesis and schematic model.** Operationalize score terms on compatible scales, identify coefficients, specify choice and learning rules, measure subjective effort separately from neural/global energy and test alternatives. |
| Learning, habit and reward: S21-C01/EQ01, S22-EQ01, S23-C01/EQ01, S34-EQ01/C01, S35-EQ01–03, S42-C01/M01, S56-M01, LAW06 | Distinct learning mechanisms and candidate recurrences | TD-style updates are standard only after state/action/reward indexing is specified; §42 and §56 recurrences are not equivalent and neither is validated as a universal law | Habit, reinforcement and cue learning have evidence, but paradigms and constructs do not automatically converge; fixed habit-formation time is unsupported | **Split the constructs and defer canonical equations.** Distinguish Pavlovian cue–outcome, instrumental action–outcome and stimulus–response habit processes. Reconcile update equations, bound states/parameters, define opportunity and reinforcement, and validate measures. |
| Intelligence and recursive control: S05-D03, S32-C01/EQ01–02/M01, S46-M01/EQ01, S47-M01, S48-C02, S49-M01/EQ01, S50-M01, S93-C01, LAW07 | Proposed construct, model and capability hypothesis | Functional and update equations are schematic; no distinct formal criterion for Recursive Intelligence supplied | Metacognition/meta-control and adaptive-control research support neighbouring processes; no unique Recursive Intelligence mechanism or incremental advantage shown | **Retain as proposed umbrella/synthesis, not established distinct theory.** Validate intelligence independently; define a discriminating meta-level representation/update criterion against metacognition, meta-control and adaptive control. |
| ROOT and behavioural intervention: S41–S59, S69-C01/PROT01, S94-C01, LAW08 | Intervention architecture and personal protocol | Component operations can be specified; the integrated package and its controller guarantees are not proved | If–then plans and selected environmental interventions have component-level evidence; package efficacy is untested | **Retain as proposed intervention architecture.** Clarify ROOT acronym versus seven operations; reconcile 14-day tracker and 28-day treatise schedule; define fidelity, opportunity, outcomes, burden, safety and comparator. No efficacy claim. |
| Stability and controller guarantees: S60-M01/C01, S61-M01/EQ01, S62-P05/C01, S63-C01, S71-EQ01–02, S74-TH05, LAW09 | Control-theoretic result, candidate Lyapunov function, conditional theorem | Schur stability is valid for the specified homogeneous discrete-time LTI model; disturbance changes the conclusion. The proposed V is not a verified Lyapunov certificate; Proposition 5 lacks a quantified drift condition; universal guarantee is under-specified | No human controller state, A/B/K or V is identified and validated | **Retain the standard control mathematics; defer human stability claims.** Define state, domain, equilibrium, positive definiteness, update, disturbances, actuator bounds and a quantified drift condition. |
| Experiments and safeguards: S75-C01, S76-EXP-A through S81-EXP-F, S82-M01, S83-L01–S89-FM01 | Research protocols, falsifiability and normative safeguards | Protocol sketches are not results; designs test component mechanisms, not the full four-part theory | No experiment executed; A–F have open readiness gates | **Retain as proposals only.** A is formal inference from supplied premises; B awaits domain lock; C cannot establish thermodynamic causation from observation; D/E test local known interventions; F tests adaptive control unless meta-level change is measured. Keep all execution gates closed. |
| Final synthesis and status language: S90-C01–S95-EQ01 | Interpretive synthesis and conceptual equation | §95 is not a fully specified state-transition model and is not shown equivalent to §3 or §71 | No integrated validation | **Downgrade “establishes” language to “proposes,” “describes” or “is consistent with evidence for” as appropriate.** Treat “completed in this treatise” as manuscript-content inventory, not completed empirical research. |

### 22.3 Formal-result reconciliation

The formal-result map is now consolidated as follows:

- **Theorem 1 / S10-TH01:** the current proof invokes soundness for the converse direction. Soundness guarantees that derivable conclusions are entailed; completeness is needed to infer derivability from semantic entailment for the chosen formal system. Require a specified sound-and-complete calculus, fixed semantics, satisfiable K and an explicit distinction between truth in all K-models and truth in the actual world. If K has no models, entailment is vacuous.
- **Theorem 2 / S11-TH01:** valid when two models satisfy the same K under fixed semantics and disagree on p. It establishes neither p nor ¬p as entailed. It does not establish equal probabilities, rational indifference, permanent scientific underdetermination or the impossibility of abductive/evidential ranking.
- **S07-P01 and Bayesian identities S14-EQ01–02:** standard mathematical identities under specified distributions and conditioning. Mutual information is an expectation, not a guarantee of positive information gain on every individual observation.
- **S20-P03:** the algebraic decomposition can establish a score inequality. A behavioural preference follows only after specifying the selector (for example, greedy choice or softmax with positive inverse temperature), feasible actions and score scales.
- **Theorem 3 / S26-TH03:** the local-score conflict is conditional on the score definitions and selector. Repetition strengthening does not follow without a separate learning rule. Split the selection result from the habit-persistence hypothesis.
- **Proposition 5 / S62-P05:** expected improvement language is not a Lyapunov proof. A formal drift inequality, state domain, disturbance assumptions and admissible controller class are required.
- **Theorem 4 / S73-TH04:** compatibility follows under the stipulated broad definition of context. It is not evidence of novelty, necessity or empirical integration.
- **Theorem 5 / S74-TH05:** score changes imply a probability change only under a specified choice rule; repeated strengthening additionally requires a learning update.
- **Schur stability / S60:** the eigenvalue condition applies to the identified homogeneous discrete-time LTI system. Persistent disturbances require a separate bounded-input/bounded-state or input-to-state analysis; they do not imply convergence to zero.

No proof correction is silently applied to the treatise in this register. These are required controlled-edition changes, not claims that the baseline text has already been repaired.

### 22.4 State, equation and notation reconciliation

The treatise contains several different abstraction levels that must not be treated as equivalent:

| Location | Representation | Current status |
|---|---|---|
| §3 / S03-M01 | \(\mathcal S_t=(A,M_t,X_t,E_t,\Pi_t,G_t,\Theta_t)\) | Conceptual full-system inventory; component spaces, units, observability and transition semantics are not defined. |
| §46 | Self-estimate \(\widehat S_t\), parameter update \(\Theta_{t+1}\), and \(S_{t+1}=F_{\Theta_{t+1}}(S_t,I_t)\) | Recursive-control sketch; estimator and update law are unspecified. |
| §71 / S71-EQ01–02 | \(\mathcal S_{t+1}=\mathcal F(\mathcal S_t,O_t,\mathcal I_t,G_t,R_t,\mathcal R_t)\), plus operator composition | High-level system update; operator domains/codomains and composition order are unspecified. Under standard right-to-left composition, the written order may not match the prose sequence. |
| §95 / S95-EQ01 | \(S_{t+1}=F(A,M_t,O_t,G_t,\mathcal R_t,\mathcal I(A,M_t),\Pi_t,R_t)\) | Conceptual summary, not a fully typed transition equation. It omits explicit \(X_t,E_t,\Theta_t\), selected action and update semantics, and is not shown equivalent to §3 or §71. |
| §31 / S31-M01 | Resource vector \(\mathcal R=(E,T_m,B,M_c,\varepsilon)\) | Candidate constraints vector; \(\varepsilon\) is an error tolerance, not the same type as resource capacities. Separate capacities, consumed quantities and quality constraints. |
| §§42 and 56 / S42-M01, S56-M01 | Two different habit-strength recurrences | Not algebraically reconciled or empirically validated; neither is a canonical update law. |
| §§52 and 57 / S52-M01, S57-EQ01 | Reuse of \(e_t\) for accessibility and signed outcome error | Notational collision; assign distinct typed symbols. |
| §§42 and 71 | Rehearsal/reinforcement variable and feedback/outcome variable use related R notation | Define distinct variables and event windows; do not assume they are identical. |
| §§19–20, 41 and tracker | Six-term action score versus reduced reward-minus-cost and tracker metrics | No validated one-to-one mapping. Retain as distinct candidate models until units, scales and estimands are reconciled. |

The full-system tuple, behavioural state and ROOT bookkeeping vector are different abstraction levels. The prior interface map's candidate state crosswalk is not a bijection and must not be presented as one. A future canonical schema needs typed state variables, observation versus inference, reward versus outcome feedback, feasible action sets, units, missingness, provenance, versioning and explicit clocks for neural/cue events, action episodes, daily summaries and weekly policy updates.

### 22.5 Proposed Laws 1–10: integrated status

| Law | Integrated status | Disposition |
|---|---|---|
| LAW01 — Contextual Dependence | Broad state/context dependence; close to a modelling truism under the treatise's expansive context definition | Retain as a scoped principle; no novelty claim. |
| LAW02 — Internal Consequence | Standard semantic consequence/derivability claim; inherits Theorem 1's proof-system correction | Retain conditionally; correct soundness/completeness and satisfiability premises. |
| LAW03 — Epistemic Underdetermination | Standard countermodel result under fixed semantics | Retain within model-theoretic scope; do not generalize to all scientific theory choice. |
| LAW04 — Physical Embodiment | General physical premise for physically realized computation | Retain; do not infer a particular behavioural coefficient or per-thought energy. |
| LAW05 — Cost-Sensitive Selection | Conditional action-selection model with empirical neighbours | Retain as a principle/hypothesis; specify score, scales, selector and falsifiable domain. |
| LAW06 — Cached-Policy | Candidate account of learned repetition and persistence | Retain with qualified scope; distinguish habit constructs and validate the update rule. |
| LAW07 — Recursive Modification | General self-monitoring/feedback capability with established neighbours | Retain as a capability hypothesis; specify the distinct meta-level mechanism if claimed. |
| LAW08 — ROOT | Intervention architecture, not a validated law or package | Retain as a protocol proposal; no efficacy claim before controlled evaluation. |
| LAW09 — Conditional Stability | Correct only under explicit controller, state, disturbance and stability assumptions | Retain conditionally; current human stability application remains unproved. |
| LAW10 — Reality-Correction | Normative/methodological requirement | Retain as a methodological principle, not an empirical or physical law. |

**Overall law-set disposition:** preserve the treatise's explicit label “proposed laws or principles.” The ten items are heterogeneous and must not be counted as ten newly established universal laws.

### 22.6 Cross-component integration verdict

The architecture is coherent as a proposed workflow, but its links have different evidential types:

1. **Space or Null → Out of Box:** primarily definitional/functional; standard inference can operate on retained structure. No distinct mechanism is established by the compatibility argument.
2. **Out of Box → Recursive Intelligence:** a proposed computational link; no specified map from inference/prediction error to a self-model estimator and parameter update.
3. **Recursive Intelligence → ROOT:** an architectural/operational link; current overlap with metacognition, meta-control and adaptive control remains unresolved.
4. **ROOT → future context/self-model:** a proposed feedback/causal link; selected intervention components have evidence, but the integrated package and update cycle have not been validated.
5. **Physical constraints → action selection:** a multilevel mechanistic hypothesis; there is no direct derivation from Landauer or neural energy budgets to subjective effort, action-score coefficients or a specific person's behaviour.

No necessary ordering, sufficiency relation, emergent capability or incremental predictive advantage for the complete four-part architecture has been demonstrated. Preserve each component as a research proposal even if a bridge is later narrowed or rejected.

### 22.7 Consolidated dispositions and remaining gates

**Retain as established within explicit scope:** selected mathematical identities and semantic results; physical embodiment and Landauer constraints under their physical assumptions; standard LTI Schur-stability criterion; selected empirical findings such as prenatal auditory familiarity, neural signalling costs, task-specific sleep effects, implementation-intention effects and metacognitive monitoring/control findings. None validates the whole framework.

**Retain with qualification:** broad context dependence; inference from retained internal structure; model-based action arbitration; habit/cue learning; clinical boundary statements; goal review as a normative safeguard; local environmental and alternative-response interventions.

**Retain as proposed / unvalidated:** the physical–cognitive bridge; action-score coefficients; intelligence functional; logistic behavioural model; habit-strength recurrences; distinct Recursive Intelligence mechanism; ROOT as an integrated package; human Lyapunov/stability application; unified state equation; four-component causal integration.

**Revise before controlled treatise edition:** Theorem 1's soundness/completeness direction; theorem/proposition premise statements; taxonomy wording; equation and symbol collisions; §3/§46/§71/§95 state mapping; §§42/56 habit update reconciliation; action-score/tracker mapping; final-synthesis headings and “completed” language.

**Keep deferred:** exact source-side page/table/figure pinpointing for all claims; primary-source verification of remaining gaps; operational definitions and psychometric validation; full M1–M18 closure including absent M18; proof corrections in the treatise; protocol preregistration/readiness; independent review.

**Experiments A–F:** no execution occurred. All protocol gates and checkboxes remain open. No result, readiness or empirical validation is inferred from this reconciliation.

**Artifact boundary:** this section updates the claim register only. It does not alter the treatise, ROOT tracker, experimental protocols or governing safeguards. The next phase is controlled source-pinpoint closure and independent claim-by-claim review, followed by a separately authorized, evidence-led treatise revision if warranted.


## 23. Source-pinpoint verification — selected high-impact evidence clusters

**Scope.** This is a targeted source-location verification pass, not complete source closure for all 204 stable IDs. Existing source IDs are reused; no new bibliography IDs are created. “Verified” below means that the stated source, study design/result and named section/table/page locator were inspected in the source itself or its authoritative publication record. An abstract-level locator is not upgraded to a full-text result. A blocked or inaccessible full text is recorded as a limitation, not silently replaced by a secondary summary.

### 23.1 Verified source-to-claim locations

| Source ID | Stable claims materially informed | Source locator actually checked | Evidence classification and scope | Pinpoint disposition |
|---|---|---|---|---|
| R11 — Attwell & Laughlin (2001) | S17-EQ01–02, S18-C01/EQ01, S31-C01, S92-C01 | Publisher article text surfaced the Materials and Methods, Results and Discussion passages; PubMed record confirms journal metadata and abstract. The paper explicitly says estimates are built from rodent grey-matter anatomical/physiological values and simplifying assumptions. | Model-based energy budget, not a direct experiment measuring human task effort. Supports signalling costs and an energy-efficiency constraint; does not support per-thought cost or the treatise's action-score coefficients. | **Partial.** Abstract and methodological scope verified; exact printed page/figure/table locator for every numerical estimate not independently page-checked. Preserve this limit. |
| R12 — Raichle & Gusnard (2002) | S18-C01, S92-C01 | PNAS article metadata and full-text record identified; the paper is a short perspective on the brain's baseline energy budget. | Review/perspective. Supports interpreting task activation against substantial ongoing baseline metabolism. | **Partial.** Bibliographic record and article identity verified; detailed numerical claim-to-page pinpoint remains open. |
| R14 — Otto, Westbrook & Daunizeau (2026) | S19-M01, S92-C01 | PubMed abstract; review abstract and publication metadata, DOI 10.1016/j.tics.2025.10.012. | Review of information-theoretic, psychological and biological accounts; explicitly identifies unresolved questions about the subjective experience of effort. | **Abstract-level verified.** Full-text section/page pinpoint remains open. |
| R15 — Kool, Gershman & Cushman (2017) | S19-M01, S20-P03, S35-C01, LAW05 | Publisher abstract, *Psychological Science* 28(9), 1321–1333; first published 21 July 2017. Abstract specifies two experiments and the accuracy/reward manipulations. Open Practices disclosure links public data and materials at OSF. | Primary experimental article. Supports task-specific arbitration between model-based and model-free control in the tested tasks. It does not test the treatise's exact additive score or thermodynamic coefficients. | **Abstract-level verified.** Full methods, sample, effect estimates and OSF analysis not yet independently reanalysed; do not overstate the two experiments. |
| R19 — Nebe et al. (2024) | S21-C01, S34-C01, S35-C01, S42-M01, S56-M01, LAW06 | Existing registered-report record and source entry; six laboratory paradigms and self-report comparison. | Primary registered report. Supports construct non-equivalence among the tested habit paradigms and limits a single universal habit score. | **Source-level result recorded;** detailed page/table locator not re-opened in this pass. Keep full-text pinpoint open. |
| R27 — AERA, APA & NCME (2014) | S32-M01, S44-M01, S65-C01 | Full official 2014 Standards PDF inspected: Chapter 1 “Validity,” printed pp. 11–30 (especially pp. 11–13 and validity evidence); Chapter 2 “Reliability/Precision,” printed pp. 33–47 (especially Standard 2.0 at p. 42 and replication-domain requirements); Chapter 3 “Fairness in Testing,” printed pp. 49–70. PDF contents and source text identify the joint sponsoring bodies. | Authoritative professional standards. Validity attaches to a specific interpretation of scores for a proposed use; multiple intended interpretations require evidence for each. Reliability/precision is population- and replication-domain-sensitive. | **Full chapter/page pinpoint verified.** This directly supports requiring construct/criterion evidence, reliability and fairness before treating the proposed intelligence functional as a valid measurement instrument. |
| R28 — Lally et al. (2010) | S21-C01, S42-M01, S56-M01, LAW06 | Publisher abstract and article metadata, *European Journal of Social Psychology* 40(6), 998–1009; DOI 10.1002/ejsp.674. Abstract describes 96 recruited, 82 analysed, 12-week daily repetition and fitted individual asymptotes; 95%-of-asymptote estimates ranged 18–254 days among fitted cases. | Primary longitudinal real-world study using self-report automaticity items. Supports variation in automaticity trajectories under repeated behaviour/context. | **Abstract-level verified.** Publisher full text was access-blocked; exact methods/results page/table locator remains open. Do not present 18–254 days as a universal habit-formation interval. |
| R31 — Gollwitzer & Sheeran (2006) | S55-C01, S80-EXP-E, LAW08 | Publisher abstract and bibliographic record, *Advances in Experimental Social Psychology* 38, 69–119; 94 independent tests and average d = 0.65 reported in abstract. | Meta-analysis, not a single primary experiment. Supports average efficacy of implementation intentions across included goal-striving outcomes. | **Abstract-level verified.** Exact page/table, inclusion rules and moderator analyses remain open; the effect is not a guarantee or evidence for ROOT package novelty. |
| R32 — Webb & Sheeran (2008) | S55-C01, S80-EXP-E | Publisher abstract and study-level description: Study 1 meta-analysed 66 tests; Study 2 examined accessibility of plan components and cue–response association. | Mixed evidence design: meta-analysis plus a mechanism study. Supports cue accessibility/association as a mechanism within implementation-intention paradigms. | **Abstract/study-summary verified.** Exact page/table locator for the mediation analysis remains open. |
| R34 — Ochs & Sauer (2022) | S41-C01, S43-C01, S54-C01, S79-EXP-D, S94-C01, LAW08 | Publisher article abstract, *Behaviour & Information Technology* 41(16), 3598–3616; one-week field experiment, N=97, app relocation/grayscale/control. The abstract reports objective use reductions also in the control group and increased self-reported problematic use. | Primary field experiment. Supports measurement-awareness caution and need for multiple outcomes; the abstract does not establish an intervention-specific causal effect. | **Abstract-level verified.** Full methods, condition contrasts and table/figure locator remain open because publisher full text was access-blocked. |
| R45 — WHO ICD-11 CDDR (2024) | S66-C01, S88-FM01 | WHO official publication page identifies the CDDR, publication date 8 March 2024, intended clinical audience and ICD-11 status. WHO-hosted manual PDF was identified but access returned 403. | Authoritative diagnostic manual publication; category 6C72 identified in the source register. | **Publication-level verified; category page not directly inspected.** The diagnostic text is independently cross-checked against R46 Table 1 and R53 below. |
| R46 — Turner et al. / WFSBP guideline (2022) | S66-C01, S88-FM01 | Publisher-hosted full-text PDF inspected: Table 1, “Diagnostic criteria for Compulsive Sexual Behaviour Disorder for ICD-11” (PDF lines 67–75); Introduction lines 41–53 and definition discussion lines 81–89. | Clinical guideline/review reproducing ICD-11 essential features: persistent impaired control, one or more behavioural manifestations, extended duration (e.g. six months or more), and marked distress/significant impairment; distress entirely due to moral disapproval is insufficient. | **Full table/section pinpoint verified.** This is a guideline reproducing ICD-11 criteria, not the WHO manual itself. The earlier R46 bibliographic metadata was incorrect and has been corrected above: *Dialogues in Clinical Neuroscience* 24(1), 10–69 (2022), DOI 10.1080/19585969.2022.2134739. |
| R51 — Fleur et al. (2021) | S46-M01, S47-M01, S48-C02, S49-M01, S50-M01, S93-C01, LAW07 | Publisher full text: Abstract, Introduction and Fig. 1 discussion; object-level/meta-level distinction and upward monitoring/downward control flow. | Interdisciplinary review. Supports overlap between the treatise's Recursive Intelligence definition and established metacognition/meta-control. | **Section/figure-level verified** in the prior source audit; no claim that Recursive Intelligence is identical to metacognition follows. |
| R53 — Sjoerds et al. (2016) | S21-C01, S34-C01, S35-C01, S42-M01, S56-M01, LAW06 | Full Frontiers article inspected: Abstract; Introduction; Participants and Methods; Results; Discussion/Conclusion. Particularly: abstract lines 297–303; N=28 sample and eligibility lines 335–355; Discussion/Conclusion lines 497–532. | Primary cross-validation study. Two task measures showed only moderate/low shared variance for goal-directed/model-based behaviour; model-free and habit-like measures did not show the expected association. The authors caution that tasks capture distinct aspects and call for further validation. | **Full section-level pinpoint verified.** Strongly qualifies any assumption that one model-free score, one habit task or a generic recurrence captures a single universal habit construct. |
| R54 — Janssen & Lazonder (2024) | S46-M01, S48-C02, S93-C01, LAW07 | Full Springer article inspected: Abstract and Introduction, especially the meta-level/object-level model discussion (article lines 43–48 and 79–83); Results report 35 studies and overall g=0.25. | Meta-analysis of monitoring-accuracy interventions in problem-solving tasks. The pooled effect is small; intervention type and setting moderate results. This is not equivalent to the broader learning-outcome effect in R55. | **Abstract/intro/results pinpoint verified.** Supports measurable metacognitive monitoring effects with bounded magnitude and domain. |
| R55 — Guo (2022) | S46-M01, S48-C02, S49-M01, S81-EXP-F, S93-C01, LAW07 | Publisher abstract and bibliographic record, *Journal of Computer Assisted Learning* 38(3), 811–832; DOI 10.1111/jcal.12650. Abstract reports random-effects meta-analysis in computer-based learning environments and effects g=0.50 for SRL activities and g=0.40 for learning outcomes. | Meta-analysis, not a primary experiment. Supports effects of metacognitive prompts in computer-based learning environments; feedback, specificity and adaptability moderate results. These outcomes do not establish accurate self-monitoring in all contexts or a distinct Recursive Intelligence mechanism. | **Abstract-level verified.** Publisher full text was access-blocked; exact study count, page/table and detailed heterogeneity/bias analysis remain open. |
| R56 — DeCasper & Spence (1986) | S08-C01, S08-C02 | Publisher abstract and article metadata, *Infant Behavior and Development* 9(2), 133–150; DOI 10.1016/0163-6383(86)90025-1. Abstract specifies repeated maternal recitation during the final six weeks of pregnancy and newborn operant-choice preference for the familiar passage. | Primary controlled developmental experiment. Supports a narrow prenatal auditory-exposure effect on newborn auditory preference. | **Abstract-level verified.** Full procedure, sample characteristics and exact tables/results pages remain open; do not generalize to adult-like cognition or broad prenatal knowledge. |

### 23.2 Cross-source corrections and qualifications

1. **R46 metadata correction:** the actual article is Turner et al. (2022), *Dialogues in Clinical Neuroscience* 24(1), 10–69, DOI 10.1080/19585969.2022.2134739. The previous journal/year/DOI metadata in this register was wrong. The correction is made in the R46 source entry; all claims depending on R46 should use the corrected citation.
2. **R27 pinpoint closure:** the official Standards PDF is now directly inspected. The validity definition is in Chapter 1, printed p. 11; validity evidence sources begin p. 13; reliability/precision is Chapter 2, printed p. 33 onward; fairness is Chapter 3, printed p. 49 onward. Validity is evidence for a score interpretation and intended use, not a property established by merely naming a construct.
3. **R53 strengthens the habit-measurement caution:** the small N=28 cross-validation sample found only moderate shared variance for goal-directed measures and no clear association between the model-free and habit-like measures. It does not invalidate all habit research; it limits interchangeability of these specific operationalizations.
4. **R54 and R55 are not interchangeable:** R54 concerns monitoring accuracy in problem-solving tasks (35 studies; g=0.25); R55 concerns self-regulated-learning activities and learning outcomes in computer-based learning environments (abstract-level g=0.50 and g=0.40). Do not combine these effect sizes or claim that either validates a general self-monitoring mechanism.
5. **R45/R46 diagnostic traceability:** the WHO CDDR is the authoritative manual, but the direct category 6C72 page was not accessible in this pass. The WFSBP guideline's Table 1 is directly verified and reproduces the required criteria. The 2018 WHO working-group paper (R57 below) independently explains the anti-overpathologizing boundary; the official WHO page remains the authoritative publication reference.
6. **R11/R12/R14/R15 and R28/R31/R32/R34/R55/R56:** where the publisher full text was blocked or only the abstract was accessible, the record remains abstract-level/partial. Exact tables, sample flow, heterogeneity, sensitivity analyses and page pinpoints are not marked closed.
7. **No source in this batch validates the treatise's proposed action-score coefficients, intelligence functional, habit recurrences, ROOT package efficacy or complete four-component integration.** Evidence for neighbouring components is not evidence for the integrated theory.

### 23.3 Additional authoritative cross-check source

#### R57 — Kraus et al. (2018): ICD-11 CSBD diagnostic boundary

Shane W. Kraus, Richard B. Krueger, Peer Briken, Michael B. First, Dan J. Stein, Meg S. Kaplan, Valerie Voon, Carmita H. N. Abdo, Jon E. Grant, Elham Atalla and Geoffrey M. Reed, “Compulsive sexual behaviour disorder in the ICD-11,” *World Psychiatry* 17(1), 109–110 (2018), DOI: [10.1002/wps.20499](https://doi.org/10.1002/wps.20499).

**Evidence type:** WHO working-group explanatory article accompanying the ICD-11 proposal; authoritative contextual explanation, not the diagnostic manual itself.

**Verified locations:** Full text inspected, especially lines 154–166. It states the persistent impaired-control pattern, extended duration and functional impairment/distress requirement; distinguishes high sexual interest without impaired control/impairment from CSBD; excludes distress solely from moral disapproval; and notes that ICD-11 classified CSBD as an impulse-control disorder rather than assuming an established behavioural-addiction mechanism.

**Supports:** the non-pathologizing qualification of §66 and the separation of sexual frequency/urge from disorder-level impaired control and impairment.

**Does not support:** diagnosing any individual, treating moral conflict as disorder, or assuming that CSBD is mechanistically identical to substance addiction.

**Pinpointing status:** full-text section and lines verified.

### 23.4 Remaining source-pinpoint backlog

The following are not closed by this batch:

- Full-text/table-level verification for R11, R12, R14, R15, R19, R28, R31, R32, R34, R55 and R56.
- Primary-study mapping beneath review/meta-analysis claims, especially R13, R14, R31, R48, R49, R50, R54 and R55.
- Exact source-to-claim mapping for every stable ID rather than representative claim families.
- Contrary/negative evidence for all intervention and cognitive-control claims, beyond the source-specific qualifications already recorded.
- Full WHO CDDR category 6C72 page pinpoint; R46/R57 are cross-checks, not substitutes for the manual.
- Full source verification for the remaining clinical, sleep, development, intelligence, neural energetics and experimental-method claims.

**Status:** selected high-impact source pinpoints have been closed or explicitly classified as abstract-level/partial. One material bibliography error (R46) has been corrected. No scientific claim has been upgraded solely because its citation metadata was verified. No treatise or tracker edits; no experiment executed or authorized.


## 24. Source-pinpoint verification — development, habit, sleep and single-case methods

**Scope.** This follow-on pass checks the remaining high-impact evidence clusters identified in §23. It prioritizes original study design, effect-domain specificity and contrary/limiting findings. It does not complete source mapping for every stable ID.

### 24.1 Verified source-to-claim locations

| Source ID | Stable claims materially informed | Source locator actually checked | Evidence classification and scope | Pinpoint disposition |
|---|---|---|---|---|
| R06 — DeCasper & Spence (1986) | S08-C01–02 | Publisher abstract and article metadata, *Infant Behavior and Development* 9(2), 133–150. Abstract specifies maternal recitation during the final six weeks of pregnancy, newborn operant-choice testing and a matched control group. | Primary controlled developmental experiment. Supports prenatal auditory exposure affecting newborn auditory preference, not general cognition. | **Abstract-level verified.** Publisher full text access-blocked; full sample/procedure/results table locator remains open. |
| R07 — Weiss et al. (2024) | S08-C01–02 | Review metadata and abstract-level scope in *Nature Human Behaviour* 8, 1251–1262. | Review of developmental trajectories across prenatal, birth and infancy. Secondary evidence, not a primary experiment establishing a particular innate capacity. | **Review-level verified.** Exact chapter/figure and primary-study trace not completed. |
| R08 — Dehaene-Lambertz & Spelke (2015) | S08-C01–02 | Review metadata and abstract-level scope, *Neuron* 88(1), 93–109. | Review of early brain organization and infant cognition. Supports early-emerging, domain-specific capacities with developmental caveats. | **Review-level verified.** Exact figure/section-to-claim map and underlying primary studies remain open. |
| R25 — Lim & Dinges (2010) | S37-C01, S67-C01, S67-C01, S78-EXP-C | PubMed abstract and article metadata, *Psychological Bulletin* 136(3), 375–389. Abstract specifies 70 articles, 147 cognitive tests, six cognitive categories and the range from negligible reasoning-accuracy effects to large simple-attention lapse effects (g = −0.776). | Meta-analysis of short-term total sleep deprivation under 48 hours. Domain-specific effects; not a study of chronic partial sleep restriction or an individual diagnosis. | **Abstract-level verified.** Full article table/forest-plot and moderator pinpoints remain open. |
| R29 — Singh et al. (2024) | S21-C01, S42-M01, S56-M01, LAW06 | Full-text PMC search-extracted article sections: Results §3.1 (study selection/risk of bias), §3.2 (study characteristics), Discussion §4 and Conclusions §5. 20 studies, 2,601 participants; 11 studies high risk of bias; only four studies supplied time-to-formation estimates; substantial variability (4–335 days). | Systematic review/meta-analysis of health behaviours. The 59–66 day median and 106–154 day mean values summarize four studies only; they are not universal habit-formation constants. | **Section/table-level source text verified.** Detailed study-level extraction and supplement table S3 not independently checked in this pass. |
| R30 — Ebert & Lin (2024) | S28-C01, S42-M01, S56-M01, LAW06 | PubMed and publisher abstract, *Annals of Behavioral Medicine* 58(11), 741–751; randomized planning intervention, N=127, consistent-context vs varied-context vs no-planning control; four-week intervention and four-week follow-up; daily steps measured by accelerometer and automaticity measured. | Primary randomized intervention. Consistent-context planning increased automaticity relative to comparisons; both planning groups increased steps during intervention. Unexpectedly, the consistent-context group did not show walking maintenance; stronger automaticity across participants was associated with maintenance. | **Abstract-level verified.** Full methods, randomization, attrition and result-table/figure pinpoints remain open. Do not claim context consistency alone maintains behaviour. |
| R41 — N-of-1 randomized intervention trials review (2018) | S69-C01/PROT01, S79-EXP-D, S80-EXP-E, S81-EXP-F | Existing article metadata, abstract and Table 1 identification; 54 publications and 1,193 participants. | Systematic review/methodology critique. Supports repeated outcomes, reversible interventions, washout, credible comparators, a priori measurement/analysis and randomization/counterbalancing where feasible. | **Table identified;** individual recommendation/page pinpoints remain open. |
| R43 — Lowe, Safati & Hall (2017) | S37-C01, S67-C01, S67-C01, S78-EXP-C | PubMed abstract, *Sleep Medicine Reviews* 36, 48–57; 61 studies across 71 populations; pooled overall cognitive-processing effect g = −0.383 and sustained-attention effect g = −0.409; several moderators reported. | Meta-analytic review of short-term sleep restriction. Supports average impairment in sustained attention and other domains, but not a universal effect across every cognitive domain. | **Abstract-level verified.** Forest-plot/table locator remains open. |
| R44 — Wüst et al. (2024) | S37-C01, S67-C01, S67-C01, S78-EXP-C | PubMed abstract, *Sleep Medicine Reviews* 76, Article 101940; 44 studies of one night with 2–6 hours sleep opportunity. Subjective sleepiness increased (SMD 0.986); sustained-attention reaction times (0.512) and lapses (0.489) worsened; no significant pooled effects for choice reaction time, cognitive throughput, working memory or inhibitory control. | Systematic review/meta-analysis. The domain-specific null findings are as important as the positive sustained-attention findings. | **Abstract-level verified.** Full-text study inclusion, risk-of-bias and sensitivity-analysis pinpoints remain open. |
| R47 — SCRIBE 2016 | S69-C01/PROT01, S79-EXP-D, S80-EXP-E, S81-EXP-F | Reporting-guideline record and design definition inspected: single-case experimental designs require prospective repeated measurement and systematic manipulation across phases; a simple pre/post diary is not equivalent. | Methodological reporting guideline, not evidence of efficacy. | **Definition-level verified.** Full checklist item-by-item application is deferred until an experiment is authorized. |

### 24.2 Evidence interpretation corrections

1. **Prenatal learning:** R06 supports a specific auditory-familiarity effect after repeated late-pregnancy exposure. R07/R08 are reviews that contextualize development; they do not establish adult-like reasoning or broad factual knowledge in newborns. The §8 claim must remain domain-specific.
2. **Habit formation:** R28 is a 12-week longitudinal study with fitted automaticity trajectories; R29 is a review/meta-analysis of health behaviours with only four studies reporting time estimates and 11/20 studies rated high risk of bias; R30 is a randomized walking-context intervention with an important distinction between automaticity and maintenance; R53 finds limited convergence between two habit-like task measures. Taken together, these sources oppose a single universal habit-strength variable or fixed formation duration.
3. **Sleep:** R25 concerns short-term total sleep deprivation; R43 concerns short-term sleep restriction across studies; R44 concerns one night of partial restriction (2–6 hours opportunity). They support sleep as a relevant state variable, especially for sustained attention, but have different exposure definitions and outcome domains. Their effect sizes must not be pooled informally or used as a personal causal coefficient.
4. **Sleep-domain specificity:** R44 found no significant pooled effects for choice reaction time, cognitive throughput, working memory or inhibitory control despite significant sleepiness and sustained-attention effects. Do not summarize it as “one bad night impairs all cognition.”
5. **Personal protocol:** R41 and R47 are design/reporting guidance. They do not turn a self-tracking schedule into an experiment. A future N-of-1 design still needs an estimand, repeated outcome, manipulation, comparator, randomization/counterbalancing where appropriate, washout/reversibility and missing-data plan.

### 24.3 Current closure status

- R06, R25, R30, R43 and R44 are **abstract-level** in this pass; the full text or detailed forest plots were not page-pinned.
- R07/R08 remain **review-level** sources; their underlying primary-study trace is not complete.
- R29 has **section-level** text for study selection, risk of bias and discussion, but its supplement table and study-by-study extraction remain open.
- R41/R47 are **methodological** sources; the full checklist has not been applied to any authorized experiment.
- No evidence in this batch upgrades the treatise's habit equations, fatigue coefficient, intelligence score, causal physical–cognitive bridge or ROOT package.

**Status:** the development, habit, sleep and single-case source clusters now have more precise scope and locator records. Remaining source access and claim-to-primary-study mapping gaps are explicit. No treatise or tracker edits; no experiment executed or authorized.


## 25. Source verification — effort, reward valuation and intelligence measurement

### 25.1 Verified source-to-claim locations

| Source ID | Stable claims materially informed | Source locator actually checked | Evidence classification and scope | Pinpoint disposition |
|---|---|---|---|---|
| R13 — Kondrakiewicz & Nawrocka (2025) | S18-C01, S19-M01, S31-C01, S92-C01, LAW04–05 | Author-institution repository full metadata record and abstract; DOI 10.1016/j.neubiorev.2025.106450. Abstract states that brain-imaging and whole-body measurements in mammals typically show minimal or no overall energy-expenditure increase during cognitive tasks and emphasizes the high cost of baseline/resting brain activity. | Review of experimental evidence, not a new primary experiment. It challenges the assumption that every cognitive act imposes a large additional whole-body metabolic cost; it does not deny neural signalling costs or subjective effort. | **Abstract and repository metadata verified.** Publisher full text is access-blocked; its cited primary-study inventory and exact page/figure locators remain open. |
| R14 — Otto, Westbrook & Daunizeau (2026) | S19-M01, S92-C01, LAW05 | PubMed abstract and bibliographic record; review compares information-theoretic, psychological and biological accounts and explicitly identifies unresolved mechanisms of subjective effort cost. | Review/theory synthesis. Supports the conclusion that experienced effort is not reducible to a settled single metabolic mechanism. | **Abstract-level verified.** Full-text sections and detailed account-by-account predictions remain open. |
| R23 — Berridge & Robinson (2016) | S35-C01, S21-C01, S34-C01, LAW06 | Full PMC article inspected: Abstract (lines 69–73); historical evidence and early dopamine-lesion/stimulation findings (76–88); definition of incentive-salience “wanting” and cue/state interaction (89–102); addiction-specific sensitization and scope (115–126); caveats and individual vulnerability (137–160). | Review of incentive-sensitization research, integrating animal and human evidence. It distinguishes incentive-salience “wanting” from hedonic “liking”; the sensitization theory is specifically an addiction account and does not make every ordinary urge a sensitized incentive-salience process. | **Full section-level pinpoint verified.** Apply only to the distinction and its studied scope; do not generalize addiction-specific mechanisms to ordinary distraction without separate evidence. |
| R24 — Shenhav, Botvinick & Cohen (2013) | S19-M01, S20-P03, S35-C01, S46-M01, S92-C01, LAW05/Law 07 | Full PMC article inspected: Summary and introduction (76–99); computational basis and controlled/automatic processing (100–136); cost of control and optimization (137–150); EVC equations (Eq. 1–3, lines 151–180). | Theoretical/normative neuroscience model integrating expected outcomes, reward/payoff and cost of control to explain allocation of cognitive control. It explicitly presents a model of control allocation, not a direct measure of thermodynamic energy expenditure. The authors state that novelty lies in formal integration rather than novelty of individual ingredients. | **Full section/equation pinpoint verified.** This is a close established conceptual neighbour for the treatise's cost-sensitive action selection; the treatise must state its distinct incremental contribution rather than treating generic reward-minus-cost arbitration as novel. |
| R27 — AERA, APA & NCME (2014) | S32-M01, S44-M01, S65-C01 | Full official Standards PDF: Chapter 1 validity definition and sources of evidence (printed pp. 11–21; especially validity definition and score-use qualification); Chapter 2 Standard 2.0 and replication-domain guidance (printed pp. 42–43); Chapter 3 fairness in testing (printed pp. 49–70). Full source text confirms validity belongs to a particular interpretation of scores for specified use, and reliability evidence must match the intended population and replication domain. | Authoritative testing standards. A conceptual score formula does not constitute a valid instrument; evidence is required for score interpretation, intended use, reliability/precision and fairness. | **Full chapter/page pinpoint verified** in §23; this section adds the direct application to the intelligence functional and composite metrics. |
| R58 — Sternberg (2019): adaptive intelligence and general intelligence | S32-C01, S32-EQ02, S32-M01, LAW07 | Publisher/PMC metadata and abstract-level record for “A Theory of Adaptive Intelligence and Its Relation to General Intelligence,” *Journal of Intelligence* 7(4), Article 23 (2019), DOI 10.3390/jintelligence7040023. | Theoretical article distinguishing adaptive intelligence from psychometric general intelligence and arguing that adaptation depends on biological and cultural context. It is a conceptual alternative, not a validation study for the treatise's functional. | **Abstract-level verified.** Full-text section and empirical validation claims not independently assessed in this pass. |

### 25.2 Integrated interpretation

1. **Physical energy is not subjective effort.** R11 concerns neural signalling energy estimates; R12 concerns baseline brain metabolism; R13 reviews whole-brain and whole-body task/rest comparisons; R14 reviews candidate mechanisms of experienced effort. These are distinct quantities and levels of analysis. None licenses a direct conversion from subjective effort ratings to joules, global energy expenditure or the treatise's Q(a) coefficient.
2. **The EVC model is a close theoretical neighbour.** R24 already integrates expected payoff, the amount/intensity of control and a cost of control into a formal action-selection account. It is not identical to the treatise's proposed six-term score, but it means the general idea “allocate control by comparing expected benefit with cost” is not a demonstrated novel mechanism. A distinct contribution would require a specified additional state, mechanism, measurable variable or discriminating prediction that outperforms the EVC and related models.
3. **Wanting/liking requires domain discipline.** R23 supports a dissociation between cue-triggered incentive-salience “wanting” and hedonic “liking,” with substantial evidence in addiction research. The review explicitly distinguishes incentive-salience “wanting” from ordinary cognitive desire. Do not use the term as a generic label for all urges, attraction, habits or ordinary distraction.
4. **The intelligence functional remains a proposed index.** R27 requires a validity argument for each intended score interpretation/use and appropriate reliability evidence. R58 shows that “intelligence as adaptation” is already an established theoretical direction with multiple competing definitions. The treatise's weighted sum therefore needs construct definition, operational indicators, task sampling, reliability, convergent/discriminant evidence, criterion/predictive evidence, fairness/invariance analysis and independent validation. It cannot be validated by showing that its own components correlate with its own success criterion.
5. **Do not collapse neighbouring theories.** EVC, adaptive intelligence, incentive salience and metacognition are not the same construct as the treatise's proposed components. Their existence constrains novelty claims and supplies comparators; it does not prove identity or disprove every possible extension.

### 25.3 New source record

#### R58 — Robert J. Sternberg (2019): adaptive intelligence and general intelligence

Robert J. Sternberg, “A Theory of Adaptive Intelligence and Its Relation to General Intelligence,” *Journal of Intelligence* 7(4), Article 23 (2019), DOI: [10.3390/jintelligence7040023](https://doi.org/10.3390/jintelligence7040023).

**Evidence type:** theoretical article/review, not a new psychometric validation study.

**Supports:** the existence of a developed theoretical distinction between psychometric general intelligence and intelligence understood as adaptation to environmental and cultural contexts.

**Does not support:** the validity of the treatise's weighted intelligence functional, the proposed component weights, or a unique definition of intelligence.

**Pinpointing status:** publication metadata and abstract verified; full-text page/section pinpoint remains open.

**Status:** selected reward/effort and intelligence-measurement sources have been checked and mapped. The evidence constrains novelty and causal language but does not validate the treatise's action score or intelligence index. No treatise/tracker edits; no experiments executed or authorized.

### R59 — McGrew (2023): Carroll's three-stratum theory, CHC structure and psychometric network analysis

Kevin S. McGrew, “Carroll’s Three-Stratum (3S) Cognitive Ability Theory at 30 Years: Impact, 3S-CHC Theory Clarification, Structural Replication, and Cognitive–Achievement Psychometric Network Analysis Extension,” *Journal of Intelligence* 11(2), Article 32 (2023), DOI: 10.3390/jintelligence11020032. PMID: 36826930; PMCID: PMC9959556.

**Evidence type:** theoretical/historical review plus secondary psychometric analyses of an archived 46-test Woodcock–Johnson III dataset, including exploratory factor analysis, bifactor confirmatory factor analysis and psychometric network analyses.

**Supports:** a substantial established comparator for the structure of human cognitive abilities; the article reports analyses consistent with a dominant psychometric g factor and multiple broad cognitive abilities in the examined dataset. It also illustrates the need to specify test indicators, factor structure, model comparisons and criterion domains rather than infer validity from a conceptual list.

**Does not support:** the treatise's five-component adaptive intelligence score, its task-dependent weights, its proposed operational definition, or the claim that its composite adds predictive value beyond established cognitive-ability measures. It is not an independent new-sample validation of the treatise's construct.

**Important limitations:** the analyses reuse an archived 46-test dataset rather than a new independent sample; the underlying publisher data are proprietary and unavailable for independent reanalysis in the article; the author declares a financial conflict of interest involving the Woodcock–Johnson III/IV batteries. The article itself notes that some alternative factor models had broadly similar fit indices, so theoretical interpretation remains relevant.

**Pinpointing status:** bibliographic metadata and abstract verified; the PMC full-text search result exposed methods, results, model-fit discussion and limitations. A complete independent table/supplementary-material reanalysis has not been performed.

**Status:** comparator source for psychometric structure and validation design; not validation of the treatise's proposed index.


## 26. Exhaustive stable-ID/source traceability matrix — structural audit and crosswalk correction

**Baseline and scope.** This matrix is compiled against the current edition branch baseline: treatise blob 123abdbe9ad3e6c24d150e7db2f38e9562d520d5, register blob 56859854fde83111edabd8e84b07038add291150, and governing-plan blob 261648d107549951a2632676a259dbd6b53d18d1. The branch compares as 99 commits ahead of main and 0 behind; this work does not merge or modify main. The 204-ID inventory was independently regenerated and reconciled against every stable ID in the first column of the claim tables: **204/204 stable IDs are represented**. There are 153 table rows because some rows deliberately group multiple stable IDs. This is a structural coverage check, not proof that every claim has a complete source trail.

### 26.1 Crosswalk integrity findings

The first-pass E01–E10 crosswalk and later supplemental E11–E15 mappings remain useful navigation aids, but several references do not match the register's canonical stable IDs. Historical records are preserved; this section supplies normalized aliases for subsequent work.

| Historical alias | Canonical registered ID | Correction |
|---|---|---|
| S07-M01 | S07-EQ01 | E10 used an unregistered ID; the actual ID is S07-EQ01. |
| S78-E03 | S78-EXP-C | E03 used a stale experiment alias. |
| S42-EQ01 | S42-M01 | E04 used a stale equation suffix. |
| S56-EQ01 | S56-M01 | E04 used a stale equation suffix. |
| S80-E05 | S80-EXP-E | E05 used a stale experiment alias. |
| S79-E04 | S79-EXP-D | E06 used a stale experiment alias. |
| S81-E06 | S81-EXP-F | E07 used a stale experiment alias. |
| S39-EQ02 | S39-EQ01 | E15 used a stale equation suffix. |
| S67-M01 | S67-C01 | E09/E15 used a stale claim suffix. |
| S69-M01 | S69-C01 | E09 used a stale claim suffix. |

These are label normalizations only. They do not add claims, alter the treatise or upgrade evidence status.

### 26.2 Reconciled evidence-cluster index

| Cluster | Canonical stable IDs assigned in this pass | Existing R records | Scope / limitation |
|---|---|---|---|
| E01 | S04-A01, S17-EQ02, S31-EQ01 | R09, R10 | Physical computation/Landauer; review sources cited historically are not all assigned R IDs. |
| E02 | S16-C01, S18-C01, S24-C02, S31-C01, S92-C01 | R11–R14 | Neural energetics and information/energy; does not establish behavioural coefficients. |
| E03 | S19-M01, S35-C01, S36-C01, S37-C01, S67-C01, S78-EXP-C | R13–R15, R24–R25, R43–R44 | Effort, cost-sensitive control and sleep; evidence is bounded and task-specific. |
| E04 | S21-C01, S22-EQ01, S34-EQ01, S35-EQ01, S35-EQ02, S35-EQ03, S42-M01, S56-M01 | R16, R18–R19, R26, R28–R30, R53 | Habit/RL; constructs and paradigms are not interchangeable; exact recurrences remain unvalidated. |
| E05 | S55-C01, S80-EXP-E | R31–R32, R48 | Implementation intentions; supports a component, not ROOT package efficacy. |
| E06 | S41-C01, S43-C01, S54-C01, S79-EXP-D | R33–R34 | Environmental/digital friction interventions; mixed and context-bound findings. |
| E07 | S46-M01, S47-M01, S48-C02, S49-M01, S50-M01, S81-EXP-F | R35–R37, R51, R54–R55 | Metacognition/meta-control; neighbouring processes, not a unique Recursive Intelligence mechanism. |
| E09 | S44-M01, S45-C01, S53-M01, S65-C01, S67-C01, S69-C01, S69-PROT01, S76-EXP-A, S77-EXP-B, S78-EXP-C, S79-EXP-D, S80-EXP-E, S81-EXP-F, S82-M01 | R27, R38, R41–R42, R47, R50 | Measurement and single-case/experimental methods; guidance is not efficacy evidence. |
| E10 | S07-EQ01, S10-M01, S10-EQ01, S10-TH01, S11-TH01, S13-EQ01, S14-EQ01, S14-EQ02, S30-C01, S30-C02, S73-TH04 | R01–R05, R21–R22, R52 | Information theory, logic, Bayesian epistemology and underdetermination; formal support is premise-bounded. |
| E11 | S08-C01, S08-C02 | R06–R08 | Prenatal/developmental evidence; narrow auditory and developmental scope. |
| E12 | S16-C01, S18-C01, S31-C01 | R11–R13 | Brain energetics; distinguish signalling, baseline metabolism and task-level expenditure. |
| E13 | S35-C01 | R23 | Wanting/liking distinction; addiction-specific sensitization must not be generalized to ordinary desire. |
| E14 | S66-C01 | R45–R46, R57 | CSBD diagnostic boundary; not a diagnosis of any individual. |
| E15 | S32-M01, S39-EQ01, S44-M01, S67-C01 | R27, R42–R44 | Psychometric validity, EMA and sleep; S39-EQ01 is the canonical registered ID. |
| E08 | No direct stable-ID assignment | No direct source record | The historical E08 note describes adjacent attractor/circuit literature only and explicitly says it does not directly support a multistable model in the baseline treatise. M18 remains absent from the baseline; do not retrofit E08 onto control-theory claims as if it validated an attractor landscape. |

**E16–E18 gap.** Section 22 refers to source clusters E01–E18, and the progress log mentions E02/E12/E16, but the committed register's recoverable cluster definitions and source-to-claim assignments stop at E15. No auditable E16, E17 or E18 definition, source inventory or stable-ID mapping is present in this artifact. Their contents are unresolved, not inferred from numbering or nearby R records. Recover the originating source-map artifact/commit and reconcile it before treating E16–E18 as part of the operative evidence map.

### 26.3 Exhaustive 204-ID traceability matrix

**Reading rule.** E-cluster and R-record entries are inherited source-map associations, not a declaration that every listed source directly supports every claim in that cluster. “Cluster-level association only” means exact wording, population, method, result and limitations still require claim-specific checking. The pinpoint column records only locators already verified in §§23–25; it does not imply closure of every source in a row. A dash means no E01–E15 assignment is recorded, not that the claim is false or that no relevant literature exists.

| Stable ID | Registered claim label | E cluster(s) | Candidate R record(s) | Traceability disposition | Existing pinpoint / limitation |
|---|---|---|---|---|---|
| S01-C01 | Organizing architecture / synthesis | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S01-C02 | A valid theory must connect levels without conflating them (L55–57) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S01-Q01 | Three motivating questions: acquiring a world model; deriving unpresented conclusions; intention–behaviour divergen | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S02-C01 | Three epistemic labels: established constraint, derived proposition, research hypothesis (L67–73) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S02-C02 | Naming does not confer scientific status (L65–68) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S02-C03 | Physical constraints alone do not explain a particular behaviour (L75–80) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S02-D01 | Organizing architecture / synthesis | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S03-EQ01 | Observation kernel \(O_t\sim P(O_t\mid E_t,X_t)\) (L95–97) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S03-EQ02 | Internal transition \(X_{t+1}=F_A(X_t,M_t,O_t,a_t,\xi_t)\) (L99–101) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S03-EQ03 | Policy/action selection \(a_t\sim\Pi_t(\cdot\mid X_t,M_t,G_t)\) (L103–105) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S03-EQ04 | Memory update \(M_{t+1}=U_M(\cdots)\) (L107–109) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S03-EQ05 | Parameter update \(\Theta_{t+1}=U_\Theta(\cdots)\) (L111–113) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S03-M01 | \(\mathcal S_t=(A,M_t,X_t,E_t,\Pi_t,G_t,\Theta_t)\) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S04-A01 | Physical premise and resource model | E01 | R09, R10 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S04-A02 | Structural dependence (L135–141) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S04-A03 | Contextual acquisition (L143–149) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S04-A04 | Internal transformation (L151–157) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S04-A05 | Bounded resources (L159–165) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S04-A06 | Adaptive selection (L167–171) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S04-A07 | Recursive accessibility (L173–177) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S04-A08 | Fallible model–world correspondence (L179–186) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S05-D01 | Definitions, general computational principle, conceptual model | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S05-D02 | Null condition (L207–215) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S05-D03 | Proposed construct, model and capability hypothesis | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S05-D04 | Novelty (L228–234) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S05-D05 | Discovery (L236–242) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S05-D06 | Habit (L244–249) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S05-D07 | Distraction (L251–256) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S05-D08 | Self-mastery (L258–263) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S06-C01 | Definitions, general computational principle, conceptual model | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S06-C02 | New external observations can alter a model; internal processing can continue without new external observations (L2 | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S07-C01 | Positive conditional mutual information means an observation reduces uncertainty (L292–299) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S07-EQ01 | Information-theoretic identities, semantic results, epistemic claims | E10 | R01–R05, R21–R22, R52 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S07-P01 | Contextual acquisition can be partial (L301–308) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S07-P02 | No new observation does not imply no computation (L310–316) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S08-C01 | A newborn is not a blank machine; inherited organization, development and learning capacity precede postnatal exper | E11 | R06–R08 | Cluster association + selected pinpoint; not full source closure | R06–R08: abstract/review-level; §§24.1–24.3. |
| S08-C02 | Artificial neural networks carry architecture and parameters shaped by design/training (L325–327) | E11 | R06–R08 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S08-C03 | An empty-space intelligence thought experiment must specify substrate, memory, state, rules, energy, sensors and in | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S09-C01 | Unobserved propositions can be inferred when available premises constrain possible worlds sufficiently (L347–357) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S09-C02 | A proposition independent of all available constraints cannot be uniquely deduced (L359–362) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S10-EQ01 | \(K\models p\) iff all K-models satisfy p (L381–389) | E10 | R01–R05, R21–R22, R52 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S10-M01 | Information-theoretic identities, semantic results, epistemic claims | E10 | R01–R05, R21–R22, R52 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S10-TH01 | If K entails p, a sound inference procedure can derive p (L391–410) | E10 | R01–R05, R21–R22, R52 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S11-TH01 | Information-theoretic identities, semantic results, epistemic claims | E10 | R01–R05, R21–R22, R52 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S12-C01 | Information-theoretic identities, semantic results, epistemic claims | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S12-C02 | Six modes: combinatorial novelty, structural inference, model-based prediction, abduction, mathematical discovery,  | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S13-C01 | Architecture and memory are shaped by evolution, development, design, training and interaction (L448–454) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S13-C02 | Internal information may support prediction (L464–473) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S13-EQ01 | \(I(W;Z)>0\), where Z=(A,M), may hold (L456–462) | E10 | R01–R05, R21–R22, R52 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S14-C01 | Predictions depend on prior structure, evidence and a model linking hypotheses to outcomes (L494–500) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S14-EQ01 | Information-theoretic identities, semantic results, epistemic claims | E10 | R01–R05, R21–R22, R52 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S14-EQ02 | Posterior predictive \(P(Y\mid D)=\sum_H P(Y\mid H,D)P(H\mid D)\) (L487–492) | E10 | R01–R05, R21–R22, R52 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S15-F01 | Six-level ladder from imagined possibility to robust explanatory structure (L503–521) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S16-C01 | Multilevel causal hypothesis, score model, conditional proposition | E02, E12 | R11–R14; R11–R13 | Cluster association + selected pinpoint; not full source closure | R11–R14: mixed partial/abstract access; §§23,25. |
| S16-C02 | Thermodynamic entropy, Shannon entropy, distraction and mental effort are distinct constructs (L528–535) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S16-EQ01 | Psychological distraction is not identical to thermodynamic entropy (L537–541) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S16-EQ02 | Six-stage physical-to-behavioural bridge (L543–550) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S17-C01 | Physical premise and resource model | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S17-C02 | Information processing has energetic and temporal implementation costs (L587–588) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S17-EQ01 | First-law accounting \(\Delta U=Q+W\) (L567–577) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S17-EQ02 | Landauer bound \(Q_{min}=k_BT\ln2\) for erasure of one unbiased bit (L579–585) | E01 | R09, R10 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S18-C01 | Physical premise and resource model | E02, E12 | R11–R14; R11–R13 | Cluster association + selected pinpoint; not full source closure | R11–R14: R13/R14 abstract-level; §§23,25. |
| S18-C02 | The brain allocates limited metabolic resources across listed processes (L605–615) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S18-C03 | Difficult tasks may impose different control demands than familiar routines (L617–623) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S18-EQ01 | Decomposed brain-power budget \(P_{brain}=P_{baseline}+P_{signalling}+P_{plasticity}+P_{regulation}\) (L596–603) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S19-C01 | The score is not a literal claim about a central brain computation (L664–665) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S19-M01 | Multilevel causal hypothesis, score model, conditional proposition | E03 | R13–R15, R24–R25, R43–R44 | Cluster association + selected pinpoint; not full source closure | R13–R15 and R24; R24 full section/equation; §25. |
| S19-M02 | Softmax action-selection distribution (L651–663) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S20-C01 | A familiar competing action can outrank a long-term goal under current local conditions (L668–692) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S20-P03 | Multilevel causal hypothesis, score model, conditional proposition | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | R24 full section/equation; §25. |
| S21-C01 | Distinct learning mechanisms and candidate recurrences | E04 | R16, R18–R19, R26, R28–R30, R53 | Cluster association + selected pinpoint; not full source closure | R19, R28–R30 and R53; R53 full text, R29 section-level, R28/R30 abstract-level; §§23–24. |
| S21-C02 | Cached responses can become maladaptive when goals or contexts change (L748–755) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S21-EQ01 | \(C_h<C_m\) (L742–746) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S22-C01 | Repeated cue–action–outcome pairings can bias later action selection (L773–780) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S22-EQ01 | Distinct learning mechanisms and candidate recurrences | E04 | R16, R18–R19, R26, R28–R30, R53 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S23-C01 | Distinct learning mechanisms and candidate recurrences | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S23-C02 | Avoidance may be maintained by relief from task discomfort (L801–810) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S23-EQ01 | \(u_t>u_{t+1}\) (L789–793) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S24-C01 | The second law does not imply that a brain locally seeks disorder or that distraction is entropy maximization (L813 | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S24-C02 | Biological organization is maintained through energy/material exchange and entropy export (L824–830) | E02 | R11–R14 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S25-C01 | Helmholtz free energy and variational free energy are not interchangeable (L840–846) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S25-EQ01 | Helmholtz free energy \(F=U-TS\) (L833–838) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S26-M01 | Multilevel causal hypothesis, score model, conditional proposition | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S26-TH03 | A cost-sensitive controller may select a locally favoured habitual response that conflicts with a higher-order goal | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S27-H01 | Accessibility, initiation cost, task uncertainty/effort, fatigue/stress, delayed reward and immediate relief/stimul | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S27-H08 | Environmental change may improve behaviour before urge disappears (L?; final sentence of §27) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S28-C01 | Definitions, general computational principle, conceptual model | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S28-EQ01 | Conditional transition distribution (L910–916) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S28-EQ02 | Four-part context decomposition (L932–948) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S29-C01 | Definitions, general computational principle, conceptual model | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S29-EQ01 | \(Y=\mathcal I(Z)\) (L958–962) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S29-P04 | Internal inference requires structure, not fresh sensory input (L968–976) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S30-C01 | Information-theoretic identities, semantic results, epistemic claims | E10 | R01–R05, R21–R22, R52 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S30-C02 | Deterministic computation can expose implicit consequences without generating information about arbitrary unconstra | E10 | R01–R05, R21–R22, R52 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S30-EQ01 | “Novel output” does not imply information from nothing (L1002–1008) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S30-EQ02 | “Implicit consequence” does not imply explicit prior representation (L1008–1010) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S31-C01 | Physical premise and resource model | E02, E12 | R11–R14; R11–R13 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S31-EQ01 | Landauer erasure inequality (L1035–1041) | E01 | R09, R10 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S31-EQ02 | \(\mathcal P_{max}=\Phi(\mathcal R,A,task)\) (L1053–1056) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S31-M01 | Resource vector \(\mathcal R=(E,T_m,B,M_c,\varepsilon)\) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S32-C01 | Proposed construct, model and capability hypothesis | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S32-EQ01 | Computation as state transformation (L1082–1086) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S32-EQ02 | Intelligence as adaptive use of state transformation (L1088–1092) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S32-M01 | Weighted intelligence functional \(\mathcal I=w_1G+w_2A_d+w_3P+w_4T_r+w_5R_c\) (L1094–1104) | E15 | R27, R42–R44 | Cluster association + selected pinpoint; not full source closure | R27 full official Standards PDF; §23. |
| S33-C01 | Investigation A is “resolved at the level of a formal framework” (L1107–1120) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S34-C01 | Cue–action–outcome learning can increase later response readiness (L1123–1158) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S34-EQ01 | Distinct learning mechanisms and candidate recurrences | E04 | R16, R18–R19, R26, R28–R30, R53 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S35-C01 | Anticipatory motivation and learned policy can persist despite modest experienced pleasure (L1161–1175) | E03, E13 | R13–R15, R24–R25, R43–R44; R23 | Cluster association + selected pinpoint; not full source closure | R23–R24 full sections; §25. |
| S35-C02 | Arbitration weight may depend on uncertainty, effort, fatigue, reliability and task demand (L1199–1208) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S35-EQ01 | Distinct learning mechanisms and candidate recurrences | E04 | R16, R18–R19, R26, R28–R30, R53 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S35-EQ02 | Model-free value \(Q_{MF}(s,a)\) (L1185–1187) | E04 | R16, R18–R19, R26, R28–R30, R53 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S35-EQ03 | Weighted arbitration \(Q_{combined}=\omega(s)Q_{MB}+[1-\omega(s)]Q_{MF}\) (L1189–1197) | E04 | R16, R18–R19, R26, R28–R30, R53 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S36-C01 | Deliberative and automatic control can be compared by benefits and costs (L1211–1227) | E03 | R13–R15, R24–R25, R43–R44 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S36-EQ01 | Net-utility inequality for choosing model-based versus cached control (L1229–1239) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S36-P01 | Allocate more deliberative control when uncertainty, changed environment, high consequences or expected error costs | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S37-C01 | Physiological state and environment can alter action selection and control demands (L1253–1277) | E03 | R13–R15, R24–R25, R43–R44 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S37-EQ01 | State-dependent score \(Q(a\mid s,z_t)=R(a\mid s,z_t)-C(a\mid s,z_t)\) (L1265–1273) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S38-C01 | Behavioural loops span milliseconds-to-years timescales (L1280–1293) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S39-C01 | Unwanted action is a state-dependent outcome, not a character judgement (L1324–1326) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S39-EQ01 | Logistic probability of competing action (L1309–1324) | E15 | R27, R42–R44 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S39-M01 | Six-variable state \(s_t=(g_t,c_t,u_t,f_t,z_t,h_t)\) (L1296–1307) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S40-C01 | Five-point summary of cue learning, wanting/liking, habits, arbitration and state effects (L1329–1340) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S41-C01 | Trigger-specific interventions may improve sustained attention; Qh=Rh−Ch, Qg=Rg−Cg, four intervention classes (L134 | E06 | R33–R34 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S41-C02 | Trigger-specific interventions may improve sustained attention; Qh=Rh−Ch, Qg=Rg−Cg, four intervention classes (L134 | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S41-M01 | Trigger-specific interventions may improve sustained attention; Qh=Rh−Ch, Qg=Rg−Cg, four intervention classes (L134 | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S42-C01 | Distinct learning mechanisms and candidate recurrences | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S42-M01 | Two different habit-strength recurrences | E04 | R16, R18–R19, R26, R28–R30, R53 | Cluster association + selected pinpoint; not full source closure | R29–R30 and R53; mixed section/abstract/full-text access; §§23–24. |
| S43-C01 | Environmental leverage and Lambda=reduction in unwanted-action probability / implementation cost (L1421–1450) | E06 | R33–R34 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S43-EQ01 | Environmental leverage and Lambda=reduction in unwanted-action probability / implementation cost (L1421–1450) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S44-C01 | Recovery metrics and weighted composite C=w1Ag−w2Fd−w3Dd−w4Lr+w5Sc (L1451–1483) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S44-M01 | Recovery metrics and weighted composite C=w1Ag−w2Fd−w3Dd−w4Lr+w5Sc (L1451–1483) | E09, E15 | R27, R38, R41–R42, R47, R50; R27, R42–R44 | Cluster association + selected pinpoint; not full source closure | R27 full PDF; §23. |
| S45-C01 | Individualized observe–estimate–intervene–measure–update loop (L1484–1514) | E09 | R27, R38, R41–R42, R47, R50 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S45-C02 | Individualized observe–estimate–intervene–measure–update loop (L1484–1514) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S45-EQ01 | Individualized observe–estimate–intervene–measure–update loop (L1484–1514) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S46-EQ01 | Self-model S_hat=M(S,observations), parameter update Theta(t+1)=Theta(t)+DeltaTheta(S_hat,G,error), and transition  | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S46-M01 | Proposed construct, model and capability hypothesis | E07 | R35–R37, R51, R54–R55 | Cluster association + selected pinpoint; not full source closure | R51 full article previously inspected; §§23,25. |
| S47-C01 | Recursive feedback loop in which an outcome modifies future parameters/policy (L1548–1571) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S47-M01 | Proposed construct, model and capability hypothesis | E07 | R35–R37, R51, R54–R55 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S48-C01 | Self-models are fallible; explanations should be judged by prospective predictions under controlled change (L1572–1 | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S48-C02 | Proposed construct, model and capability hypothesis | E07 | R35–R37, R51, R54–R55 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S49-C01 | Discounted objective J(pi) and update pi(t+1)=Update(pi(t),estimated gradient,feedback) (L1591–1625) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S49-EQ01 | Discounted objective J(pi) and update pi(t+1)=Update(pi(t),estimated gradient,feedback) (L1591–1625) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S49-M01 | Proposed construct, model and capability hypothesis | E07 | R35–R37, R51, R54–R55 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S50-C01 | Ordered goal hierarchy G0≺G1≺G2≺G3 and revisable higher-level constraints (L1626–1653) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S50-M01 | Proposed construct, model and capability hypothesis | E07 | R35–R37, R51, R54–R55 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S51-C01 | ROOT Control Protocol as seven stages: Recognise, Obstruct, Override, Train, Correct, Optimise, Learn (L1654–1671) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S52-C01 | Seven-variable ROOT state s=(c,u,f,d,g,h,e) (L1672–1691) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S52-M01 | Reuse of \(e_t\) for accessibility and signed outcome error | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S53-C01 | Trigger record E=(c,s,a,r,tau) and distinction between trigger and action (L1692–1711) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S53-M01 | Trigger record E=(c,s,a,r,tau) and distinction between trigger and action (L1692–1711) | E09 | R27, R38, R41–R42, R47, R50 | Cluster association + selected pinpoint; not full source closure | R53 full article; §23. |
| S54-C01 | Obstruction lowers accessibility e'<e and is expected to lower p_h(s | E06 | R33–R34 | Cluster association + selected pinpoint; not full source closure | R54 full article sections; R55 abstract-level; §23. |
| S54-EQ01 | Obstruction lowers accessibility e'<e and is expected to lower p_h(s | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S55-C01 | If–then implementation intention maps a specified cue to a concrete alternative action (L1740–1755) | E05 | R31–R32, R48 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S56-M01 | Two different habit-strength recurrences | E04 | R16, R18–R19, R26, R28–R30, R53 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S57-C01 | Signed error e=y*−y and correction based on outcome deviation (L1782–1802) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S57-EQ01 | Reuse of \(e_t\) for accessibility and signed outcome error | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S58-C01 | Optimisation across sleep, activity, nutrition, workload, environment, task difficulty and recovery (L1803–1819) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S59-C01 | ROOT feedback cycle; cycle output becomes context for the next cycle (L1820–1852) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S59-M01 | ROOT feedback cycle; cycle output becomes context for the next cycle (L1820–1852) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S60-C01 | Closed-loop behavioural model \(x_{t+1}=(A-BK)x_t+w_t\); stability when eigenvalues lie inside unit circle (L1853–1 | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S60-M01 | Control-theoretic result, candidate Lyapunov function, conditional theorem | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S61-EQ01 | Lyapunov-style \(V(x)\) as weighted sum of squared goal deviation, unwanted habit activation and return latency; ex | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S61-M01 | Control-theoretic result, candidate Lyapunov function, conditional theorem | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S62-C01 | Proposition 5: repeated effective feedback reduces expected frequency or duration of unwanted responses under five  | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S62-P05 | Control-theoretic result, candidate Lyapunov function, conditional theorem | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S63-C01 | Control-theoretic result, candidate Lyapunov function, conditional theorem | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S64-C01 | Self-mastery does not require zero urge; goal-action probability conditional on positive urge should remain meaning | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S64-EQ01 | Self-mastery does not require zero urge; goal-action probability conditional on positive urge should remain meaning | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S65-C01 | Separate phone, gaming, television, sleep, sexual distraction and study-avoidance behaviours rather than assume one | E09 | R27, R38, R41–R42, R47, R50 | Cluster association + selected pinpoint; not full source closure | R27 full PDF; §§23,25. |
| S66-C01 | Sexual attraction/urges and masturbation are not inherently pathological; CSBD requires persistent impaired control | E14 | R45–R46, R57 | Cluster association + selected pinpoint; not full source closure | R45 manual page remains open; R46 Table 1 and R57 full text checked; §23. |
| S67-C01 | Sleep timing/quality affects the operating conditions for attention and executive control; two-week log and referra | E03, E09, E15 | R13–R15, R24–R25, R43–R44; R27, R38, R41–R42, R47, R50; R27, R42–R44 | Cluster association + selected pinpoint; not full source closure | R25, R43–R44 abstract-level; §24. |
| S68-C01 | Breaking an ambiguous study task into a concrete first action reduces initiation cost and uncertainty (L2021–2038) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S69-C01 | Intervention architecture and personal protocol | E09 | R27, R38, R41–R42, R47, R50 | Cluster association + selected pinpoint; not full source closure | R41 and R47 methodological sources; checklist application remains open; §24. |
| S69-PROT01 | Personal protocol: 7-day baseline, 7-day environmental change, 14-day alternative-response training, then weekly re | E09 | R27, R38, R41–R42, R47, R50 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S70-C01 | Organizing architecture / synthesis | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S71-C01 | Unified state transition \(\mathcal S_{t+1}=\mathcal F(\mathcal S_t,O_t,\mathcal I_t,G_t,R_t,\mathcal R_t)\); \(\ma | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S71-EQ01 | \(\mathcal S_{t+1}=\mathcal F(\mathcal S_t,O_t,\mathcal I_t,G_t,R_t,\mathcal R_t)\), plus operator composition | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S71-EQ02 | Unified state transition \(\mathcal S_{t+1}=\mathcal F(\mathcal S_t,O_t,\mathcal I_t,G_t,R_t,\mathcal R_t)\); \(\ma | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S72-C01 | Organizing architecture / synthesis | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S73-C01 | Contextual and generative intelligence are complementary if context includes external observations and internal str | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S73-TH04 | Organizing architecture / synthesis | E10 | R01–R05, R21–R22, R52 | Cluster association + selected pinpoint; not full source closure | R02–R03 and R52; formal proof assumptions remain controlling. |
| S74-C01 | Self-mastery as feedback-driven policy modification under constraints; goal-action probability rises when relative  | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S74-TH05 | Control-theoretic result, candidate Lyapunov function, conditional theorem | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S75-C01 | Research protocols, falsifiability and normative safeguards | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S76-EXP-A | Research protocols, falsifiability and normative safeguards | E09 | R27, R38, R41–R42, R47, R50 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S77-EXP-B | Experiment B: predict a physical outcome before direct observation (L2226–2240) | E09 | R27, R38, R41–R42, R47, R50 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S78-EXP-C | Experiment C: effort, fatigue and task uncertainty may change habitual-distraction selection (L2242–2256) | E03, E09 | R13–R15, R24–R25, R43–R44; R27, R38, R41–R42, R47, R50 | Cluster association + selected pinpoint; not full source closure | R25 and R43–R44 abstract-level sleep sources; §24. |
| S79-EXP-D | Experiment D: obstruction of cue accessibility may reduce unwanted actions (L2258–2270) | E06, E09 | R33–R34; R27, R38, R41–R42, R47, R50 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S80-EXP-E | Experiment E: trigger-specific alternative-response training may improve recovery (L2272–2284) | E05, E09 | R31–R32, R48; R27, R38, R41–R42, R47, R50 | Cluster association + selected pinpoint; not full source closure | R31–R32 and R48; meta-analysis/abstract-level trail; §§23,25. |
| S81-EXP-F | Research protocols, falsifiability and normative safeguards | E07, E09 | R35–R37, R51, R54–R55; R27, R38, R41–R42, R47, R50 | Cluster association + selected pinpoint; not full source closure | R35–R37, R49–R51 and R54–R55; comparator and meta-level criterion remain open. |
| S82-M01 | Research protocols, falsifiability and normative safeguards | E09 | R27, R38, R41–R42, R47, R50 | Cluster-level association only; exact claim fit remains to be checked | No exact locator attached to this ID in §§23–25. |
| S83-L01 | Research protocols, falsifiability and normative safeguards | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S84-FM01 | Coherence can coexist with empirical falsity; independent risky predictions are a safeguard (L2335–2339) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S85-FM01 | Novelty is not equivalent to discovery or evidential support (L2341–2345) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S86-FM01 | Energy cost alone is not a complete explanation of behaviour (L2347–2351) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S87-FM01 | Overengineering self-control can create unsustainable burden; prefer the smallest useful intervention (L2353–2357) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S88-FM01 | Clinical problems should not be treated solely as failures of discipline (L2359–2363) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S89-FM01 | Research protocols, falsifiability and normative safeguards | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S90-C01 | Interpretive synthesis and conceptual equation | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S91-C01 | Information-theoretic identities, semantic results, epistemic claims | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |
| S92-C01 | Multilevel causal hypothesis, score model, conditional proposition | E02 | R11–R14 | Cluster association + selected pinpoint; not full source closure | R11–R15 and R24; selected source pinpoints; §§23,25. |
| S93-C01 | Proposed construct, model and capability hypothesis | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | R35–R37, R51 and R54–R55; mixed full/abstract-level access; §23. |
| S94-C01 | Intervention architecture and personal protocol | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | R31–R34, R41, R47–R48; component and method sources; §§23–25. |
| S95-EQ01 | \(S_{t+1}=F(A,M_t,O_t,G_t,\mathcal R_t,\mathcal I(A,M_t),\Pi_t,R_t)\) | — | — | No E01–E15 stable-ID assignment recorded; decide source need by claim kind. | No exact locator attached to this ID in §§23–25. |

### 26.4 Source-access and contrary-evidence controls

1. **Access level is part of traceability.** Preserve distinctions already recorded in §§23–25: full-text/section or equation pinpoints (for example R23, R24, R27, R46, R51, R53 and R54/R57 where stated); section-level text (R29); abstract-level evidence (including R06, R13–R15, R25, R28, R30–R32, R34, R43–R44, R55–R56 and R58); and metadata/review-only or blocked sources (including R07/R08 and blocked full text for R13/R14/R58). Do not promote abstract-only or metadata-only items to full-text verification.
2. **Primary versus secondary evidence.** R13/R14 and several E-cluster reviews/meta-analyses are synthesis sources. Their presence does not complete the primary-study trail. Remaining primary-study mapping is especially important for neural energetics, effort/control, habit paradigms, digital friction, metacognitive interventions, sleep and intelligence measurement.
3. **Contrary and limiting evidence remains visible.** Preserve mixed environmental-intervention findings (R34 and the small field experiment recorded in the E01–E18 adjudication), task-specific and null sleep-domain findings (R44), limited cross-task convergence for habit measures (R53), unexpected maintenance results in the context-planning trial (R30), and the distinction between self-reported strategy use and monitoring accuracy (R54/R55). These qualify relevant claims; they do not constitute blanket refutations.
4. **No direct refutation is established by this matrix.** Several claims are definitions or formal results; some component mechanisms have bounded evidence; multiple proposed mechanisms, coefficients and integrated packages remain untested; and some claims lack claim-specific source mapping. “Not established” must not be rewritten as “disproved.”
5. **Non-empirical claims need the right support standard.** Definitions require coherence and operational utility; formal results require valid derivations and fixed semantics; methodological norms require defensible standards or rationale; empirical and causal claims require appropriate primary evidence, design quality and possible falsifiers.
6. **Unmapped rows are an explicit backlog.** For every ID without an E-cluster assignment, decide whether it is (a) a definition/notation/methodological rule needing no empirical source, (b) a formal claim needing a formal reference and proof check, (c) a model needing comparator/identification evidence, or (d) an empirical claim needing primary evidence. Do not fill gaps by assigning a source merely because it appears in the same section or discusses a neighbouring construct.

### 26.5 Claim-level disposition priorities derived from the matrix

- **Highest source-risk:** physical-to-cognitive bridge and action-score coefficients (S16/S18/S19/S20/S31/S92); proposed intelligence functional (S32); habit recurrence and construct validity (S21/S22/S34/S35/S42/S56); distinct Recursive Intelligence (S46–S50/S93); ROOT efficacy and local intervention effects (S41/S43/S54/S55/S79/S80/S94); sleep/fatigue and causal interpretation (S37/S67/S78); and unified state/controller model (S03/S46/S60–S64/S71/S74/S95).
- **Formal-proof priority:** S10-TH01, S11-TH01, S20-P03, S26-TH03, S62-P05, S73-TH04 and S74-TH05. Their dependencies are summarized in §22.3; the remaining task is exact proof-to-premise checking and controlled correction, not citation accumulation.
- **Source-record priority:** resolve E16–E18 provenance; complete primary-study mapping beneath review-level claims; finish the WHO CDDR category 6C72 page-level check; and verify sources currently classified abstract-only/metadata-only before any claim is upgraded.
- **Novelty/alternatives priority:** compare exact proposed mechanisms and measurable outputs—not labels—with EVC, model-based/model-free control, metacognition/meta-control, adaptive control, habit learning and established behavioural interventions. A neighbouring theory is neither automatic refutation nor evidence of distinctiveness.

**Disposition.** The structural stable-ID inventory is complete and the legacy alias errors are normalized here. The source map is **partially reconciled, not exhaustive at the level of direct source-to-claim support**. No claim is upgraded by cluster association; E16–E18 remain unresolved; contrary/negative findings remain attached to their limited scopes. This is a traceability audit, not the final claim-level source disposition or independent review. No treatise or tracker edits; no experiments executed or authorized.

## 27. First-pass source-requirement triage for claims without an E-cluster assignment

**Purpose.** Section 26 identified stable IDs without a direct E01–E15 cluster assignment. This section does not add speculative citations. It classifies what kind of verification each unmapped item needs before it can receive a final disposition. Classification is based on the registered claim label and stable-ID type, and is therefore a triage result—not a completed source audit.

**Coverage.** 145 stable IDs have no E01–E15 assignment in Section 26. The remaining IDs already have one or more cluster-level associations. A source requirement is determined by the claim's actual content, not by the suffix alone.

### 27.1 Formal and semantic verification required

These items primarily require a fixed formal language, definitions, valid derivation, model assumptions or a suitable formal reference. Empirical sources are not a substitute for proof validity.

S02-C01, S03-EQ01, S03-EQ02, S03-EQ03, S03-EQ04, S03-EQ05, S07-C01, S07-P01, S07-P02, S09-C01, S09-C02, S12-C01, S16-EQ01, S16-EQ02, S17-EQ01, S18-EQ01, S20-P03, S21-EQ01, S23-EQ01, S24-C01, S25-C01, S25-EQ01, S26-TH03, S28-EQ01, S28-EQ02, S29-EQ01, S29-P04, S30-EQ01, S30-EQ02, S31-EQ02, S32-EQ01, S32-EQ02, S36-EQ01, S36-P01, S37-EQ01, S43-EQ01, S45-EQ01, S46-EQ01, S49-EQ01, S54-EQ01, S57-EQ01, S60-M01, S61-EQ01, S61-M01, S33-C01, S62-P05, S64-EQ01, S71-EQ01, S71-EQ02, S73-C01, S74-TH05, S90-C01, S91-C01, S95-EQ01

### 27.2 Model specification, identification or validation required

These items require typed variables, state/action spaces, units, transition or update rules, identifiability/observability analysis, parameter estimation where applicable, and comparison against simpler or established models. A citation to general control or learning theory does not validate the proposed instance.

S01-C01, S03-M01, S19-M02, S26-M01, S49-C01, S52-C01, S57-C01, S59-C01, S06-C01, S06-C02, S12-C02, S13-C01, S14-C01, S17-C01, S19-C01, S28-C01, S29-C01, S31-M01, S32-C01, S38-C01, S39-M01, S41-M01, S44-C01, S45-C02, S47-C01, S48-C01, S52-M01, S59-M01, S60-C01, S62-C01, S63-C01, S70-C01, S71-C01, S72-C01, S74-C01, S93-C01, S94-C01

### 27.3 Empirical evidence or primary-source mapping required

These items make or summarize claims about development, neural/behavioural mechanisms, learning, effort, prediction, intervention effects, or other phenomena. They require a source that matches the population, task, outcome and causal strength of the wording; review-level citations may orient the search but cannot substitute for primary evidence where a specific mechanism or causal effect is claimed.

S13-C02, S16-C02, S17-C02, S18-C02, S18-C03, S20-C01, S21-C02, S22-C01, S23-C01, S23-C02, S27-H01, S27-H08, S34-C01, S35-C02, S40-C01, S41-C02, S42-C01, S58-C01, S68-C01

### 27.4 Definition, taxonomy, methodological or normative clarification required

These items are principally definitions, classifications, research questions, scope boundaries or methodological rules. They do not all require an empirical citation. They do require internal consistency, non-circular operational definitions, explicit scope, and—where a standard or normative recommendation is invoked—a traceable rationale or authoritative methodological source.

S01-C02, S01-Q01, S02-C02, S02-C03, S02-D01, S15-F01, S05-D01, S05-D02, S05-D03, S05-D04, S05-D05, S05-D06, S05-D07, S05-D08, S08-C03, S39-C01, S50-C01, S51-C01, S53-C01, S64-C01, S75-C01, S83-L01, S84-FM01, S85-FM01, S86-FM01, S87-FM01, S88-FM01, S89-FM01

### 27.5 Mixed-status axioms and foundational premises

S04-A02, S04-A03, S04-A04, S04-A05, S04-A06, S04-A07, S04-A08

The axioms must not be treated as a homogeneous formal axiom set. Their verification requirements differ: physical embodiment is a well-established physical premise; structural/contextual dependence and contextual acquisition contain broad conceptual and empirical generalizations; internal transformation and adaptive selection need formal operational definitions plus domain evidence; bounded resources need construct/measurement scope; recursive accessibility and fallible model–world correspondence require narrower definitions and appropriate cognitive/epistemic support. The existing Section 22 premise map remains controlling.


### 27.6 Triage limits and next checks

1. The categories above are **source-requirement classes**, not support ratings. An item in the empirical group is not thereby unsupported in the wider literature; it is simply not linked to a cluster in the current map.
2. Some labels are grouped summaries or repeat a construct across sections. Before source assignment, compare the full claim text and exact treatise line range; do not cite a whole cluster to a repeated summary without checking what it adds.
3. A model may need both formal and empirical verification. For example, a softmax equation can be mathematically valid while its use as a behavioural choice model remains empirically unvalidated.
4. The next claim-level pass should process empirical claims first where a factual/causal assertion is made, then model-bearing claims, then formal results, and finally definitions/normative rules. This ordering prioritizes the largest risk of overstated real-world conclusions while preserving proof validity as a separate audit.
5. The E16–E18 provenance issue remains open. No recovered source-map artifact has yet supplied an auditable definition for those clusters. No new cluster should be fabricated to make the numbering continuous.


### 27.7 Candidate source routing for the remaining empirical claims

The following are candidate records to inspect—not adjudicated support. They identify where the existing bibliography offers a plausible starting point and where new primary evidence may still be needed.

| Stable ID | Candidate existing source records | Required check / likely gap |
|---|---|---|
| S13-C02 | R01, R21–R22 | Clarify whether the statement concerns statistical prediction, algorithmic inference or actual-world prediction; information/complexity sources alone do not establish predictive utility. |
| S16-C02 | R01, R09, R20 | Verify construct distinctions among thermodynamic entropy, Shannon entropy, variational free energy and psychological effort; keep formal definitions separate from empirical claims. |
| S17-C02 | R09, R11–R14 | Separate physical computation cost, neural signalling cost, baseline metabolism and incremental task energy; primary human task-level evidence remains limited. |
| S18-C02 | R11–R14 | Existing evidence supports energetic demand and baseline costs, not necessarily the exact process allocation or budget decomposition in the treatise. |
| S18-C03 | R14–R15, R24–R26 | Check task-specific control demand and effort; avoid treating subjective effort, fatigue and neural energy as interchangeable. |
| S20-C01 | R15, R24, R26 | Cost-sensitive selection is a plausible comparator; test the exact long-term-goal versus familiar-action claim and its boundary conditions. |
| S21-C02 | R16, R18–R19, R26, R53 | Distinguish cached action values, stimulus-response habits and context-dependent persistence; primary paradigm-specific evidence needed. |
| S22-C01 | R16, R18–R19, R28–R30, R53 | Verify cue–action–outcome learning and whether the proposed generalization is supported across task types. |
| S23-C01 | R16, R18–R19, R28–R30, R53 | Separate model-free learning, habit automaticity and response readiness; the exact recurrence is not validated by these sources. |
| S23-C02 | R17–R18 | Relief is not sufficient to demonstrate negative reinforcement; verify response–consequence contingency and subsequent response-probability change. |
| S27-H01 | R13–R15, R23–R26, R29 | Treat the listed influences as candidate factors, not an established causal ranking; each requires construct-specific measurement and relevant primary evidence. |
| S27-H08 | R30, R33–R34 | Context and friction interventions are local evidence; distinguish action reduction, urge persistence and maintenance. |
| S34-C01 | R16, R18–R19, R28–R30 | Establish the exact learning outcome and whether cue–action–outcome pairing predicts later readiness in the specified context. |
| S35-C02 | R15, R24–R26 | Arbitration factors are theoretical/computational candidates; verify task-dependent effects and distinguish model-based/model-free constructs. |
| S40-C01 | R16–R19, R23–R26 | This is a synthesis row; each of its five component propositions needs its own evidence scope, not one blanket citation. |
| S41-C02 | R31–R34, R48 | Evidence for implementation intentions and environmental interventions does not validate the combined intervention or sustained-attention claim. |
| S42-C01 | R16, R18–R19, R28–R30, R53 | Review each recurrence and learning mechanism separately; resolve the §42/§56 equation conflict before any empirical parameterization. |
| S58-C01 | R25, R43–R44, R30 | Sleep effects are domain- and exposure-specific; activity/context planning evidence does not validate a universal optimization package. |
| S68-C01 | R15, R24, R31–R32, R48 | Task decomposition and implementation intentions are plausible neighbouring methods; a direct source for initiation-cost reduction in this exact formulation is still required. |

**Routing conclusion.** Several “empirical” IDs are actually model summaries, taxonomies or operational schemas and have been moved to the corresponding formal/model/definition groups above. The remaining 20 rows are the narrower empirical-source queue. Candidate R records must be read against exact claim wording before a source-to-claim link is accepted.


**Disposition.** The 145 unmapped IDs have been triaged by verification requirement; none is promoted to supported, contradicted or rejected by this classification. Direct source-to-claim matching and final dispositions remain open. No treatise/tracker edits; no experiments executed or authorized.


## 28. Claim-level source adjudication — cost-sensitive choice, habit measurement and digital friction

This section closes selected source-to-claim checks for the highest-risk empirical rows in §27.7. It is not a final disposition of all 19 empirical claims.

### 28.1 Cost-sensitive choice and arbitration

**Claims:** S20-C01, S35-C02, with related synthesis claims S27-H01 and S40-C01.

- R15 is a primary two-experiment study, not a general theory validation. It supports a specific task-sensitive allocation result: participants increased model-based control when the task gave it a performance advantage and incentives made that advantage more valuable; they did not increase it merely because stakes rose in a task where model-based control did not improve reward.
- The second experiment is important limiting evidence against an incentive-only heuristic. However, the paper itself notes that the two task structures differed in several ways, leaving some task-structure moderation unresolved.
- This is evidence for a neighbouring model-based/model-free arbitration account. It does not establish the treatise's broader six-factor weight function, the physical/energetic meaning of its cost terms, the exact scalar Q(a) decomposition, or the proposed person's behaviour.
- **Disposition:** component-level support for task-specific arbitration; no direct validation of the treatise's exact action score or personal causal explanation. Keep S20-C01 conditional and S35-C02 as a candidate factorization pending operational measurement and model comparison.

### 28.2 Habit learning and construct validity

**Claims:** S21-C02, S22-C01, S23-C01, S34-C01, S42-C01, with related S27-H01 and S40-C01.

- R19 provides a substantial registered-report study (N = 220; task-specific analysis samples N = 213 and N = 208) that separates frequency-based choice repetition from several value-based habit operationalizations.
- Its positive frequency-based findings in two paradigms support the limited possibility that repeated choice frequency can bias later choice/habit-related measures, including in a task without external reinforcement as operationalized by the authors.
- Its negative findings are equally material: the six habit paradigms did not converge on one common latent habit construct, and none of the tested task measures showed criterion validity against real-life habit questionnaires in this sample. The study's convenience sample and long multi-session protocol constrain generalization.
- R19 also cautions against equating model-free reinforcement learning with established habits: the authors discuss the distinction between outcome-independent habit and reward-dependent model-free learning (lines 56–62). R53 independently found limited convergence in a smaller task comparison; the two studies should not be collapsed into a single universal estimate.
- R16 supplies formal reinforcement-learning algorithm definitions; R18 is a review of reward/decision systems. Neither by itself establishes that the treatise's §42/§56 recurrences measure one common habit-strength construct.
- **Disposition:** bounded evidence for frequency-related and task-specific habit-like effects; contrary evidence against interchangeable habit measures and universal model-free/habit identity. The treatise's habit equations remain unvalidated and internally unreconciled.

### 28.3 Relief and negative reinforcement

**Claim:** S23-C02.

- R17's authoritative definition requires a response-contingent removal, prevention or postponement of an aversive stimulus and a subsequent increase in the response's probability. A temporary reduction in discomfort alone is not sufficient.
- The current treatise wording “can reinforce” is appropriately conditional, but the empirical claim requires observing the response–consequence contingency and subsequent behaviour. A diary entry showing relief after avoidance does not establish negative reinforcement.
- **Disposition:** retain only as a candidate mechanism until contingency and later response change are measured. Do not infer reinforcement from relief alone.

### 28.4 Digital friction and environmental obstruction

**Claims:** S27-H08 and S41-C02, with related S41-C01, S43-C01, S54-C01 and S79-EXP-D.

- R33's preregistered N = 112 field experiment found grayscale reduced objectively measured screen time by about 50 minutes/day relative to self-monitoring control; time-limit goal setting did not significantly differ from control. Reduced screen time had no immediate causal effect on subjective well-being or academic performance. The endpoint was device screen time, not sustained attention.
- R34's N = 97 one-week experiment found objective use reductions in intervention and control groups, while self-reported problematic use increased. This highlights measurement awareness and weakens a simple causal reading of pre/post change.
- Together these studies support the narrower proposition that specific environmental friction can sometimes reduce a measured digital-use outcome. They do not establish a general effect on unwanted actions, urge intensity, attention, habit extinction, or ROOT efficacy.
- **Disposition:** retain as context-specific intervention hypotheses; do not generalize screen-time effects to attention or self-mastery. Any future claim test must measure both behaviour and relevant functional outcomes, with eligible-opportunity denominators and substitution monitoring.

### 28.5 Updated claim-source assignments and remaining gaps

| Stable ID | Source assignment after this pass | Evidential boundary |
|---|---|---|
| S20-C01 | R15, R24, R26 | Task-specific cost-benefit arbitration; no universal/person-specific causal claim. |
| S21-C02 | R16, R18–R19, R53 | Habit/model-free distinction and weak cross-paradigm convergence. |
| S22-C01 | R16, R18–R19, R28–R30, R53 | Cue/action/outcome learning; no single universal habit construct. |
| S23-C01 | R16, R18–R19, R28–R30, R53 | Learning mechanisms differ; equations remain unvalidated. |
| S23-C02 | R17–R18 | Negative reinforcement requires contingency and subsequent response increase. |
| S27-H08 | R30, R33–R34 | Context/friction effects are outcome- and setting-specific. |
| S34-C01 | R16, R18–R19, R28–R30 | Later response readiness requires precise operationalization. |
| S35-C02 | R15, R24–R26 | Arbitration factors are candidate constructs, not established coefficients. |
| S41-C02 | R31–R34, R48 | Component intervention evidence; no ROOT or sustained-attention validation. |
| S42-C01 | R16, R18–R19, R28–R30, R53 | Habit recurrence/strength remains unvalidated. |
| S27-H01 | R13–R15, R23–R26, R29 | Candidate-factor list; no established causal ranking. |
| S40-C01 | R16–R19, R23–R26 | Composite synthesis must be split into its component claims. |

**Disposition.** Selected empirical-source checks are now at full-text/abstract-verified levels for R15, R19 and R33, and the exact scope of R34 remains bounded as recorded in §23. These findings narrow several claims but do not validate the integrated architecture. The remaining empirical queue—especially neural energy allocation, task uncertainty/effort, sleep/activity optimization and task decomposition—still needs claim-specific primary evidence. No treatise or tracker edits; no experiments executed or authorized.


## 29. Historical evidence-cluster provenance recovery and claim-level adjudication — neural energetics, effort, sleep and task initiation

### 29.1 Recovery result for E16–E18

The historical evidence-to-claim adjudication commit `1b3ba58bc19d2c936c1237013b2c051915afb790` contains a detailed source-level discussion that explicitly groups **E02/E12/E16** with neural energetics and physical-to-cognitive bridge claims (S16/S18/S24/S31/S92, with related effort claims S19/S35–S37). It records the following boundaries: Attwell & Laughlin (R11) is a rodent grey-matter model-based estimate; Raichle & Gusnard (R12) emphasize high baseline energy and relatively small transient task changes; Kondrakiewicz & Nawrocka (R13) review evidence of minimal/no whole-body energy increase for many cognitive tasks; Otto et al. (R14) describe the experienced effort-cost mechanism as unsettled; and Shenhav et al. (2017) identify unresolved questions in control allocation.

This recovers **partial provenance for E16**, but not a complete cluster definition or a verified source-to-claim map. The same historical diff refers to a short identifier `4b6c2e6` as a future commit (“to be assigned”); it does not provide a full commit SHA. The accessible `edition` branch history for the register does not expose a corresponding full-SHA artifact. It is therefore not admissible as a committed source-map record.

**E17 and E18 remain unrecovered.** The historical adjudication summary names E01–E18 collectively but supplies no independently auditable definitions, source inventories or stable-ID mappings for E17/E18 in the records located. No labels or mappings are inferred from numbering, adjacency or the E16 discussion. The register's E01–E15 crosswalk remains the only normalized cluster map. E16 is recorded as a partial historical evidence cluster; E17/E18 remain provenance gaps.

### 29.2 Claim-level adjudication of remaining high-risk empirical rows

| Stable ID | Evidence examined / access level | What the evidence supports | What it does not establish | Provisional disposition |
|---|---|---|---|---|
| S13-C02 | R01, R21–R22: formal/theoretical records already in the register; no claim-matched empirical primary study closed in this pass | Depending on the intended meaning, formal inference and statistical prediction can be described with established mathematical tools | That a particular inference predicts an unobserved actual-world state, or that the proposed framework improves prediction | Split the statement into (i) inference from premises, (ii) statistical prediction against held-out outcomes and (iii) discovery/actual-world truth. Defer any predictive-performance claim pending an explicit target, baseline and validation set |
| S16-C02 | R01, R09, R20: formal/conceptual source trail; no new empirical validation needed for definitions | The relevant constructs can be distinguished at the level of definitions: thermodynamic entropy, Shannon information, variational free energy and subjective effort are not interchangeable quantities | A conversion between them, a shared unit, or a causal equivalence between information processing and experienced effort | Retain only as a construct-separation requirement; specify each quantity's domain, units and mathematical role. Do not present a cross-domain equivalence |
| S17-C02 | R11–R14: R11 model-based rodent estimate; R12 baseline-energy discussion; R13 review abstract; R14 review abstract | Neural signalling has energetic costs; baseline brain metabolism is substantial; current reviews caution that many cognitive tasks produce little or no measurable whole-body energy increment | A human per-inference/per-thought cost, a task-specific energy coefficient, or the treatise's proposed allocation of energy across cognitive operations | Narrow to the physical/neural energetic premise. Defer process-level allocation and all behavioural coefficients until directly measured in an appropriate human task design |
| S18-C02 | R11–R14: mixed model/review evidence, with R13/R14 abstract-level access in the recorded audit | Neural energetic demand and the distinction between baseline and task-related change are legitimate topics for a multilevel account | The exact process-budget decomposition or mapping from neural energy to a person's cognitive effort | Revise as a research hypothesis with separately typed neural, whole-body and subjective measures; no empirical validation of the proposed decomposition |
| S18-C03 | R14–R15, R24–R26: R14 abstract-level review; R15 full-text primary experiments; R24 full-text theoretical comparator; other records at their registered access levels | Task structure and expected performance benefit can influence model-based/model-free control allocation in the R15 paradigms; EVC supplies a close cost-sensitive control framework | A universal effort law, a measured physiological-energy explanation, the exact six-factor weights, or the personal causal account in the treatise | Retain as a bounded task-sensitive control hypothesis; distinguish effort report, control demand, fatigue and metabolic cost. Exact action-score terms remain unvalidated |
| S58-C01 | R25, R43–R44: sleep meta-analyses/reviews at abstract-level in the recorded audit; R30 randomized context-planning study at abstract-level | Sleep loss/restriction can impair selected outcomes, especially sustained attention; effects vary by exposure and cognitive domain. R44 reports null pooled effects for several domains. R30 shows that context planning and maintenance need not move together | A universal sleep/activity optimization function, a single-night general cognitive impairment claim, or causal efficacy of the treatise's combined optimization package | Split by exposure, outcome and time horizon. Retain domain-specific sleep effects; defer the optimization package and any universal ranking |
| S68-C01 | R15/R24 and R31–R32: task-control comparator plus implementation-intention meta-analysis/mechanism study; no direct source for the exact initiation-cost formulation closed | Specific plans and cue–response associations can support action initiation in some contexts; task decomposition is a plausible design hypothesis | A general reduction in subjective initiation cost or uncertainty from any arbitrary “first action,” across tasks and populations | Retain as a testable heuristic, not a universal empirical law. Define initiation latency, eligible opportunities, task difficulty and a comparator before claiming an effect |

### 29.3 Cross-claim conclusions and evidence boundaries

1. **Physical-to-cognitive bridge:** the evidence supports the existence of physical implementation and neural energetic costs. It does not bridge those facts to subjective effort, fatigue, action selection or the treatise's coefficients without intermediate constructs and direct measurements. These are separate dependent variables, not synonyms.
2. **Effort and control:** R15's task-sensitive allocation finding and R24's EVC framework are relevant comparators. They reduce any novelty claim based only on combining reward and cost, but they neither refute nor validate the exact proposed model. Incremental predictive value must be tested against these baselines.
3. **Sleep and cognition:** total sleep deprivation, multi-night restriction and one-night partial restriction must not be pooled as if they were one exposure. Null results in choice reaction time, throughput, working memory or inhibitory control remain part of the evidence, not noise to omit.
4. **Task initiation:** implementation intentions and cost-sensitive control are adjacent mechanisms. They do not directly verify the treatise's specific “concrete first action reduces initiation cost and uncertainty” proposition.
5. **Access discipline:** R11/R12 are model/review-level sources, R13/R14/R25/R30/R43/R44 are recorded as abstract-level in the prior audit, and R15/R24 have full-text inspection. No abstract-only record is described here as a full-text reanalysis; no review-level finding is mislabelled as a new primary experiment.
6. **Disposition discipline:** “not directly supported by the mapped evidence” means unresolved or insufficiently tested, not disproved. No new claim is marked established or refuted in this section.

### 29.4 Remaining work after this pass

- Recover a full-SHA historical source artifact, if one exists, for the E16 adjudication and any E17/E18 definitions; otherwise preserve the provenance gap explicitly.
- Complete primary-study mapping beneath the review-level neural-energy and sleep records.
- Resolve the intelligence-measurement queue (S32) through a construct-validity and criterion-validation audit; the current R27 standards and R58 theoretical article do not validate the treatise's functional.
- Continue the remaining model/empirical rows, then conduct a final direct source-to-claim audit across all 204 IDs. The matrix in §26 remains a routing inventory, not a completed 204-claim adjudication.

**Disposition.** This pass partially recovers E16's historical subject matter and explicitly leaves E17/E18 unresolved. It narrows seven high-risk claim IDs without upgrading their evidence status. No treatise or tracker edits; no experiments executed or authorized.


## 30. Claim-level intelligence construct and measurement audit — S32

### 30.1 Claim decomposition and type separation

The baseline text at §32 (L1057–1104) contains four distinct claim types that must not be collapsed:

- **S32-C01 — conceptual distinction:** intelligence requires functional properties beyond the mere execution of a fixed state transformation. This is a framework-selected definition, not a universally accepted necessary-and-sufficient definition.
- **S32-EQ01 — computational abstraction:** computation is represented as state transformation. This is a broad modelling shorthand, not a complete account of every theory of computation.
- **S32-EQ02 — operational definition:** intelligence is adaptive use of state transformation to model, predict or control under changing conditions. This is stipulative and overlaps adaptive intelligence, learning, adaptive control and meta-control.
- **S32-M01 — measurement proposal:** a weighted composite of generalization (G), adaptation to changed conditions (A_d), predictive accuracy (P), transfer (T_r), and recovery/correction after error (R_c). This is a proposed index, not a validated psychometric instrument.

The five dimensions are plausible capability domains, but their inclusion in one formula does not establish that they form a single latent trait, are mutually discriminable, exhaust intelligence, or should be linearly additive. The score may instead be a **formative decision index** whose components jointly define a chosen capability profile. That measurement model must be decided explicitly; reflective latent-variable assumptions and formative-composite assumptions imply different validation procedures.

### 30.2 Source adjudication and established comparators

- **R27 — AERA/APA/NCME Standards (2014):** the authoritative measurement standard already registered in §23. The relevant principle is that validity concerns the interpretation and use of scores, supported by evidence appropriate to the intended construct, population and decision. The standards do not confer validity on an untested formula.
- **R58 — Sternberg (2019):** the article is a theoretical account distinguishing adaptive intelligence from psychometric general intelligence and emphasizing biological/evolutionary and cultural context. It establishes that the broad adaptive-intelligence territory has a developed theoretical neighbour; it is not a validation study for the treatise's five terms or weights. The full article is now available through the indexed open-access record, but the earlier audit only verified metadata and abstract; detailed page/section mapping remains open.
- **R59 — McGrew (2023):** the article provides a major psychometric comparator through Carroll's three-stratum and CHC cognitive-ability work. It reports exploratory and confirmatory analyses of an archived 46-test Woodcock–Johnson III dataset and psychometric-network analyses linking cognitive and achievement composites. The paper reports a dominant g factor alongside broad abilities in the analysed dataset, while also discussing model alternatives and structural interpretation. Its data are proprietary and the author declares a financial conflict involving the WJ III/IV batteries. It is a secondary analysis/research article, not a new independent validation sample for S32-M01.
- **R59 qualification:** the reported analyses do not prove that g is the only meaningful construct or that CHC is a final, uncontested taxonomy. They do show that a new intelligence score must compare itself with established multidimensional and hierarchical psychometric models, and must state exactly what incremental explanatory or predictive value it adds.

### 30.3 Component-level operational requirements

| Component | Minimum operationalization required | Main validity threat |
|---|---|---|
| G — generalization | Performance on prespecified held-out items, tasks or environments that differ from training examples; quantify distance from training distribution | Memorization, near-transfer mislabeled as generalization, task leakage |
| A_d — adaptation | Performance and learning trajectory after a controlled change in task rules, environment or constraints; include adaptation cost and recovery time | Confounding adaptation with baseline ability, prior familiarity or extra practice |
| P — predictive accuracy | Prospective predictions made before outcomes, with defined target, horizon, calibration and proper scoring rule; evaluate on held-out cases | Retrospective explanation, target leakage, accuracy without calibration or base-rate comparison |
| T_r — transfer | Separate near and far transfer; specify source/target task distance and retention interval; compare with matched practice controls | Rebranding task similarity or repeated practice as transfer |
| R_c — recovery/correction | Error detection, post-error correction, recovery latency, resumed-task accuracy and functional cost; measure whether the system updates its strategy appropriately | Rewarding speed while ignoring accuracy, or treating any post-error change as learning |

These are candidate operational requirements, not an approved test battery. Each component needs multiple appropriately sampled tasks and repeated observations where the construct is expected to generalize beyond one task.

### 30.4 Composite-score and validation defects to resolve

1. **Construct model:** decide whether the five terms are reflective indicators of a common latent capability, formative components of a designed index, or separate dimensions to be reported as a profile. Do not use one model's validation logic for another.
2. **Scale and units:** define each component's metric, direction, range, uncertainty and missing-data rule. A weighted sum is uninterpretable if the terms are not commensurately scaled or if normalization changes across populations/tasks.
3. **Weights:** “task-dependent weights” means the score may be context-indexed rather than a stable general intelligence measure. State who/what selects weights, under which objective and constraints, and whether the weights are fixed before evaluation. Do not tune weights on the same outcomes used to claim validity.
4. **Reliability:** estimate component-level measurement reliability and score/profile stability across tasks, raters, occasions and conditions. A single internal-consistency coefficient is not sufficient for a heterogeneous formative composite.
5. **Validity:** provide content representation, response-process evidence, internal structure where relevant, convergent and discriminant relations, criterion relations and prospective predictive validity. Distinguish prediction of cognitive-test performance from real-world adaptive outcomes.
6. **Incremental validity:** compare against psychometric g/CHC measures and relevant specific abilities, plus adaptive-control, learning and metacognitive baselines. The proposed score must improve held-out prediction or decisions at an acceptable cost; merely correlating with existing ability scores is not novelty.
7. **Fairness and invariance:** examine measurement invariance, differential item/task functioning, accessibility, language/cultural context and opportunity to learn. Sternberg's R58 discussion makes cultural context particularly salient for an adaptive-intelligence interpretation.
8. **Independence:** preregister the construct model, tasks, weights, exclusions, outcomes and analysis. Use independent samples or genuinely held-out cohorts for confirmation; avoid selecting tasks and weights after observing validation outcomes.
9. **Utility:** specify what decision the score is intended to improve. A score may be psychometrically coherent yet have no useful incremental decision value; evaluate calibration, error costs and consequences of use.

### 30.5 Claim-level dispositions

| Stable ID | Claim kind | Formal/evidential status | Provisional disposition | Required closure |
|---|---|---|---|---|
| S32-C01 | Conceptual definition | Defensible as the framework's chosen distinction; not a universal definition and not empirically settled by wording alone | Retain as a scoped definition; do not claim definitional consensus or novelty | Compare explicitly with general intelligence, adaptive intelligence, learning and adaptive control; state necessary/sufficient criteria if intended |
| S32-EQ01 | Mathematical/conceptual shorthand | Broad state-transformation abstraction | Retain with scope note | Specify what counts as state, transformation and computation in the intended system class |
| S32-EQ02 | Operational definition | Stipulative; overlapping established constructs | Retain provisionally; add discriminant criteria | State the additional operation or measurable capability that distinguishes the proposed intelligence construct from ordinary adaptive control/learning |
| S32-M01 | Proposed composite measure | No task battery, scoring manual, reliability, norms, weights, invariance or independent criterion/predictive validation is supplied | Defer as a measurement instrument; keep as a research proposal only | Define measurement model, tasks, scales, weights, reliability, fairness, comparator set, independent validation and incremental utility |

**No support upgrade.** R27 supplies validation standards; R58 supplies a theoretical neighbour; R59 supplies an established psychometric comparator. None validates the proposed five-component score. The absence of such validation does not disprove the possibility that a useful adaptive-capability profile or index could be developed.

### 30.6 Research design gate for any future S32 validation

A valid next study would need to be staged rather than jump directly to a weighted scalar:

1. Publish a construct map and item/task blueprint for each of the five dimensions, including exclusions and overlaps.
2. Conduct content review and cognitive-interview/response-process work across the intended populations and cultural/language contexts.
3. Pilot task reliability, difficulty range, ceiling/floor effects, learning effects, test–retest stability and cross-task generalizability.
4. Compare alternative measurement models (correlated dimensions, hierarchical/factor models where justified, and formative composite/profile approaches); report model fit and sensitivity rather than selecting a preferred model solely by fit.
5. Fix weights or the weight-selection algorithm before the confirmatory test; keep a separate development dataset and untouched validation cohort.
6. Evaluate convergent, discriminant, criterion and prospective predictive validity against g/CHC and relevant domain-specific baselines, then test incremental decision utility.
7. Test fairness/invariance and report subgroup-specific uncertainty and failure cases; do not publish a universal scalar if the evidence supports only context-specific profiles.

This is a readiness specification, not an experiment authorization. It does not authorize any A–F protocol or a new S32 study.

**Disposition.** S32 is now source-adjudicated at the level of conceptual scope, established comparators and measurement requirements. The conceptual definition can be retained as a framework choice; the five-term functional remains unvalidated and must not be called a measured intelligence score. No treatise/tracker edits; no experiments executed or authorized.


## 31. Recursive Intelligence distinctiveness audit — §§46–50 and §93

### 31.1 Exact construct in the baseline treatise

The baseline defines Recursive Intelligence as representing aspects of a system's own processing and using those representations to change future operation (§46, L1515–1547; §93). Its formal sketch is:

- self-state estimate: \(\widehat S_t=\mathcal M(S_t,\text{observations})\);
- parameter update: \(\Theta_{t+1}=\Theta_t+\Delta\Theta(\widehat S_t,G_t,\text{error}_t)\);
- changed transition: \(S_{t+1}=F_{\Theta_{t+1}}(S_t,I_t)\).

The loop in §47 describes outcome measurement, self-model update and policy modification. Section 48 requires fallible self-models and prospective testing; §49 supplies a generic discounted objective and policy update; §50 introduces a revisable goal hierarchy. Section 93 summarizes the construct as using representations of one's own operation to change future operation.

This is a coherent candidate description of self-monitoring plus adaptive policy modification. The question is not whether such processes exist; established literatures study them. The unresolved issue is whether the treatise specifies an additional, measurable operation that distinguishes **Recursive Intelligence** from metacognition, meta-control, adaptive control and ordinary reinforcement learning.

### 31.2 Direct comparison with established neighbours

| Neighbouring construct | What the registered evidence describes | Overlap with the treatise | Remaining distinction not yet demonstrated |
|---|---|---|---|
| Metacognition | R36 reviews confidence, uncertainty and self-evaluation; R37 (2026) reviews self-evaluation of cognitive processes and transformations of uncertainty that support control across timescales; R51 distinguishes object-level cognition from meta-level monitoring/control | Estimating one's own state, recognizing error, judging performance and using those judgments to regulate subsequent cognition | The treatise does not yet specify what its self-model represents beyond familiar performance/state estimates, or a unique operation beyond monitoring and regulation |
| Meta-control | R35 describes monitoring controlled processing and regulating underlying control parameters in light of goals and constraints; R39 is a primary human sequential-decision experiment in which reward stakes and transition stability alter the relative benefit/demand of model-based strategies | Changing control parameters or strategy selection in response to feedback, goals, task demands and constraints | R39 does not implement the treatise's explicit self-model, but it demonstrates that dynamic strategy regulation is already an experimentally operationalized construct. The treatise needs a controlled incremental prediction beyond such meta-control |
| Adaptive control / adaptive policy learning | R16 defines standard temporal-difference and reinforcement-learning algorithms; the earlier formal audit identifies adaptive-control and feedback systems as established neighbours | Updating parameters or policies from error, reward and observed system performance | A parameter update \(\Theta_{t+1}=U(\Theta_t,\text{feedback})\) is not distinctive recursion by itself. The update rule, controller class and target need formal definition |
| Model-based/model-free arbitration | R15 and R39 show task- and incentive-sensitive adjustment between decision strategies | Selecting or weighting internal strategies according to expected benefit, cost and task structure | This is strategy arbitration, not necessarily a model of one's own learning/update mechanism. The treatise must show what extra state or operation it adds |

**Evidence boundary.** R35/R36/R37/R51 are reviews or conceptual syntheses; R39 is a primary human experiment with a specific sequential-decision task and cross-sectional age comparison. These sources establish close neighbours and concrete operational precedents. They do not establish that Recursive Intelligence is identical to those constructs, nor do they prove that the proposed construct is impossible or redundant. They do show that the present wording is not yet sufficient to support a novelty claim.

### 31.3 Formal audit of the proposed recursive equations

1. **Estimator input leakage:** \(\widehat S_t=\mathcal M(S_t,\text{observations})\) appears to provide the estimator with the true state \(S_t\), even though the purpose of an estimator is to infer a potentially latent state from observations/history. Replace the true-state input with an explicitly available observation/history object unless the state is directly observable by definition.
2. **Unspecified self-model target:** “aspects of its own processing” could mean performance, confidence, policy, memory, learning rate, controller parameters, resource use or the update mechanism itself. These are different target variables and require separate operational definitions.
3. **No explicit second-order update:** the current \(\Delta\Theta\) changes behavioural parameters, but the treatise does not define an update to the rule that computes \(\Delta\Theta\), its learning rate, model class, error weighting or update policy. Without this, the equations express ordinary adaptive/meta-control, not a demonstrably higher-order recursion.
4. **Generic objective:** the discounted return in §49 is standard reinforcement-learning notation. The treatise correctly says human self-regulation need not literally implement gradient descent, but the conceptual \(\widehat{\nabla J}\) still needs an estimator and policy-update semantics if it is to be tested.
5. **Goal hierarchy:** §50 introduces a normative hierarchy of immediate, task, daily, long-term and identity/value goals. It does not define a measurable cognitive operation or show that higher-level goals are ordered by a single relation. It should not be used as evidence that a recursive mechanism exists.
6. **Circular validation risk:** if a system's own explanation of why it failed is both the estimator input and the criterion for successful self-modeling, the test is circular. Section 48 correctly points toward independent observable outcomes and prospective controlled predictions; this safeguard must become an actual evaluation protocol.

### 31.4 Candidate discriminator required before claiming a distinct construct

A possible discriminator—not yet established by the treatise—is an explicit model of the system's **own update process**, not merely a model of its current performance or control state. Such a proposal would need to specify:

- object-level state and policy, including the ordinary adaptive controller;
- meta-level estimates of the controller's own update rule, uncertainty, learning rate, model class or update reliability;
- a distinct meta-update that changes how future object-level updates are selected or evaluated;
- a measurable consequence that cannot be reproduced by ordinary metacognitive monitoring, meta-control or adaptive control under matched information, capacity and feedback;
- a falsifier: if the nested representation/update adds no held-out predictive or control benefit over the simpler baselines, the distinct-construct claim is not supported.

This is a candidate route to discriminant validity, not a recommendation to add a “meta-meta” layer merely to preserve novelty. If no non-arbitrary, useful discriminator can be defined, the more accurate treatment may be to present Recursive Intelligence as an integrative label or design architecture built from established metacognitive/meta-control processes, rather than as a newly demonstrated cognitive mechanism.

### 31.5 Required comparative evaluation (not authorized for execution)

Any future validation should compare at least four capacity-matched systems on the same tasks and held-out environments:

1. object-level learning/adaptive control without self-monitoring;
2. metacognitive monitoring and confidence calibration;
3. meta-control that adjusts strategy/control parameters using task demands and feedback;
4. the proposed recursive architecture with its explicitly specified self-model and meta-update.

Predefine outcomes such as adaptation sample efficiency, held-out transfer, post-error recovery accuracy and latency, calibration, robustness to misleading self-assessment, and resource/burden cost. Use ablations to remove the self-model and the meta-update separately. Compare against established model-based/model-free arbitration and simple fixed/adaptive policies. Complexity and information access must be controlled; otherwise an apparent gain may come from additional computation or feedback rather than recursion. The study must be preregistered and independently validated. This is a design requirement only; no experiment A–F is authorized or executed.

### 31.6 Claim-level dispositions

| Stable ID | Provisional disposition | Required closure |
|---|---|---|
| S46-M01 / S46-EQ01–EQ03 | Retain as a candidate self-model/adaptive-parameter architecture; downgrade any claim of a distinct mechanism | Correct estimator inputs; define latent/observed state, model target, update rule, constraints and measurable meta-level operation |
| S47-M01 / S47-C01 | Retain as a feedback-loop description; do not treat the loop as proof of unique recursion | Identify what is added beyond standard feedback, adaptive control and meta-control; specify stages and typed interfaces |
| S48-C01 / S48-C02 | Retain as a methodological safeguard | Pre-register prospective predictions and evaluate them against independent outcomes and competing explanations |
| S49-M01 / S49-EQ01–EQ02 / S49-C01 | Retain the objective as a generic policy-learning formulation; do not attribute literal gradient descent to humans | Specify state/action/reward/harm semantics, estimator, policy class, update algorithm and comparator |
| S50-M01 / S50-C01 | Retain as a normative goal-organization proposal, not a cognitive mechanism | Define priority/abstraction/authority relations, incomparable goals and legitimate revision constraints |
| S93-C01 | Retain as a high-level construct hypothesis; novelty and distinctness remain unestablished | Provide the operational discriminator and demonstrate incremental explanatory/predictive/control value against metacognition, meta-control and adaptive-control baselines |

**Disposition.** The existing evidence establishes substantial neighbouring constructs and at least one direct human experimental precedent for meta-control. The treatise's current equations and loop do not yet identify a unique recursive operation or demonstrate incremental utility. The construct should remain a provisional synthesis/hypothesis, not a validated new intelligence mechanism. No treatise/tracker edits; no experiments executed or authorized.


## 32. ROOT Control Protocol component evidence and package-efficacy audit — S41/S43/S51/S54/S55/S79/S80/S94

### 32.1 Scope and outcome definition

The baseline §94 defines ROOT as seven operations: Recognise the trigger; Obstruct the automatic pathway; Override with a specific alternative; Train the replacement; Correct using outcome data; Optimise biological/environmental conditions; Learn and consolidate. The stated aim is not elimination of impulses, but increasing the probability that chosen objectives govern behaviour despite competing signals.

This is a **proposed multicomponent behavioural intervention architecture**. Evidence for one component does not establish the efficacy of the sequence, the full package, the proposed causal order, or superiority over a simpler intervention. The seven-stage acronym also needs clarification: the first four stages spell ROOT; the remaining stages add COL. Unless the seven-step name is intentionally ROOTCOL, the mnemonic and protocol taxonomy are not aligned.

The primary outcome cannot be “fewer urges” alone. A valid evaluation should measure goal-concordant action at eligible opportunities, while separately recording urge intensity, cue exposure, obstruction fidelity, alternative response, recovery latency, task accuracy/functional output, substitution to other behaviours, burden and adverse effects. A lower target-action count caused by fewer opportunities, avoidance of the task or displacement to another behaviour is not necessarily improved self-regulation.

### 32.2 Component-level evidence map

| ROOT operation | Relevant registered sources | Bounded evidence | Missing evidence for the ROOT claim |
|---|---|---|---|
| Recognise | R42 EMA/self-report measurement; R27 testing/measurement standards | Repeated measurement can describe context and behaviour; measurement quality and construct definition matter | No evidence that the proposed trigger taxonomy is exhaustive, reliable or sufficient to identify causal triggers. Self-report alone can be reactive and error-prone |
| Obstruct | R33 randomized grayscale field experiment; R34 one-week obstruction field experiment | R33 found a context-specific reduction in objectively measured screen time for grayscale versus control; R34 found objective use fell in intervention and control groups while self-reported problematic use increased | No general effect on all unwanted actions, urge intensity, sustained attention, habit extinction or ROOT efficacy. Substitution and opportunity denominators remain necessary |
| Override | R31 implementation-intention meta-analysis; R32 cue-accessibility/cue-response mechanism study; R48 2024 meta-analysis of 642 tests | If–then plans and rehearsed cue–response mappings can improve goal attainment across studied tasks; R48 reports heterogeneous outcome effects and moderators | Does not show that every alternative is feasible, that a specific person's chosen alternative works, or that override is effective when the cue is not detected or the alternative is obstructed |
| Train | R19 habit-paradigm registered report; R28 Lally et al.; R29 habit-formation review; R30 randomized context-planning trial; R53 habit-measure study | Repetition/context and automaticity can change in some settings; R30 supports a context effect on automaticity for walking | No validated ROOT replacement-training schedule or universal formation duration. Habit measures do not converge reliably; automaticity is not the same as maintenance or functional success |
| Correct | R54 monitoring-accuracy meta-analysis; R55 metacognitive-prompt meta-analysis; R27 testing standards | Metacognitive prompts can improve reported self-regulated-learning activities and learning outcomes; objective monitoring-accuracy effects are smaller (R54 g=0.25) | Does not establish that the proposed personal correction loop accurately identifies causes, avoids metric gaming or improves long-term outcomes. Self-report and objective calibration must remain separate |
| Optimise | R25 total sleep deprivation meta-analysis; R43 sleep-restriction meta-analysis; R44 one-night partial-restriction meta-analysis; R30 context planning | Sleep exposure affects selected cognitive outcomes, especially sustained attention; context consistency can influence a specific walking/automaticity outcome | No validated combined biological/environmental optimization package, universal priority ordering or causal claim that changing sleep/activity/context improves the target behaviour in this protocol |
| Learn and consolidate | R19/R28–R30/R53 for habit and automaticity; R41/R47 for single-case evaluation | Some task-specific automaticity and learning effects are documented; repeated measurement and credible comparison are needed to establish individual change | No evidence that the ROOT sequence consolidates a durable replacement policy or generalizes to novel contexts; no package-level maintenance or relapse-prevention data |

### 32.3 Cross-component limitations and contradictory evidence

1. **Obstruction is not a universal mechanism.** R33's grayscale effect is tied to objectively measured smartphone screen time in its student sample and did not immediately improve well-being or academic performance. R34's control-group decline and increase in self-reported problematic use show that awareness/reactivity and time trends can confound simple before/after claims.
2. **Planning evidence is not ROOT evidence.** R31/R32/R48 support implementation intentions in specified settings. They do not validate the full seven-stage protocol, nor prove that the exact order Recognise→Obstruct→Override→Train→Correct→Optimise→Learn is optimal.
3. **Habit formation is not equivalent to maintenance.** R19/R53 raise construct-convergence and criterion-validity concerns; R29 identifies substantial variability and risk of bias; R30's context-planning intervention increased automaticity, but the consistent-context group unexpectedly did not show the expected walking maintenance. Do not use automaticity as a proxy for durable functional improvement.
4. **Self-correction can be miscalibrated.** R54's objective monitoring-accuracy effect is smaller than broader self-regulated-learning outcome effects, while R55 concerns metacognitive prompts and learning outcomes. Reported strategy use, subjective confidence and objective monitoring accuracy are different endpoints.
5. **Optimization effects are domain-specific.** R25/R43/R44 concern different sleep exposures and outcomes. Null pooled effects in several domains in R44 must remain visible. A generic “optimize biology” stage is too broad to support a single causal claim.
6. **No package comparator exists in the registered evidence.** The current sources do not compare the complete ROOT sequence with usual practice, a minimal single-component intervention, a matched multicomponent intervention, or a component-ablated ROOT version.

### 32.4 Package-level causal and measurement requirements

A future ROOT evaluation must specify, before data collection:

- **Target population and scope:** the behaviour class, setting, age/population, inclusion/exclusion criteria and whether the protocol is a self-management aid or a clinically supervised intervention. Do not generalize across unrelated behaviour classes without replication.
- **Causal model:** stage-specific mechanisms and expected mediators; which stages are necessary, optional, concurrent or sequential; expected lag and carryover; and conditions under which a stage could backfire.
- **Estimand:** probability of goal-concordant action per eligible opportunity, change in functional output, and durability after active support is removed. Keep urges, target-action counts, screen time, automaticity and functional performance as separate outcomes.
- **Opportunity denominator:** count occasions when the target cue/choice was genuinely present and the goal-consistent response was feasible. Log cue exposure, obstruction status, alternative availability and missing opportunities.
- **Comparator:** compare with usual practice and at least one credible simpler intervention. For component attribution, use factorial/dismantling or sequential randomization where feasible; do not compare a well-supported full intervention with a deliberately weak no-support control and call the difference a ROOT-specific effect.
- **Fidelity and adherence:** operational definitions for each stage, actual exposure, user burden, deviations, contamination and co-interventions. A checklist of intended steps is not proof that the steps occurred.
- **Functional and adverse outcomes:** task completion/accuracy, sleep and health impacts where relevant, distress/burden, substitution, rebound, avoidance, and harms from excessive obstruction or rigid goal pursuit.
- **Analysis:** repeated-measures structure, baseline trend, autocorrelation, missingness, carryover, multiple outcomes, uncertainty intervals and pre-specified stopping rules. A pre/post difference alone is not a causal estimate.
- **Maintenance and transfer:** follow-up after active intervention, retention, generalization to new contexts and performance under cue changes; distinguish short-term compliance from a learned durable response.
- **Independent replication:** validate in separate samples/settings before claiming general package efficacy.

### 32.5 Design hierarchy and readiness gate

The 28-day treatise protocol and 14-day tracker pilot remain distinct. The treatise's 7-day baseline + 7-day environmental change + 14-day alternative-response training design is a fixed sequential intervention. It does not isolate stage effects because phase order, time trend and carryover are confounded. The tracker’s 14-day pilot is not equivalent and should not be represented as a shortened validated version.

R41/R47 support the need for repeated outcomes and stronger single-case design features when causal individual-level claims are intended. R49 distinguishes SMART designs for slower adaptive decision points from MRT designs for faster repeated decisions; R50 documents frequent reporting gaps in SMART studies. The choice depends on the ROOT stage timing and the estimand, not on a generic preference for one design label.

**Readiness decision:** the current ROOT protocol is **not ready for an efficacy claim or execution as a causal experiment**. It can be retained as a descriptive planning framework or a hypothesis-generating personal workflow, provided it is not marketed as validated. Any controlled evaluation remains subject to the governing plan's preregistration, comparator, measurement, safety, sample-size and authorization gates. This section does not authorize execution of experiments A–F or any new ROOT trial.

### 32.6 Claim-level dispositions

| Stable ID | Provisional disposition | Required closure |
|---|---|---|
| S41-C01 / S41-C02 | Component-level planning/friction evidence only; sustained-attention and combined-intervention claims remain unestablished | Define attention and goal-concordant behaviour outcomes; isolate intervention components and comparator |
| S43-C01 | Retain as a provisional within-person leverage metric, not a validated effect measure | Define opportunity denominator, counterfactual, setup/maintenance burden and uncertainty |
| S51-C01 | Retain as a named seven-stage proposal; acronym/sequence architecture is unclear | Decide ROOT versus ROOTCOL naming; define stage contracts, sequencing, iteration and required/optional stages |
| S54-C01 / S54-EQ01–EQ02 | Retain as a local, falsifiable accessibility hypothesis | Measure accessibility, target behaviour, opportunity, substitution, task output and causal comparator |
| S55-C01 | Retain as a component with substantial neighbouring evidence | Specify cue, goal commitment, alternative feasibility, rehearsal and fidelity; avoid attributing component evidence to ROOT |
| S79-EXP-D | Retain as an unexecuted local obstruction hypothesis | Meet design, denominator, fidelity, comparator, substitution and safety gates |
| S80-EXP-E | Retain as an unexecuted test of an established if–then planning family | Use active comparator and isolate planning from obstruction; do not treat positive outcome as proof of ROOT novelty |
| S94-C01 | Retain as a proposed operational architecture; package efficacy unvalidated | Reconcile acronym and duration mismatch; specify causal model, outcome, fidelity, burden, comparator and independent validation |

**Disposition.** Component evidence exists for implementation intentions, some digital-friction effects, selected habit/context processes and metacognitive prompting. The results are heterogeneous and outcome-specific. No registered evidence demonstrates that the complete ROOT package improves durable goal-concordant behaviour, sustained attention or self-mastery, or that its seven-stage sequence adds value over simpler components. No direct refutation of the package is established either; it remains untested as an integrated intervention. No treatise/tracker edits; no experiments executed or authorized.


## 33. Typed state/controller integration audit — §§3, 46, 60–64, 71, 74 and 95

### 33.1 Baseline equation reconciliation

The four principal representations in the treatise are not currently one mathematically consistent state model:

| Location | Representation | Intended role | Integration problem |
|---|---|---|---|
| §3 | \(\mathcal S_t=(A,M_t,X_t,E_t,\Pi_t,G_t,\Theta_t)\) | Primitive system tuple | Most complete inventory, but observation, action, reward/feedback, resource state and disturbance are introduced outside the tuple; update order is ambiguous |
| §46 | \(\widehat S_t=\mathcal M(S_t,\text{observations})\); \(\Theta_{t+1}=\Theta_t+\Delta\Theta(\widehat S_t,G_t,\text{error}_t)\); \(S_{t+1}=F_{\Theta_{t+1}}(S_t,I_t)\) | Self-model and recursive parameter update | Estimator appears to receive the true state; \(C_t\) control state is introduced but not typed; no explicit update of \(\Pi_t\) or of the update rule itself |
| §60 | \(x_{t+1}=(A-BK)x_t+w_t\) | Linear closed-loop stability illustration | \(A\) and \(K\) now denote control matrices/gain, colliding with architecture \(A\) and knowledge base \(K\) elsewhere; this state is not mapped to \(\mathcal S_t\) |
| §71 | \(\mathcal S_{t+1}=\mathcal F(\mathcal S_t,O_t,\mathcal I_t,G_t,R_t,\mathcal R_t)\) | Unified four-operation transition | No explicit selected action, environment state, policy parameters or disturbance; \(\mathcal I_t\), \(R_t\) and \(\mathcal R_t\) lack typed domains; operator order is unresolved |
| §74 | Two-action softmax in terms of \(Q_g,Q_h\), followed by a learning/update claim | Conditional choice-probability result | Monotonicity follows only for a specified softmax selector with fixed positive inverse temperature; the subsequent learning premise needs an explicit update rule |
| §95 | \(S_{t+1}=F(A,M_t,O_t,G_t,\mathcal R_t,\mathcal I(A,M_t),\Pi_t,R_t)\) | Final compressed architecture | Drops explicit \(X_t,E_t,\Theta_t\) and selected action \(a_t\); substitutes \(\mathcal I(A,M_t)\) for \(\mathcal I_t\); no equivalence to §§3/71 is derived |

### 33.2 Specific semantic and formal defects

1. **Transition/action ordering in §3.** The prose says the system receives a signal, updates its internal state and may choose an action, but the displayed transition uses \(a_t\) before the policy equation defines how \(a_t\) is selected. Either specify action selection before state transition, or explicitly model a simultaneous/joint transition kernel. The equations should not leave this order to interpretation.
2. **Observation model and state sufficiency.** \(O_t\sim P(O_t\mid E_t,X_t)\) is a useful observation-kernel sketch, but it does not define the observation space, measurement process, history dependence or missingness. The tuple is not shown to be Markov-sufficient. A Markov claim would require that the next-state distribution be conditionally independent of earlier history given the declared state and inputs.
3. **Undefined feedback/reward.** \(r_t\), \(\text{feedback}_t\), \(R_t\) and “outcome” appear in different equations without a shared definition. Reward, prediction error, observed outcome, self-report and intervention fidelity are not interchangeable. A multi-outcome vector is more defensible than one overloaded scalar.
4. **Memory/policy/parameter interfaces.** §3 updates \(M_t\) and \(\Theta_t\), but does not say whether \(\Pi_t\) is a parameterized policy or a separately updated object. §46 updates \(\Theta_t\) and then changes \(F_{\Theta}\), but does not specify whether this changes the transition model, the action policy or both.
5. **Self-estimation leakage.** §46's \(\mathcal M(S_t,\text{observations})\) provides the estimator with \(S_t\), although the self-model is supposed to estimate potentially latent aspects of the system. Use an observable history/belief-state input, unless the state is explicitly defined as directly observable.
6. **Unmapped control state.** §46 introduces \(C_t\) but the primitive tuple in §3 has no corresponding component or mapping. It must either be a component of \(X_t\)/\(\Pi_t\) with an explicit definition or a separately typed state variable.
7. **Operator composition in §71.** Under standard right-to-left function composition, \(\mathcal F_{context}\circ\mathcal F_{inference}\circ\mathcal F_{control}\circ\mathcal F_{learning}\) applies learning first, then control, inference and context. That is not the apparent narrative order. If the operations are concurrent/coupled, ordinary serial composition is insufficient; define a joint update or a dependency graph. The sentence “ordered or coupled” currently merges two different mathematical structures.
8. **Missing action and environment in §§71/95.** Actions are central to the §3 transition and §74 choice rule, but absent from the unified equations. Environmental state is explicit in §3 but only implicitly absorbed into “external context” in §95. If these are encapsulated in another argument, the encoding map must be stated.
9. **Symbol collisions.** A is architecture in §§3/95 and a state matrix in §60; K is a knowledge base in formal sections and a feedback gain in §60; \(R_t\) is feedback/outcome in §71/95 and a rehearsal-related variable in the habit recurrence; M is memory and also appears in the self-model operator; G denotes goal structure but also generalization in the intelligence functional. These are avoidable namespace collisions, not cosmetic issues, because they obscure whether terms are the same variable.
10. **Time-scale mismatch.** Neural/cue events, action episodes, focus blocks, daily summaries and weekly policy reviews are not one homogeneous time step. A shared subscript \(t\) cannot imply identical sampling or update cadence. The aggregation and synchronization rules must be explicit.
11. **§60-to-human mapping absent.** The Schur stability theorem is valid for the specified homogeneous discrete-time LTI model. The treatise does not identify human state variables, control matrices, gains, sampling interval or disturbance model, nor map them to the primitive tuple. The theorem is a mathematical template, not evidence of behavioural stability.
12. **§74-to-system mapping absent.** The conditional softmax result is a local choice rule. It does not define the transition model, parameter learning, goal revision or stability of the full system. Repeated success alone does not supply a monotone learning update.

### 33.3 Candidate typed contract for controlled revision

The following is a **candidate schema for reconciliation**, not a finalized model or an instruction to rewrite the treatise. It keeps exogenous environment, latent internal state, observations, action, outcomes, resources and policy updates distinct.

| Type | Candidate object | Required semantics |
|---|---|---|
| Fixed architecture | \(\mathfrak A\) | Physical/computational organization and fixed transition constraints; not confused with a state matrix |
| Environment | \(e_t\in\mathcal E\) | External conditions and available cues, with an explicit exogenous or coupled update rule |
| Latent internal state | \(x_t\in\mathcal X\) | Current internal condition; state components and units defined for the target domain |
| Memory/history | \(m_t\in\mathcal M\) | Stored representations and relevant history; specify retention, decay and update timing |
| Goal/constraints | \(g_t\in\mathcal G\) | Goal structure, feasibility constraints and normative priority; distinguish user-chosen goals from measured outcomes |
| Policy and parameters | \(\pi_{\theta_t}\), \(\theta_t\in\Theta\) | Feasible-action distribution and the parameters governing it; specify whether learning updates policy, model or both |
| Observation | \(o_t\in\mathcal O\) | Measured signal generated by an observation model; provenance, noise and missingness recorded |
| Belief/self-estimate | \(b_t\in\mathcal B\) | Estimate derived from observation/history, not silently supplied the inaccessible true state |
| Action | \(a_t\in\mathcal A_{feasible}(b_t,e_t,g_t)\) | Selected action within an explicitly defined feasible set |
| Outcome/feedback | \(y_t\in\mathcal Y\) | Vector of separately defined task outcome, reward/progress, prediction error, functional quality and self-report; no untyped scalar aggregation |
| Resources | \(\rho_t\in\mathcal R\) | Distinct resource state with units, constraints and measurement method; not confused with reward/feedback |
| Disturbance/uncertainty | \(\epsilon_t\) | Exogenous noise/model error with a specified distribution or bounded set where required |

A minimal sequential skeleton could then be written as:

\[
 o_t\sim p_{\mathfrak A}(o_t\mid x_t,e_t),\qquad
 b_t=\mathcal B(b_{t-1},o_t,a_{t-1},y_{t-1}),
\]
\[
 a_t\sim\pi_{\theta_t}(\cdot\mid b_t,m_t,g_t,e_t),\qquad
 (x_{t+1},m_{t+1},e_{t+1})\sim
 T_{\mathfrak A,\theta_t}(x_t,m_t,e_t,a_t,\epsilon_t),
\]
\[
 (\theta_{t+1},\pi_{t+1})=
 U(\theta_t,\pi_t,b_t,g_t,y_t,\rho_t).
\]

This skeleton is intentionally incomplete: it shows the type boundaries and update ordering that must be specified, but it does not establish that the selected variables form a sufficient state, that the operators are identifiable, or that the model predicts human behaviour. A final specification must decide whether environment updates are endogenous, how goals can be revised, how outcomes are observed, and whether policy learning and self-model learning are separate operators.

### 33.4 Integration tests required before calling the model unified

- **Type check:** every operator declares input/output spaces, units, permissible values, missingness and error behaviour.
- **State sufficiency:** demonstrate or explicitly disclaim Markov sufficiency; compare a reduced state with relevant history-augmented alternatives.
- **Causal ordering:** identify whether observation precedes action, action precedes outcome, and feedback updates memory, model, policy or goals; separate simultaneous from serial operations.
- **Clock/aggregation:** define event, episode, daily and weekly update windows and how summaries enter slower policy updates.
- **Symbol registry:** reserve unique names for architecture, control matrices, knowledge sets, reward, rehearsal, resources, memory, model and goals.
- **Identifiability/observability:** show which latent variables and parameters can be estimated from the proposed observations and which remain assumptions.
- **Baseline comparison:** compare the integrated model against established component models and simpler combinations; test whether the full architecture adds held-out predictive or control value.
- **Ablation:** remove each proposed component in turn to test whether its contribution is measurable rather than merely narratively assigned.
- **Robustness:** evaluate uncertainty, disturbances, missing data, context shifts, distribution shift and failure handling.
- **Independent validation:** freeze the model before held-out evaluation; do not tune state definitions or parameters on the final test outcomes.

### 33.5 Claim-level dispositions

| Stable ID | Provisional disposition | Required closure |
|---|---|---|
| S03-M01 / S03-EQ01–EQ05 | Retain as a broad schematic inventory; not a fully specified Markov/state-space model | Fix state/action/observation ordering; define spaces, units, noise, observation history, memory and parameter/policy updates |
| S46-M01 / S46-EQ01–EQ03 | Retain as candidate self-model/update architecture, subject to §31 | Remove estimator input leakage; define \(C_t\), belief state and whether update affects model, policy or both |
| S60-M01 / S60-C01 | Retain the Schur result as a mathematical condition for a specified homogeneous LTI system; no human stability claim | Identify the human model and map its state/input/disturbance to the typed contract before empirical application |
| S61-M01 / S61-EQ01 | Candidate performance/stability proxy only; not a Lyapunov certificate | Define state, equilibrium, units, positive definiteness, invariant domain and drift/decrease conditions |
| S62-P05 / S62-C01 | Conditional proposition remains unproved as written | Supply a quantified deterministic/stochastic drift condition and separately test empirical premises |
| S63-C01 | Practical caution retained; blanket impossibility wording remains under-specified | Define controller class, actuation bounds, disturbance set and performance criterion |
| S64-C01 / S64-EQ01 | Retain as a candidate goal-action criterion, not a validated measure | Define feasible opportunities, context, appropriate goal action, urge scale and threshold |
| S71-C01 / S71-EQ01/EQ02 | Retain as an architectural placeholder, not a defined unified transition law | Type every argument/operator, resolve composition order or concurrency, and include action/environment/policy updates |
| S74-TH05 / S74-C01 | Retain only as a conditional softmax monotonicity result plus an unvalidated human-control hypothesis | State fixed positive inverse temperature, feasible action set and explicit learning update; do not infer full-system stability |
| S95-EQ01 | Downgrade to a conceptual summary until shown equivalent to the typed system model | Restore omitted state/action variables or define their encoding; reconcile notation and derive equivalence to §§3/71 |

**Disposition.** The plan's earlier provisional interface contract is consistent with this audit, but remains a design contract rather than a validated model. Sections 3, 46, 71 and 95 currently describe related but non-equivalent abstractions; §§60–64 and §74 add local control results without closing the full-system interface. The candidate typed schema makes the missing obligations explicit and should guide any future controlled revision. No treatise/tracker edits; no experiments executed or authorized.
