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
