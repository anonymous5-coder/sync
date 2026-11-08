# Claim Evidence Register — Unified Theory of Context, Discovery, and Self-Mastery

**Purpose:** source-controlled research register for claim-level audit, evidence traceability, formal qualification and disposition. This is a research artifact, not the governing execution plan and not an assertion that the framework is validated.

**Audit baseline:** `document_master_visual.md` on branch `edition`, blob `123abdbe9ad3e6c24d150e7db2f38e9562d520d5` (2,618 lines; 95 numbered sections). Section line locations below refer to this exact baseline and must be refreshed if the source changes.

**Scope of this revision:** Sections 1–15 (first claim-inventory batch). This is a claim-level source/disposition pass, not completion of the full 95-section audit.

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

## 7. Open dependencies and next audit actions

- Complete the source-to-claim map for §§16–27, then §§28–40, and continue in baseline section order.
- Add primary-source locations where reviews currently provide only contextual support.
- Reconcile §2's three labels with §1's claim categories and §15's multidimensional evidence ladder without silently rewriting the treatise.
- Complete the full formal premise map and cross-reference the detailed M1–M18 audit.
- Preserve the distinction between “not explicitly stored,” “not logically entailed,” “statistically predictable” and “empirically corroborated.”
- Reopen S08 if new developmental evidence changes the scope of the newborn example.
- Do not mark Section 12.2, 12.5, 12.6 or Section 13.1 complete on the basis of this first batch alone.

**Status:** §§1–15 have a first claim-level source/disposition register. This batch is not the complete audit of the treatise, and no claim is promoted to empirical validation by inclusion here.
