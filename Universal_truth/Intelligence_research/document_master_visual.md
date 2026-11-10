# THE UNIFIED THEORY OF CONTEXT, DISCOVERY, AND SELF-MASTERY
## A Master Treatise on Space or Null Theory, Out of Box Theory, Recursive Intelligence, and the ROOT Control Protocol

**Version:** Master Treatise 1.0  
**Date:** 4 November 2026  
**Status:** Research draft — a conceptual synthesis with conditional formal results, candidate models, bounded evidence assessments, and experimental protocols that have not been executed.

---

## Abstract

This manuscript examines a proposed relationship among four named foundations:

1. **Space or Null Theory** — a proposed account of how context, internal structure and available information condition processing.
2. **Out of Box Theory** — a proposed account of deriving or constructing conclusions that were not explicitly supplied as observations, subject to the information and constraints already represented.
3. **Recursive Intelligence** — a proposed functional construct concerning self-representation, monitoring and modification of future system operation.
4. **ROOT Control Protocol** — a proposed behavioural intervention architecture for recognising triggers, changing action accessibility, practising alternative responses and updating interventions from outcomes.

The manuscript does not establish that these are four distinct mechanisms, that they form a complete unified theory, or that their integration has explanatory or predictive superiority over established alternatives. It develops a conceptual dependency map and identifies the formal, empirical and operational conditions that would be needed to test the proposed relationships.

Its formal core includes standard information-theoretic identities and conditional model-theoretic results. In particular, a proposition entailed by a knowledge base can be derived under a proof calculus complete for the specified semantics; this is derivation from premises, not acquisition of arbitrary facts without information. A separate countermodel argument describes a boundary on what follows from premises when admissible models disagree. These results do not establish predictive performance in a physical system.

The physical–cognitive discussion treats embodiment, energy and finite resources as constraints on biological computation. It considers cost-sensitive action selection, reinforcement learning, habit and cognitive control as candidate links between physical implementation and behaviour. The complete causal bridge from physical resource use to subjective effort, action valuation and an individual's behaviour has not been identified or validated. The equations are therefore presented with explicit assumptions and limitations rather than as a literal description of brain computation.

The manuscript also reviews candidate behavioural-state, learning, feedback and stability models. The ROOT state vector is an operational set of ordinal self-ratings, not a validated latent state or clinical instrument. The control-theory results apply to specified mathematical systems; no human or ROOT controller has been identified as stable, and the proposed behavioural feedback statement is a testable hypothesis rather than a stability theorem. The four foundations' joint update remains schematic, with typed interfaces, update semantics and incremental explanatory value unresolved.

The evidence review distinguishes primary studies, reviews, abstract-level records and access-limited sources. It identifies relevant neighbouring theories and competing explanations, while retaining unresolved source and provenance gaps. Experiments A–F are protocol templates only: none has been executed, preregistered or empirically validated. The integrated ROOT package has no demonstrated package-level efficacy.

The manuscript's current contribution is therefore a structured conceptual synthesis, a set of conditional formal results, a claim-level evidence/disposition inventory and a research programme with explicit unresolved requirements. It is not a validated unified theory, a new established law of nature, a proven behavioural controller or an independently reviewed final edition.

---

# PART I — FOUNDATIONS AND THEORETICAL SCOPE

## 1. The problem to be solved

The original document identified three linked questions:

- How can intelligence acquire knowledge from a world it initially does not understand?
- How can intelligence derive something that has not been explicitly presented to it?
- Why can a system that understands its own objective repeatedly execute a different, unwanted behaviour?

These questions appear to belong to separate disciplines: epistemology, physics, information theory, neuroscience, reinforcement learning, and control engineering. The apparent separation is partly an artefact of disciplinary boundaries. Each concerns a system that has an internal state, receives or generates information, acts under constraints, and changes as a consequence of its interaction with the world.

The unified problem is:

> How does a physically embodied information-processing system acquire a model of reality, infer consequences beyond direct observation, select actions under limited resources, and modify the mechanisms that govern its future selection of actions?

This question will be treated at four levels:

| Level | Object of analysis | Principal question |
|---|---|---|
| Physical | Matter, energy, state transitions | What can a physical system store, compute, and change? |
| Informational | Signals, uncertainty, memory, models | What information is available and what can be inferred? |
| Cognitive | Attention, learning, valuation, action | How does an organism select and sustain behaviour? |
| Recursive-control | Self-monitoring and policy modification | How can a system change its own future operation? |

A valid theory must connect these levels without confusing them. A neural computation is physical, but a psychological concept is not automatically a thermodynamic quantity. An inference can be logically valid without being empirically true. A behaviour can be habitual without being an addiction. A mathematical model can be useful without being a literal description of every neuronal event.

These distinctions are not retreats from theoretical ambition. They are conditions for deriving claims that can survive scrutiny.

## 2. What the theory is—and is not

This treatise retains the user's names exactly:

- **Space or Null Theory**
- **Out of Box Theory**
- **Recursive Intelligence**
- **ROOT Control Protocol**

The framework adds formal definitions and mathematical machinery around these names. The names identify the conceptual contributions; they do not imply that the corresponding formulations have already been accepted as established scientific laws.

Three epistemic labels will be used:

- **Established constraint:** a result supported by mature scientific theory or substantial empirical evidence.
- **Derived proposition:** a result that follows mathematically from stated assumptions.
- **Research hypothesis:** a proposed claim whose empirical validity remains to be tested.

The distinction matters particularly in the physical–cognitive bridge. Thermodynamics constrains all biological computation. It does not, by itself, tell us why a particular person checks a phone at 11:17 a.m. The latter requires a model of learned values, cues, physiology, task structure, and available actions.

---

# PART II — AXIOMATIC CORE

## 3. Primitive objects

Let an intelligent system be represented at time $t$ by:

$$
\mathcal{S}_t=(A,M_t,X_t,E_t,\Pi_t,G_t,\Theta_t)
$$

where:

- $A$: architecture — the system's physical and computational organization, transition rules, and built-in constraints.
- $M_t$: internal memory and representations at time $t$.
- $X_t$: current internal state, including active neural or computational states.
- $E_t$: environment, including external signals, objects, other agents, and physical conditions.
- $\Pi_t$: available policies or action-selection rules.
- $G_t$: objective structure, including goals, constraints, needs, and priorities.
- $\Theta_t$: parameters that can change through learning, development, or deliberate modification.

At each decision step, the system receives an observation, selects an action, and then transitions to its next internal state:

$$
O_t \sim P(O_t\mid E_t,X_t)
$$

$$
a_t\sim \Pi_t(\cdot\mid X_t,M_t,O_t,G_t)
$$

$$
X_{t+1}=F_A(X_t,M_t,O_t,a_t,\xi_t)
$$

Here $\xi_t$ represents noise and unmodelled influences; $r_{t+1}$ denotes the outcome/reward observed after action $a_t$, and $\text{feedback}_{t+1}$ denotes post-action feedback used by a learning update. These are schematic variables, not yet operationally typed.

The system may update memory and policy:

$$
M_{t+1}=U_M(M_t,O_t,a_t,r_{t+1})
$$

$$
\Theta_{t+1}=U_\Theta(\Theta_t,\text{feedback}_{t+1})
$$

The formulation is intentionally general. A human brain, an artificial agent, and a physical controller can all be represented at this abstract level, although their architectures and mechanisms differ substantially. $\mathcal S_t$ is a system-level descriptor, not a claim that the listed components form a minimal or Markov-sufficient state; state sufficiency and update rules must be established for each application.

## 4. Axioms

### Axiom 1 — Physical embodiment

Every real information-processing operation is implemented by a physical system. Its state transitions are constrained by the laws governing its physical substrate.

**Consequence:** There is no physically realized computation that is exempt from energy, time, noise, material, and causal constraints.

### Axiom 2 — Structural dependence

A system's response to a signal depends not only on the signal but also on the system's architecture and current internal state.

$$
Y=F_A(X,M,O)
$$

The same input can produce different outputs in systems with different memories, architectures, or states.

### Axiom 3 — Contextual acquisition

New external observations can alter internal representations, beliefs, and future behaviour.

$$
M_{t+1}=U_M(M_t,O_t,\ldots)
$$

This is the formal core of **Space or Null Theory**.

### Axiom 4 — Internal transformation

A system can transform stored representations through operations that are not equivalent to copying its observations. It can compose, abstract, simulate, deduce, compress, and generate candidate models.

This is the formal core of **Out of Box Theory**.

### Axiom 5 — Bounded resources

A finite physical system has finite energy, time, memory, bandwidth, and processing capacity over any specified interval.

For a system operating over an interval $[0,T]$:

$$
\int_0^T P(t)\,dt \leq E_{\mathrm{available}}(T)
$$

where $P(t)$ is power and $E_{\mathrm{available}}$ is the available energy budget.

### Axiom 6 — Adaptive selection

When multiple actions are available, the system's action-selection mechanism assigns them different probabilities or priorities according to its state, learned values, goals, and constraints.

### Axiom 7 — Recursive accessibility

Some systems can construct representations of aspects of their own state or behaviour and use those representations to modify later processing.

This is the formal core of **Recursive Intelligence**.

### Axiom 8 — Fallible model–world correspondence

An internal model is not identical to the external world. It can be incomplete, inaccurate, overconfident, or underdetermined by available evidence.

A system must therefore distinguish a model-derived conclusion from a verified fact.

**Physical-implementation references (limited scope):** R09, R10, R60, R61, R62. These sources inform the physical-computation and neural-energy constraints relevant to Axioms 1 and 5; they do not establish the entire eight-item list, particularly the adaptive-selection or recursive-accessibility capability claims. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 5. Definitions

### Definition 1 — Context

A context is any structured condition that changes the interpretation, probability, cost, or consequence of a system's state transition.

Context is broader than a sensory stimulus. It includes:

- external observations;
- internal memories;
- current bodily state;
- task goals;
- learned associations;
- social and physical constraints;
- mathematical or logical premises;
- the system's architecture.

Thus, an absence of new external input does not imply an absence of context.

### Definition 2 — Null condition

A null condition is a specified absence of a selected class of input. It must always identify what is absent.

For example:

$$
X_{\mathrm{external}}=0
$$

does not imply:

$$
M=0,\quad A=0,\quad G=0
$$

A literal absence of every physical state and every computational rule is not a meaningful operating condition for an intelligence. A system cannot perform an inference without some state and some transition structure.

### Definition 3 — Intelligence

For this framework, intelligence is the capacity of a system to construct and use internal representations to predict, infer, select, or adapt actions in relation to structured objectives and environmental constraints.

This is an operational definition, not a claim that all intelligent systems are conscious.

### Definition 4 — Novelty

A result is novel relative to a system if the result was not explicitly represented in the system's accessible records before the relevant computation.

Novelty is relative to a reference set. It does not mean that the result came from no prior information.

### Definition 5 — Discovery

A discovery is a newly obtained representation or proposition that is both novel relative to the system and supported by a valid derivation, a successful prediction, or an evidential procedure.

A generated possibility is not automatically a discovery. A discovery requires a justified relationship between the representation and its target.

### Definition 6 — Habit

A habit is a learned policy that can be selected or executed with reduced dependence on deliberative evaluation of the current consequences.

A habit may be beneficial, neutral, or harmful. Automaticity alone does not imply pathology.

### Definition 7 — Distraction

A distraction is a shift of limited processing or action resources away from a currently selected objective toward a competing representation or action.

Distraction is defined functionally by displacement, not morally by whether the competing activity is good or bad.

### Definition 8 — Self-mastery

Self-mastery is the sustained capacity to preserve, revise, and execute chosen objectives while regulating competing impulses and adapting to feedback.

It does not mean eliminating biological drives, suppressing every thought, or maintaining uninterrupted concentration indefinitely.

---

# PART III — SPACE OR NULL THEORY

## 6. Formal statement

**Space or Null Theory:** A system's meaningful processing is conditioned by its internal structure and by the contexts available to it. New external context can supply information that changes its internal model, while the absence of new external context does not erase the information and structure already present within the system.

The theory therefore contains two different cases:

1. **External-context acquisition:** the system receives new observations.
2. **Internal-context operation:** the system continues processing using stored representations and architecture without receiving new observations.

These cases must not be conflated.

## 7. Information-theoretic formulation

Let $W$ denote a relevant world-state and $M$ the system's internal representation. The uncertainty about the world before receiving an observation is:

$$
H(W\mid M)
$$

After receiving observation $O$, the remaining uncertainty is:

$$
H(W\mid M,O)
$$

The information gained from the observation, relative to the existing model, is:

$$
I(W;O\mid M)=H(W\mid M)-H(W\mid M,O)
$$

If this conditional mutual information is positive, the observation reduces uncertainty about the relevant world-state.

But an observation need not always reduce uncertainty. It can be irrelevant, noisy, misleading, or ambiguous. The formal expression does not guarantee that every incoming stimulus is useful.

### Proposition 1 — Context can be informative without being sufficient

An observation can reduce uncertainty about one variable while leaving other variables undetermined.

**Derivation:** Mutual information is defined relative to the joint distribution of specified variables. A positive $I(W;O\mid M)$ establishes a reduction in conditional uncertainty about $W$, not complete knowledge of all properties of the world. Therefore, contextual acquisition can be partial.

### Proposition 2 — No new observation does not imply no computation

If $O_t$ is absent during an interval but $A$, $M_t$, and $X_t$ remain nontrivial, internal state transitions can continue:

$$
X_{t+1}=F_A(X_t,M_t,0,\xi_t)
$$

This can include memory replay, simulation, deduction, planning, and spontaneous dynamics.

**Conclusion:** A system can continue to think in the absence of new sensory input because it is not operating in the absence of all context.

**Claim-linked evidence register records:** R01, R05, R21. R01 and R21 provide information-theoretic foundations; R05 addresses statistical inference and model dependence. R03 is mapped to the separate underdetermination discussion in §11, and R22 to algorithmic complexity in §13, rather than to the conditional-mutual-information identity here. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 8. The newborn and the empty-system thought experiment

A newborn is not a blank machine. Its nervous system has inherited structure, developmental programs, sensory transducers, regulatory mechanisms, and learning capacities. Its early experience changes the system, but the capacity to learn is itself part of the system's initial organization.

Likewise, an artificial neural network is not a blank entity at inference time. Its architecture and parameters embody a large amount of structure produced by training and design.

The hypothetical intelligence placed in an empty region of space must also be specified carefully:

- Does it have a physical substrate?
- Does it have memory?
- Does it have internal state?
- Does it have transition rules?
- Does it have energy?
- Does it have sensors?
- Does it possess inherited structure?

If all of these are removed, the thought experiment no longer describes an operating intelligence. If they remain, the system has internal context even if external context is absent.

This clarification strengthens rather than weakens Space or Null Theory: the theory concerns the conditions for meaningful processing, not the simplistic assertion that every thought requires a fresh external stimulus.

---

**Claim-linked evidence register records:** R06, R07, R08. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.

# PART IV — OUT OF BOX THEORY: EPISTEMIC LIMIT AND EXPANSION


## 9. The central question

Can an intelligence deduce, predict, or uncover a reality that it has not directly observed?

Yes—under precise conditions.

A system can derive a proposition about an unobserved object or event when its internal premises constrain the possible worlds strongly enough that the proposition follows from those premises.

This is not access to information from literal nothingness. It is the extraction of consequences that were implicit in a structured model.

The important distinction is between:

- **not directly observed**;
- **not explicitly represented**;
- **not logically implied by the system's available information**.

These are three different conditions.

A proposition may be unobserved and not explicitly stored, yet logically implied by the model. Such a proposition can be discovered by inference.

A proposition that is independent of every constraint available to the system cannot be uniquely inferred merely by thinking harder.

**Claim-linked evidence register records:** R02, R05. These sources support the distinction between deductive consequence, inductive support and model-dependent statistical inference; the formal countermodel argument is stated directly above.

## 10. Formal epistemic model

Let $\Omega$ be the set of possible worlds compatible with the system's background information. Let $K$ be the system's knowledge base, consisting of premises, constraints, axioms, and learned regularities.

A proposition $p$ is entailed by $K$ if:

$$
K\models p
$$

Equivalently:

$$
\forall w\in\Omega(K),\quad p(w)=\mathrm{true}
$$

where $\Omega(K)$ is the subset of possible worlds satisfying $K$.

The system does not need to observe the particular event described by $p$ if the proposition is already entailed by the constraints in $K$.

### Theorem 1 — An entailed proposition can be derived before direct observation

**Statement:** Let $K$ be a knowledge base with at least one model under a specified semantics. If $K\models p$ and the chosen proof calculus is complete for that semantics, then $K\vdash p$. The derivation can be obtained without a new direct observation of the event described by $p$, provided the system can execute the required proof search with sufficient computational resources.

**Proof:**

1. By assumption, every model of $K$ satisfies $p$: $K\models p$.
2. By completeness of the chosen proof calculus, semantic consequence implies derivability: $K\vdash p$.
3. Soundness gives the converse validity safeguard: any proposition derived in that calculus from $K$ is a semantic consequence of $K$.
4. The derivation uses the premises and inference rules in $K$; it does not require a new direct observation of the target event.
5. The nonempty model-class condition prevents the entailment from being vacuous because $K$ has no models. The result establishes derivability from $K$, not actual-world truth. For that further claim, the actual world $W$ must satisfy the premises: $W\models K$.

$$
K\models p\quad\xRightarrow[\text{completeness}]{}\quad K\vdash p
$$

The proposition can be new to the system while being logically constrained by information it already possesses. This is discovery relative to the system's prior representation, not acquisition of an unconstrained fact from nothing.

### Corollary 1 — Discovery need not require direct sensory access

Direct sensory access is not a necessary condition for every valid discovery. A theorem, mathematical consequence, or physical prediction can be derived from prior constraints.

### Corollary 2 — The world can be predicted through its structure

If an internal model captures reliable structural regularities of the world, deductions from that model can describe unobserved features of the world.

The reliability of the prediction depends on the reliability and scope of the model.

**Claim-linked evidence register records:** R02, R05. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 11. The underdetermination boundary

The preceding theorem does not imply that every unknown fact can be inferred.

### Theorem 2 — No unique deduction of an unconstrained contingent fact

**Statement:** If two possible worlds $w_1$ and $w_2$ satisfy all information available to a system, but a proposition $p$ is true in $w_1$ and false in $w_2$, then the system's available information does not logically determine $p$.

**Proof:**

1. Let $K$ be the system's total available information.
2. Suppose $w_1\models K$ and $w_2\models K$.
3. Suppose $p(w_1)=\mathrm{true}$ and $p(w_2)=\mathrm{false}$.
4. Then not every model of $K$ satisfies $p$.
5. Therefore $K\not\models p$, and likewise $K\not\models\neg p$.

Hence, no sound deduction from $K$ alone can uniquely establish $p$.

This is not a weakness of intelligence. It is a limit imposed by information and logic.

**Claim-linked evidence register records:** R03, R05. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 12. The upgraded meaning of Out of Box Theory

**Out of Box Theory:** An intelligence can generate and derive conclusions that are not explicitly contained in its observations, by exploiting structural information encoded in its architecture, representations, mathematical constraints, learned regularities, and inferential operations. It can thereby predict or discover unverified realities before direct sensory confirmation, provided those realities are sufficiently constrained by the information it possesses.

The theory is stronger than mere recombination. It includes:

1. **Combinatorial novelty:** constructing new arrangements of known elements.
2. **Structural inference:** deriving consequences of relationships not explicitly stated.
3. **Model-based prediction:** predicting unobserved outcomes from a model.
4. **Abductive construction:** proposing a model that could explain observations.
5. **Mathematical discovery:** deriving necessary consequences of axioms and definitions.
6. **Empirical anticipation:** predicting a physical phenomenon before directly observing it.

The theory does not license arbitrary certainty. It distinguishes derivation, prediction, and speculation.

**Claim-linked evidence register records:** R02, R04, R05. These references distinguish deductive consequence from probabilistic updating and ampliative statistical inference; they do not establish a single mechanism unifying the six listed modes.

## 13. How can internal architecture contain information about reality?

The architecture $A$ and memory $M$ of an intelligence are not independent of the universe.

For humans, architecture is shaped by biological evolution, development, and physical interaction. For artificial systems, architecture and parameters are shaped by design, data, optimization, and the physical processes that generated those data.

The system can therefore carry compressed structural information about the world.

Let $W$ represent the world and $Z=(A,M)$ the system's internal structure. In general:

$$
I(W;Z)>0
$$

may hold when the system's architecture or memory is statistically dependent on world structure.

This does not mean the system contains a complete copy of reality. It means that its internal state may carry information correlated with features of the world. The statement $I(W;Z)>0$ is conditional on a specified joint distribution; it is not a universal fact about every architecture. Positive mutual information alone does not guarantee that the information is accessible, task-relevant, stable out of sample or sufficient for accurate prediction.

A system can exploit that information to predict additional features only if its model and inference procedure preserve the relevant dependence and generalize to the target conditions.

### Example: Mathematical prediction of an unobserved phenomenon

A theory may combine previously established observations with mathematical constraints and imply a new phenomenon. The predicted phenomenon can be unknown to the theorist at the time of derivation. If the prediction is later observed, the derivation has achieved empirical success.

The discovery is not magic. The model encoded constraints that the world also obeyed.

The prediction is powerful precisely because it risks failure: the world could have contradicted the model.

**Claim-linked evidence register records:** R01, R05, R21, R22. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 14. Bayesian form of Out of Box Theory

Let $H$ be a hypothesis and $D$ the available evidence. A system forms:

$$
P(H\mid D)=\frac{P(D\mid H)P(H)}{P(D)}
$$

A model can then predict a future or unobserved observation $Y$:

$$
P(Y\mid D)=\sum_H P(Y\mid H,D)P(H\mid D)
$$

The prediction is derived from the combination of prior structure, evidence, and a model connecting hypotheses to outcomes.

A strong prediction can be made without directly observing $Y$. But the prediction remains conditional on the model and prior assumptions.

### Distinguishing deduction from induction

- Deduction: if premises are true and the inference is valid, the conclusion follows necessarily.
- Induction: evidence supports a generalization but does not guarantee it.
- Abduction: a hypothesis is proposed as a possible explanation.
- Prediction: a model assigns an expected outcome to an unobserved condition.

Out of Box Theory includes all four, but their certainty levels differ.

**Claim-linked evidence register records:** R04, R05. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 15. A disciplined epistemic ladder

Every generated result should be assigned to one of these levels:

| Level | Status | Required support |
|---|---|---|
| 0 | Imagined possibility | Coherent representation |
| 1 | Internally consistent hypothesis | No contradiction found within stated assumptions |
| 2 | Deductive consequence | Valid derivation from explicit premises |
| 3 | Probabilistic prediction | Calibrated model and evidence |
| 4 | Independently corroborated discovery | Successful tests or independent observations |
| 5 | Robust explanatory structure | Repeated prediction, replication, and resistance to alternatives |

This ladder prevents a common error: moving from "I can conceive it" to "it is true."

It also prevents the opposite error: assuming that an unobserved proposition cannot be known. A proposition can be logically entailed before the event is observed.

---

# PART V — THE PHYSICAL–COGNITIVE BRIDGE

## 16. The bridge must be derived, not asserted

A mind is not an abstract decision-maker floating outside physics. A human brain is an open, non-equilibrium biological system. It receives chemical energy, maintains ion gradients, transmits electrochemical signals, changes synaptic strengths, regulates the body, and produces behaviour.

Neural computation therefore has physical costs.

But a critical distinction must be maintained:

- Thermodynamic entropy is a physical state function or statistical quantity.
- Shannon entropy measures uncertainty in a probability distribution.
- Psychological distraction is a functional displacement of attention or action.
- Mental effort is a subjective and computational phenomenon associated with control demands and resource allocation.

These quantities can be related through models. They are not identical by definition.

The valid bridge is not:

$$
\text{psychological distraction}=\text{thermodynamic entropy}
$$

The valid bridge is:

$$
\text{physical resource constraints}
\rightarrow
\text{bounded computation}
\rightarrow
\text{cost-sensitive control}
\rightarrow
\text{action selection}
\rightarrow
\text{learned behavioural persistence}
$$

This is the central derivation of the treatise.

**Claim-linked evidence register records:** R09, R11, R13, R14, R60, R63. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 17. Physical computation and energy

A computation is a physical process implemented by a substrate. The system must move between physical states that encode logical states.

Let:

- $z$ be the physical microstate;
- $m$ be the logical or informational state;
- $T$ be the temperature of the relevant thermal environment;
- $W$ be work supplied to a computation;
- $Q$ be heat transferred into the system.

Using the convention that $Q$ is heat added to the system and $W$ is work done on the system, the first law gives:

$$
\Delta U=Q+W
$$

If $W$ instead denotes work done by the system, the equivalent form is $\Delta U=Q-W$. Physical state changes require energy exchange or redistribution; sign conventions must be used consistently.

For logically irreversible erasure of one unbiased bit, Landauer's principle gives the ideal lower bound on heat dissipated to the environment:

$$
Q_{\mathrm{diss,min}}=k_B T\ln 2
$$

This is heat dumped to the environment under specified assumptions, not the heat input $Q$ in the first-law convention above and not the actual energy cost of a human thought. Real biological computation is far from an idealized one-bit erasure operation.

The principle relevant to this treatise is broader: information processing is physically implemented, and its implementation has energetic and temporal costs.

**Claim-linked evidence register records:** R09, R10, R11, R12, R13, R60, R61, R62, R63, R69, R70. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 18. The brain as an open non-equilibrium system

A living brain does not sit at thermodynamic equilibrium. It maintains organized states through continuous energy and material exchange.

A simplified energy budget is:

$$
P_{\mathrm{brain}}(t)
=
P_{\mathrm{baseline}}(t)
+
P_{\mathrm{signalling}}(t)
+
P_{\mathrm{plasticity}}(t)
+
P_{\mathrm{regulation}}(t)
$$

The terms are conceptual categories, not a claim that they can be cleanly separated in every measurement.

Brain function involves distributed metabolic demand across processes such as:

- sensory processing;
- internal prediction;
- memory retrieval;
- action selection;
- motor execution;
- autonomic regulation;
- learning and plasticity;
- error monitoring.

A task that requires sustained working memory, inhibition, conflict resolution, and active updating may impose a different control demand from a familiar routine.

The brain does not simply choose the task with the greatest abstract long-term value. It must implement that choice through a biological system with finite capacities and competing needs.

**Claim-linked evidence register records:** R11, R12, R13, R14, R60, R61, R62, R63, R69. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 19. From energy constraints to computational cost

Let $a$ denote an available action. Define:

- $R(a)$: expected task or reward value;
- $E(a)$: expected physical/physiological energy expenditure, distinct from subjective effort;
- $C_{\mathrm{ctrl}}(a)$: control and deliberation cost;
- $D(a)$: delay cost;
- $K(a)$: switching or initiation cost;
- $L(a)$: expected long-term consequence;
- $\rho$: weighting of energetic cost;
- $\gamma$: weighting of control cost;
- $\delta$: weighting of delay;
- $\kappa$: weighting of switching cost.

A simplified action score is:

$$
Q(a)=
R(a)+L(a)
-\rho E(a)
-\gamma C_{\mathrm{ctrl}}(a)
-\delta D(a)
-\kappa K(a)
$$

This equation is a candidate model specification. Its terms must be converted to commensurable utility units or explicitly normalized before they can be added; raw energetic, temporal, delay and control-cost measurements do not automatically share units. In particular, physical energy expenditure $E(a)$ must not be inferred from subjective effort or treated as interchangeable with $C_{\mathrm{ctrl}}(a)$. Define $R(a)$ and $L(a)$ on compatible decision horizons and check for overlap to avoid double counting. Its coefficients must be estimated for a particular system; they are not universal constants of the brain, and no such coefficients have been identified here.

The action-selection mechanism can be represented by a softmax distribution:

$$
P(a\mid s)=
\frac{\exp(\beta Q(a\mid s))}
{\sum_{b\in\mathcal{A}(s)}\exp(\beta Q(b\mid s))}
$$

where $s$ is the current state, $\mathcal{A}(s)$ is the feasible action set, and $\beta>0$ controls the sharpness of selection. The parameter $\beta$ has inverse-score units if $Q$ is dimensional; a dimensionless implementation requires a normalized score. The distribution assumes a nonempty feasible action set.

As $\beta$ increases, higher-scoring actions dominate more strongly. As $\beta$ decreases, selection becomes more stochastic.

This is a useful formal model of action selection. It is not a claim that the brain literally computes a single scalar $Q$ in a central location.

**Claim-linked evidence register records:** R13, R14, R15, R24. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 20. Why a familiar distraction can defeat an important task

Consider two actions:

- $a_f$: continue a difficult, important task;
- $a_h$: execute a familiar habitual response, such as checking a phone.

The long-term objective may favour $a_f$:

$$
L(a_f)>L(a_h)
$$

But the habitual response may have:

- lower initiation cost;
- lower immediate effort;
- a stronger cue association;
- faster reward or relief;
- less need for deliberation;
- a more predictable immediate outcome.

Thus, it is possible that:

$$
Q(a_h\mid s)>Q(a_f\mid s)
$$

under the current state $s$, even though the person explicitly endorses the long-term value of $a_f$.

This is one possible formalization of an intention–execution gap under the specified score model.

The gap does not require the person to be unintelligent. It requires only that the mechanisms governing immediate action selection differ from the person's reflective evaluation of long-term goals.

### Proposition 3 — Local action advantage can favour a globally inferior action

**Statement:** In a specified decision state, a selector can favour a locally higher-scoring action even when another action has greater long-term objective value.

**Derivation:**

1. Let the long-term objective value be $V_L(a)$.
2. Let immediate selection value be $Q(a)=V_{\mathrm{immediate}}(a)+V_L(a)-C(a)$.
3. Suppose $V_L(a_f)>V_L(a_h)$.
4. Suppose the cost and immediate-value difference satisfies:

$$
V_{\mathrm{immediate}}(a_h)-C(a_h)
>
V_{\mathrm{immediate}}(a_f)-C(a_f)
+
V_L(a_f)-V_L(a_h)
$$

5. Then $Q(a_h)>Q(a_f)$.
6. Under softmax selection with $\beta>0$, $a_h$ is more probable than $a_f$. A greedy selector chooses $a_h$ only if it is a maximizer over the full feasible action set.

Therefore, under the stated score definitions and selector conditions, the model can favour an action that conflicts with the reflective long-term objective.

The solution must change the action-selection conditions, not merely repeat the long-term preference.

**Claim-linked evidence register records:** R15, R24, R26. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 21. Why habits are efficient—and why efficiency can become a trap

A habit is a cached policy. It stores a response that was previously useful or rewarding and reduces the need to recompute the decision every time.

This has an obvious computational advantage.

Suppose a model-based controller evaluates future consequences at cost $C_m$ each time it acts. A cached controller has a smaller execution cost $C_h$, where:

$$
C_h<C_m
$$

If the environment is stable and the cached action remains suitable, the habit is efficient.

But if the environment changes or the person's objective changes, the cached response may no longer be appropriate. The system can continue executing the old policy because the cue-response mapping is well learned and requires little deliberation.

This is the central duality:

$$
\boxed{\text{Habit = computational efficiency under repetition}}
$$

and

$$
\boxed{\text{Maladaptive habit = cached efficiency misapplied to a changed objective}}
$$

A habit is not inherently bad. Its value depends on whether the cue-response mapping remains aligned with current goals and conditions.

**Claim-linked evidence register records:** R16, R18, R19, R23, R26, R28, R29, R30, R53. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 22. Cue learning as a dynamical system

Let $s_t$ denote the state available before action $a_t$; it includes cue $c_t$ and any other variables used by the policy. After action $a_t$, the system receives outcome/reward $r_{t+1}$ and enters state $s_{t+1}$.

One standard off-policy candidate is the Q-learning update:

$$
Q_{\mathrm{RL},t+1}(s_t,a_t)
=
Q_{\mathrm{RL},t}(s_t,a_t)
+
\alpha
\left[
r_{t+1}
+
\gamma \max_{a'\in\mathcal{A}(s_{t+1})}
Q_{\mathrm{RL},t}(s_{t+1},a')
-
Q_{\mathrm{RL},t}(s_t,a_t)
\right]
$$

where:

- $\alpha$ is a learning rate;
- $\gamma$ is a future-value discount factor;
- $\mathcal{A}(s_{t+1})$ is the feasible action set in the next state;
- $Q_{\mathrm{RL},t}(s,a)$ is an action-value estimate, distinguished from the generic action score $Q(a)$ in §19.

The update assumes that the state representation is adequate for a Markov-style transition model and that reward timing and the feasible action set are defined. Those assumptions have not been validated for the human behavioural model in this treatise. This is a standard computational learning abstraction, not a complete biological habit-formation mechanism. The displayed one-step update assumes a Markov-style state representation, a defined finite feasible action set, $0\leq\gamma<1$ and a learning rate $0<\alpha\leq1$. No convergence guarantee is claimed; convergence would require additional conditions on stationarity, exploration and the learning-rate schedule.

If the cue is represented in the state, the action is included in the feasible action set, and the outcome is encoded as reward, the action-value estimate can increase when the observed TD target exceeds its current estimate. Relief or novelty is not automatically a reward: its sign and magnitude must be specified by the task's reward function. Relief counts as negative reinforcement only when it is contingent on the response and increases the future probability of that response.

A later encounter with the cue can bias action selection if the operative policy uses the learned action values. The update alone does not guarantee that the policy changes, that the action becomes habitual, or that the effect persists outside the specified state/action representation.

**Claim-linked evidence register records:** R16, R18, R19, R26, R28, R30, R53. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 23. Why relief can reinforce behaviour

Not all reinforcement is pleasure-seeking.

Suppose an uncomfortable state $u$ precedes an avoidance action $a_e$. The action temporarily reduces discomfort:

$$
u_t>u_{t+1}
$$

The reduction itself can reinforce $a_e$, even if the action produces no lasting satisfaction.

The sequence is:

$$
\text{Discomfort}
\rightarrow
\text{Avoidance}
\rightarrow
\text{Relief}
\rightarrow
\text{Increased probability of avoidance next time}
$$

This is negative reinforcement in the technical behavioural sense: a response is strengthened because it removes or reduces an aversive condition.

The implication is important for studying. A person may not be pursuing entertainment alone; they may be escaping uncertainty, effort, fear of failure, boredom, or fatigue.

If the true reinforcing consequence is relief from task discomfort, merely blocking entertainment may expose the discomfort without teaching a replacement response.

**Claim-linked evidence register records:** R16, R17, R18, R19, R28, R30, R53. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 24. Thermodynamic entropy is not psychological disorder

A common but invalid shortcut is to say that the brain chooses distraction because it follows the second law of thermodynamics or seeks maximum entropy.

That statement is too broad to be a scientific explanation.

The second law constrains the total entropy balance of physical processes. It does not imply that every subsystem maximizes disorder locally, nor that a person chooses the easiest stimulus because the brain is "trying to increase entropy."

Biological systems maintain local organization by consuming free energy and exporting entropy to their surroundings.

A more defensible statement is:

1. Neural computation is physically implemented.
2. It consumes metabolic resources and is subject to noise and finite capacity.
3. Cognitive control has opportunity costs.
4. Learned policies can reduce the repeated cost of action selection.
5. Cue-triggered habits can therefore dominate when deliberative control is costly, weakened, or poorly supported by the environment.

This is a physical–computational bridge. It does not equate entropy with distraction.

**Claim-linked evidence register records:** R11, R14. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 25. A free-energy distinction

In thermodynamics, Helmholtz free energy is:

$$
F=U-TS
$$

where $U$ is internal energy, $T$ temperature, and $S$ thermodynamic entropy.

In statistical inference and theoretical neuroscience, "variational free energy" is a mathematical quantity used to bound surprise or model evidence under particular assumptions.

The two concepts are related historically and mathematically in some formulations, but they are not interchangeable. A cognitive model minimizing variational free energy is not automatically minimizing the brain's physical Helmholtz free energy in a simple literal sense.

For this treatise, the term **resource-constrained predictive control** will be used when the argument concerns action selection, uncertainty, and biological cost. This avoids turning a useful mathematical analogy into an unsupported identity.

**Claim-linked evidence register records:** R20. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 26. The physical–cognitive bridge: Proposed multilevel hypothesis

The proposed bridge hypothesis can be represented as a chain of candidate links:

$$
\begin{aligned}
&\text{Physical embodiment}\\
&\Downarrow\\
&\text{Finite energy, time, and computational capacity}\\
&\Downarrow\\
&\text{Cost-sensitive allocation of processing and control}\\
&\Downarrow\\
&\text{Preference for cached, low-cost policies under some conditions}\\
&\Downarrow\\
&\text{Cue-triggered repetition and habit persistence}\\
&\Downarrow\\
&\text{Potential displacement of reflective long-term objectives}
\end{aligned}
$$

This is not a deterministic law that every low-energy action is selected. The system also considers reward, risk, uncertainty, social demands, bodily needs, and learned goals.

### Conditional model result 3 — Local-score selection can conflict with a reflective goal

**Statement:** In a specified action-selection model, a habitual policy can be selected more often than a deliberative policy even when the latter has greater reflective long-term value, if the model's local score favours the habitual policy.

**Derivation:**

1. Let $G$ be a reflective long-term goal, and let $\Pi_h$ and $\Pi_m$ be feasible habitual and deliberative policies.
2. Suppose $\Pi_m$ has greater value under the reflective long-term objective, while the local action score includes immediate value and control costs defined on a commensurable scale.
3. Suppose the resulting local scores satisfy $Q(\Pi_h)>Q(\Pi_m)$.
4. Under a finite-action softmax selector with fixed inverse-temperature $\beta>0$, this inequality makes $\Pi_h$ more probable than $\Pi_m$. A greedy selector chooses $\Pi_h$ only if it is a maximizer over the full feasible action set.
5. Therefore, the specified model can favour a locally higher-scoring policy that conflicts with the reflective long-term objective.

This is a conditional result about the model's score and selector, not a derivation of the physical-to-behavioural bridge or an explanation of any individual's parameters. Repeated selection strengthens a cue-policy association only if a separate learning/update rule entails that change; no such rule is specified here.

**Claim-linked evidence register records:** R13, R14, R15, R60, R63. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 27. What the physical bridge predicts

The model predicts that unwanted habitual behaviour should become more likely when:

- the habitual cue is highly accessible;
- the habitual action has low initiation cost;
- the competing task has high uncertainty or effort;
- the person is fatigued or under stress;
- the task's reward is delayed;
- the habitual action reliably provides immediate relief or stimulation;
- the environment makes the alternative action difficult to initiate.

It also predicts that changing the environment can improve behaviour even before the underlying urge disappears.

This is a major practical consequence: self-control can be improved by changing the transition structure of the environment, not only by strengthening conscious resistance.

---

**Claim-linked evidence register records:** R13, R15, R23, R26, R29, R30, R33, R34. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.

# PART VI — INVESTIGATION A: FOUNDATIONS OF INTELLIGENCE


## 28. Research question A1: What constitutes context?

Context is not merely whatever is outside the mind. It is any information-bearing or constraint-bearing condition that changes the system's possible interpretations or transitions.

Formally, let the transition distribution be:

$$
P(X_{t+1}\mid X_t,A,M_t,C_t)
$$

A variable $C_t$ is contextually relevant if changing it changes the distribution of possible next states, interpretations, or actions.

A context can be:

- sensory;
- bodily;
- social;
- temporal;
- mathematical;
- linguistic;
- remembered;
- goal-related;
- architectural.

A variable that has no causal, informational, or computational influence on the system's relevant operation is not contextually relevant for that operation.

### Context decomposition

Define:

$$
C_t=(C_t^{\mathrm{ext}},C_t^{\mathrm{int}},C_t^{\mathrm{struct}},C_t^{\mathrm{goal}})
$$

where:

- $C^{\mathrm{ext}}$: external observations;
- $C^{\mathrm{int}}$: internal memory and active representations;
- $C^{\mathrm{struct}}$: architecture and formal constraints;
- $C^{\mathrm{goal}}$: objectives and evaluation criteria.

This decomposition resolves the ambiguity in the phrase "no context." A system can have no new external context while retaining internal, structural, and goal context.

**Claim-linked evidence register records:** R30. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 29. Research question A2: Can meaningful inference occur with zero external input?

Yes, if "zero external input" means no new external observation during the inference interval, while internal state and rules remain available.

Let the inference state be $Z=(A,M,X)$. A computation is:

$$
Y=\mathcal{I}(Z)
$$

If $Z$ is nontrivial, $\mathcal{I}$ can produce a result not explicitly stored in $M$.

Examples include:

- deriving a mathematical theorem;
- proving a contradiction from assumptions;
- calculating a consequence of a physical model;
- simulating a possible future;
- composing a new plan from remembered components.

If the phrase means no information, no structure, no state, and no rules whatsoever, then there is no defined inference process. The premise removes the conditions required for the operation.

### Proposition 4 — Internal inference requires structure, not fresh sensory input

A nontrivial inference can occur without new sensory input if the system has an internal state and a transformation rule capable of producing a distinct output.

This proposition follows directly from the definition of computation. It does not imply that the result is true about the external world.

**Claim-linked evidence register records:** R02, R05, R21, R22. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 30. Research question A3: What is the relationship between prior information and genuinely novel knowledge?

The answer depends on what "new" means.

Let $K$ be the system's prior knowledge and $p$ a proposition.

- $p$ is **newly represented** if the system did not previously encode it explicitly.
- $p$ is **deducible** if $K\models p$.
- $p$ is **probabilistically supported** if $P(p\mid K)$ is high under a calibrated model.
- $p$ is **empirically new** if it identifies a feature of the world not previously established by the relevant community or system.
- $p$ is **information-independent** if its truth is not constrained by $K$.

A proposition can be newly represented and deducible. It can be empirically new while being structurally implied by existing evidence. It cannot be uniquely deduced from premises that leave it unconstrained.

### Information conservation and inferential novelty

A deterministic computation does not create information about an arbitrary external variable from nothing. However, it can expose information that was implicit in a compressed representation.

For example, a compact set of axioms can entail an enormous number of theorems. The theorems are not necessarily stored as explicit strings in the axioms. Their consequences are generated by the inferential structure.

In algorithmic terms, a short program can generate a long output. The output may be novel and complex relative to the observer, even though its generation is determined by the program and input.

This distinction is central to Out of Box Theory:

$$
\boxed{\text{Novel output}\not\Rightarrow\text{information from nothing}}
$$

and:

$$
\boxed{\text{Implicit consequence}\not\Rightarrow\text{explicit prior representation}}
$$

**Claim-linked evidence register records:** R01, R05, R21, R22, R03. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 31. Research question A4: What are the physical limits of information processing?

There is no single universal number that describes all computational limits. Several distinct constraints apply:

1. **Energy cost:** computation requires physical state transitions and, for logically irreversible operations under standard assumptions, erasure has a Landauer lower bound.
2. **Time cost:** a physical system has finite speed and must perform state transitions over time.
3. **Memory capacity:** a finite substrate can maintain only a finite number of distinguishable stable states under specified physical conditions.
4. **Noise:** physical systems are subject to thermal, quantum, and implementation noise.
5. **Communication:** information transfer is constrained by bandwidth, distance, and signal propagation.
6. **Error correction:** reliable computation requires redundancy or error management, which itself consumes resources.
7. **Causal access:** a system cannot use information from events outside its causal access.

The Landauer bound for erasing one unbiased bit is:

$$
E_{\mathrm{erase}}\geq k_BT\ln 2
$$

under the standard isothermal assumptions. This is not a lower bound on every logical operation. Reversible computation can, in principle, avoid the same erasure cost, though practical implementation has other costs.

The brain's actual energy expenditure per useful inference is vastly more complex than the idealized one-bit bound. The bound establishes a physical floor for a particular operation, not a direct conversion factor from thoughts to joules.

### A useful resource vector

Represent a system's resource state by:

$$
\mathcal{R}=(E,T_m,B,M_c,\varepsilon)
$$

where:

- $E$: available energy;
- $T_m$: available computation time;
- $B$: communication bandwidth;
- $M_c$: memory capacity;
- $\varepsilon$: tolerated error probability.

An intelligent system's achievable performance is a function of all five:

$$
\mathcal{P}_{\max}=\Phi(\mathcal{R},A,\text{task})
$$

This is a general engineering relation. It says that intelligence as implemented by a physical system is constrained by its substrate and task.

**Claim-linked evidence register records:** R09, R10, R11, R13, R14, R60, R61, R62. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 32. Research question A5: Can intelligence be mathematically distinguished from computation?

Not by the mere fact that a system computes. Intelligence requires additional functional properties.

A minimal computational system can execute a fixed mapping. An adaptive intelligent system must generally exhibit some combination of:

- internal state representation;
- learning or model revision;
- generalization to new conditions;
- prediction;
- goal-sensitive action selection;
- error correction;
- transfer across tasks;
- self-monitoring or adaptive control.

A useful operational distinction is:

$$
\text{Computation}=\text{state transformation}
$$

$$
\text{Intelligence}=\text{adaptive use of state transformation to model, predict, or control under changing conditions}
$$

This is not the only possible definition of intelligence. It is a definition chosen for the present framework.

### Proposed Intelligence Functional

Define an operational intelligence score:

$$
\mathcal{I}
=
w_1G+w_2A_d+w_3P+w_4T_r+w_5R_c
$$

where:

- $G$: generalization;
- $A_d$: adaptation to changed conditions;
- $P$: predictive accuracy;
- $T_r$: transfer across tasks;
- $R_c$: recovery and correction after error;
- $w_i$: task-dependent weights.

This is a candidate measurement proposal, not a validated intelligence scale or a universal natural constant. The components may overlap and may not share a common measurement scale. Before aggregation, each component requires defined observable indicators, task sampling, scoring direction, normalization, reliability, construct and criterion validity, and tests of discriminant validity against established cognitive-ability measures. The weights $w_i$ cannot be selected solely by intuition: they require a prespecified rationale and out-of-sample validation. A compensatory weighted sum may also conceal a serious weakness in one component behind high scores in another, so component profiles and uncertainty should be reported alongside any composite. Memory, processing speed, prior training, domain knowledge and opportunity to learn must be measured or controlled where relevant.

**Claim-linked evidence register records:** R27, R58, R59. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 33. The unified result of Investigation A

The five questions yield the following conclusions:

1. Context includes external, internal, structural, and goal-related constraints.
2. Inference can continue without new external input when internal state and rules remain.
3. Novel conclusions can be derived from implicit structure, but arbitrary unconstrained facts cannot be uniquely inferred.
4. Physical information processing is bounded by energy, time, memory, bandwidth, noise, and causality.
5. The framework provisionally defines intelligence as adaptive, model-based use of computation under changing conditions.

**Investigation A yields a provisional conceptual synthesis, not a resolved or validated theory.** Its formal claims remain conditional, its proposed intelligence measure is unvalidated, and its empirical adequacy depends on operationalization, comparison with established alternatives, and prospective testing.

---

# PART VII — INVESTIGATION B: MECHANICS OF BEHAVIOURAL CONTROL

## 34. Research question B1: How are cue-response associations learned?

A cue-response association can be learned when a cue reliably predicts an outcome or when an action following the cue produces a consequential result.

Let $s_t$ include the cue and other state variables, $a_t$ be the selected action, $r_{t+1}$ be the outcome received after that action, and $Q_{\mathrm{RL},t}(s_t,a_t)$ be the estimated action value.

A candidate off-policy action-value update is the Q-learning rule specified in §22, with the cue included in the state representation. It uses the outcome received after the action and the estimated value of the best feasible next action. It is not interchangeable with a generic scalar prediction-error expression: the state, action, reward timing and bootstrap target must be defined consistently.

Repeated cue-action-outcome sequences may increase the estimated value or readiness of a policy under an appropriate learning rule. Whether this produces a human habit, and how it interacts with goal-directed control, requires a separate behavioural and neural model.

A more complete model must include:

- cue salience;
- action availability;
- reward magnitude;
- reward delay;
- uncertainty;
- stress;
- physiological state;
- competing actions;
- the history of reinforcement;
- whether the outcome is valued or merely relieving.

The simple update equation is a useful starting abstraction, not a complete neuronal mechanism.

**Claim-linked evidence register records:** R16, R18, R19, R23, R26, R28, R30, R53. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 35. Research question B2: How do reward anticipation and habit formation interact?

Reward anticipation can influence action before the reward is received. Habit formation can make the action less dependent on a fresh evaluation of its outcome.

The two mechanisms can interact:

1. A cue predicts an attractive or relieving outcome.
2. The cue acquires motivational significance.
3. The associated action is repeated.
4. Repetition makes the action more readily executable.
5. The action can be initiated even when the person no longer values the outcome as highly as before.

This helps explain why wanting and liking can diverge.

The system can retain a strong action tendency even when the actual pleasure is modest.

### Model-based and model-free control

A model-based controller estimates consequences:

$$
Q_{\mathrm{MB}}(s,a)
=
\mathbb{E}\left[
r+\gamma V(s')\mid s,a,\widehat{T}
\right]
$$

where $\widehat{T}$ is an internal model of state transitions.

A model-free controller uses cached values:

$$
Q_{\mathrm{MF}}(s,a)
$$

A simple arbitration model is:

$$
Q_{\mathrm{combined}}
=
\omega(s)Q_{\mathrm{MB}}
+
[1-\omega(s)]Q_{\mathrm{MF}}
$$

where $\omega(s)$ represents the degree to which model-based control is used in state $s$.

The weight can depend on uncertainty, effort, fatigue, reliability, and task demand. The model is a useful computational abstraction; it should not be interpreted as a literal single switch in the brain.

**Claim-linked evidence register records:** R13, R14, R15, R16, R18, R19, R23, R24, R25, R26, R28, R30, R43, R44, R53, R62, R63. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 36. Research question B3: How does cognitive control compete with automatic behaviour?

Cognitive control supports the maintenance of goals, inhibition of competing responses, task switching, and correction of errors.

Automatic behaviour reduces the need for repeated deliberation.

Neither system is universally superior.

A useful controller must arbitrate between them.

Let:

- $C_{\mathrm{MB}}$: cost of model-based evaluation;
- $C_{\mathrm{MF}}$: cost of executing a cached policy;
- $U_{\mathrm{MB}}$: expected value of deliberative control;
- $U_{\mathrm{MF}}$: expected value of cached control.

Choose model-based control when:

$$
U_{\mathrm{MB}}-C_{\mathrm{MB}}
>
U_{\mathrm{MF}}-C_{\mathrm{MF}}
$$

Choose cached control when the inequality reverses.

The problem occurs when the cached policy remains cheap and strongly cued despite being misaligned with the reflective objective.

### Control arbitration proposition

A system should allocate more control to deliberative evaluation when:

- the environment has changed;
- the habitual response has become unreliable;
- the consequences are high;
- uncertainty is large;
- the current goal conflicts with the cached policy;
- the cost of an error exceeds the cost of deliberation.

This yields a design principle: do not demand maximum deliberation for every action. Demand it where the expected value of correction justifies its cost.

**Claim-linked evidence register records:** R13, R15, R24, R25, R43, R44, R62, R63. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 37. Research question B4: How do sleep, stress, and environmental conditions alter action selection?

The action-selection equation already contains state-dependent terms. Sleep, stress, and environment can change:

- available control resources;
- reward sensitivity;
- perceived effort;
- working-memory reliability;
- response inhibition;
- cue salience;
- the probability of detecting an error;
- the cost of initiating a task.

Let $\phi_t$ represent physiological context, distinct from the task-demand variable $z_t$ used in §39. Then:

$$
Q(a\mid s,\phi_t)
=
R(a\mid s,\phi_t)-C(a\mid s,\phi_t)
$$

The same action can have different effective values under different physiological conditions.

A difficult task may be manageable after adequate sleep but disproportionately costly under fatigue. A familiar distraction may then win more often.

This does not establish that every focus problem is caused by sleep or stress. It establishes that they are plausible state variables that should be measured rather than ignored.

**Claim-linked evidence register records:** R25, R43, R44. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 38. A multi-timescale model of unwanted loops

Behavioural control operates across several timescales:

| Timescale | Process | Example |
|---|---|---|
| Milliseconds–seconds | Cue detection and response competition | Notification captures attention |
| Seconds–minutes | Action selection and immediate reinforcement | Checking the phone |
| Hours–days | Repeated routines and state-dependent learning | Studying becomes associated with scrolling |
| Weeks–months | Habit consolidation and environmental adaptation | Automatic phone checking |
| Months–years | Identity, goals, health, and life structure | Persistent avoidance of academic work |

These bands are illustrative, not empirically fixed boundaries or a universal sequence. Processes can overlap and operate concurrently; the relevant time horizon depends on the target behaviour and decision being studied.

An intervention should be designed with the relevant mechanism's timescale in view. This is a design heuristic, not a validated universal rule. A brief inhibition technique may interrupt an immediate response, but it does not by itself establish lasting environmental change or resolve an underlying sleep disorder. No multistable attractor landscape, basin geometry or transition-barrier model is specified in this treatise; those analyses are deferred until a concrete state space and transition law exist.

**Claim-linked evidence register records:** R28, R30, R38, R49. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.

## 39. The full behavioural-loop model

Let the state vector be:

$$
s_t=(g_t,c_t,u_t,f_t,z_t,h_t)
$$

where:

- $g_t$: active goal;
- $c_t$: cue state;
- $u_t$: urge or motivational activation;
- $f_t$: perceived fatigue (ordinal self-rating); any objective physiological measure is a separate variable and is not represented by $f_t$;
- $z_t$: task difficulty and uncertainty;
- $h_t$: learned habit strength.

The probability of executing a competing action can be modelled as:

$$
P(a_h\mid s_t)
=
\sigma\left(
b_0+b_1c_t+b_2u_t+b_3f_t+b_4z_t+b_5h_t-b_6g_t
\right)
$$

where $\sigma(x)=1/(1+e^{-x})$ is the logistic function.

This is a proposed statistical model, not a fitted or validated model. Its linear predictor treats the ordinal ratings as numeric inputs and therefore assumes meaningful equal spacing unless recoded; categorical, monotone or nonlinear alternatives should be compared. Repeated observations require a design and analysis that account for within-person, day/block clustering and temporal dependence. The coefficients must be estimated from observations; the model does not assert that all factors act linearly or independently.

The key point is that an unwanted action is a function of a state, not a mysterious failure of character.

**Claim-linked evidence register records:** R27, R42, R44. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 40. The unified result of Investigation B

1. Cue-response associations are learned through predictive and reinforcing interactions.
2. Reward anticipation can motivate behaviour even when actual pleasure is limited.
3. Habits cache policies and reduce repeated deliberation costs.
4. Cognitive control and automatic action selection compete and are arbitrated according to value, cost, reliability, and state.
5. Sleep, stress, task difficulty, and environmental structure can shift the balance.

This provides a mechanistic account of why a person may know what to do yet repeatedly do something else.

---

**Claim-linked evidence register records:** R16, R19, R23, R26. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.

# PART VIII — INVESTIGATION C: RECURSIVE INTELLIGENCE AND SELF-MASTERY


## 41. Research question C1: Can trigger-specific interventions improve sustained attention?

Yes, in principle, because the model identifies state variables that can be changed before or during action selection.

A trigger-specific intervention changes one or more of:

- cue probability;
- cue salience;
- response accessibility;
- action initiation cost;
- expected immediate reward;
- task uncertainty;
- alternative-response availability;
- control demand.

Suppose the unwanted action has score:

$$
Q_h=R_h-C_h
$$

and the desired action has score:

$$
Q_g=R_g-C_g
$$

A successful intervention need not eliminate $R_h$. It can reduce the accessibility of the cue, increase the cost of the habitual action, reduce the initiation cost of the goal action, or improve the expected value of the goal action.

The objective is to create:

$$
Q_g-Q_h>0
$$

in the relevant states often enough for the desired policy to become practised and reliable.

### Four intervention classes

1. **Antecedent intervention:** change the conditions before the cue appears.
2. **Response interruption:** insert a delay or alternative action after cue detection.
3. **Consequence redesign:** alter what reinforces the action.
4. **Policy retraining:** practise a new response until it becomes accessible.

Trigger-specific plans are particularly useful because they connect a known state to a preselected response.

**Claim-linked evidence register records:** R31, R32, R33, R34, R48. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 42. Research question C2: How quickly do alternative responses become established?

There is no universal number of days. Learning rate depends on:

- frequency of cue exposure;
- consistency of the alternative response;
- reward and relief structure;
- cue strength;
- stress and sleep;
- task complexity;
- prior learning;
- environmental stability;
- individual differences.

A simple learning curve can be represented as:

$$
H_{t+1}=H_t+\alpha(1-H_t)R_t-\beta H_tN_t
$$

where:- $H_t$ is the strength of the new habit;
- $\alpha$ is a learning parameter;
- $R_t$ represents successful rehearsal;
- $\beta$ is a weakening parameter;
- $N_t$ represents non-reinforcement or competing learning.

This is a proposed model, not a validated universal law of habit acquisition. A bounded interpretation requires $H_t$ to remain within a defined range (for example, $[0,1]$) and parameter/input constraints that preserve that range; these constraints and parameters have not been identified here.

It predicts diminishing increments as $H_t$ approaches an upper bound, provided successful rehearsal continues.

A new response becomes more reliable through repeated execution in the relevant context, not merely through repeated verbal intention.

**Claim-linked evidence register records:** R16, R18, R19, R26, R28, R29, R30, R53. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 43. Research question C3: Which environmental changes produce the largest improvements?

The model predicts the greatest benefit from interventions that change high-leverage variables:

- remove or reduce cues with strong learned associations;
- increase friction for unwanted actions;
- decrease friction for desired actions;
- separate contexts associated with incompatible behaviours;
- make the next desired action immediately visible;
- reduce uncertainty about how to begin;
- protect sleep and recovery;
- create predictable work periods;
- reduce the number of decisions required at task initiation.

The best intervention is not necessarily the most severe. It is the intervention that produces the largest improvement at acceptable cost and can be maintained.

### Environmental leverage ratio

Define:

$$
\Lambda=
\frac{\text{reduction in unwanted-action probability}}
{\text{implementation cost}}
$$

A high-$\Lambda$ intervention is intended to represent a large reduction in unwanted-action probability relative to its implementation burden. To estimate it, define the baseline/comparator, eligible-opportunity denominator, observation window and burden scale in advance. If implementation cost is zero, the ratio is undefined; if the probability reduction is negative, the result indicates worsening rather than benefit. Comparisons across interventions require a common cost scale. This is an exploratory heuristic, not a validated universal or clinical score.

**Claim-linked evidence register records:** R33, R34. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 44. Research question C4: How can behavioural recovery be measured?

The number of urges is not a sufficient measure of self-mastery. A person can experience many urges yet respond effectively.

Useful metrics include:

1. **Goal adherence:** proportion of planned work intervals in which the intended task is maintained.
2. **Distraction frequency:** number of unplanned shifts per unit time.
3. **Distraction duration:** time spent in the competing action.
4. **Return-to-task latency:** time between noticing a distraction and resuming the intended task.
5. **Cue-response success:** proportion of trigger encounters followed by the planned alternative.
6. **Initiation latency:** time between planned start and actual task engagement.
7. **Sleep regularity:** consistency of sleep and wake timing.
8. **Functional outcome:** actual work completed, not just time spent at a desk.

A useful composite measure is:

$$
\mathcal{C}
=
w_1A_g-w_2F_d-w_3D_d-w_4L_r+w_5S_c
$$

where:

- $A_g$: goal adherence;
- $F_d$: distraction frequency;
- $D_d$: distraction duration;
- $L_r$: return-to-task latency;
- $S_c$: successful cue-response substitutions.

The weights must be selected for the task, and the component measures require prespecified direction, time window and scaling before they can be combined. Without commensurable scales, the weighted sum is not interpretable as a coherent quantity. The composite is exploratory, not validated; a composite score should never conceal the underlying measurements.

**Claim-linked evidence register records:** R27, R38, R41, R42, R44, R47, R50. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 45. Research question C5: How can the protocol adapt to individual differences?

The controller must estimate the person's own state rather than assume every distraction has the same cause.

A system can use a repeated loop:

$$
\text{Observe}\rightarrow\text{Estimate}\rightarrow\text{Intervene}
\rightarrow\text{Measure}\rightarrow\text{Update}
$$

For each episode, record:

- what happened before the distraction;
- the task being attempted;
- the internal state (boredom, uncertainty, fatigue, anxiety, urge);
- the competing action;
- the immediate consequence;
- the time needed to return;
- the intervention attempted.

Over time, this produces an individualized model of the person's cue-response structure.

A person whose main trigger is task ambiguity needs a different intervention from someone whose main trigger is sleep deprivation or a highly accessible device.

The protocol must be adaptive, not dogmatic.

---

**Claim-linked evidence register records:** R27, R29, R30, R38, R41, R42, R47, R50. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.

# PART IX — RECURSIVE INTELLIGENCE: FORMAL SELF-MODIFICATION


## 46. From ordinary intelligence to recursive intelligence

Ordinary adaptive intelligence changes its internal model in response to external feedback.

Recursive Intelligence adds a further operation: the system represents aspects of its own processing and uses those representations to change its future operation.

Let:

- $S_t$: current system state;
- $I_t$: incoming information;
- $G_t$: goal state;
- $C_t$: control state;
- $\widehat{S}_t$: the system's estimate of its own state;
- $\Theta_t$: parameters governing future behaviour.

Then:

$$
\widehat{S}_t=
\mathcal{M}_{\psi}(O_{0:t},A_{0:t-1},r_{1:t})
$$

$$
\Theta_{t+1}=
U_{\Theta}(\Theta_t,\widehat{S}_t,G_t,\text{error}_t,\text{feedback}_t)
$$

$$
S_{t+1}=F_{\Theta_{t+1}}(S_t,I_t)
$$

Here $S_t$ is generally latent; the estimator receives an observation/action/outcome history rather than direct access to the true state. $U_{\Theta}$ is an unspecified update operator, not an identified learning algorithm. Its parameter domain, constraints, objective, uncertainty and update cadence must be defined before the expression can be treated as an executable model.

The system is not merely processing the world. It is processing information about its own processing. However, monitoring and updating parameters are also found in metacognition, meta-control and adaptive control. A distinct recursive mechanism would require an explicit meta-level representation or operation on the controller/update process and a discriminating prediction beyond those established alternatives.

**Claim-linked evidence register records:** R24, R35, R36, R37, R39, R51, R54, R55. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 47. The recursive loop

$$
\boxed{
\begin{aligned}
&\text{World observation}\\
&\downarrow\\
&\text{Internal model}\\
&\downarrow\\
&\text{Prediction and action}\\
&\downarrow\\
&\text{Outcome measurement}\\
&\downarrow\\
&\text{Self-model update}\\
&\downarrow\\
&\text{Policy modification}\\
&\downarrow\\
&\text{Changed future action}
\end{aligned}
}
$$

A feedback loop in which outcomes modify later parameters is already a standard feature of adaptive control and reinforcement learning. The diagram therefore illustrates recursive feedback in a broad descriptive sense; by itself it does not establish a distinct Recursive Intelligence mechanism. Distinctiveness would require a specified meta-level representation or operation on the controller's own update process, plus a prediction that ordinary adaptive-control and metacognitive models do not already make.

**Claim-linked evidence register records:** R35, R37, R39, R51, R54, R55. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 48. The self-model must be fallible

A recursive system can misestimate itself.

It may:

- misidentify a trigger;
- attribute a failure to the wrong cause;
- overestimate its control capacity;
- choose an intervention that increases stress;
- optimize a misleading metric;
- confuse short-term compliance with long-term improvement.

Therefore, self-monitoring must be checked against observable outcomes.

The system should not merely ask, "Why did I fail?" It should ask, "Which explanation best predicts what will happen under a controlled change?"

This turns self-reflection into model testing.

**Claim-linked evidence register records:** R35, R36, R37, R51, R54, R55. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 49. A formal objective for recursive control

Let $\pi$ be a behavioural policy. Define:

$$
J(\pi)=
\mathbb{E}\left[
\sum_{t=0}^{T}
\gamma^t
\left(
R_G(s_t,a_t)
-\lambda C(a_t)
-\mu H(a_t)
\right)
\right]
$$

where:

- $R_G$: reward or progress relative to the chosen goal;
- $C(a_t)$: energetic, cognitive, or practical cost;
- $H(a_t)$: harm or risk;
- $\lambda,\mu$: weights;
- $\gamma$: discount factor.

The expectation is over trajectories generated by a specified policy and transition model over the finite horizon $T$. The objective is only interpretable after the time step, reward/cost/harm scales, weights, constraints and treatment of uncertainty are defined. Costs and rewards expressed in different units require a justified conversion or normalization.

A parameter update of the form

$$
\pi_{t+1}=\operatorname{Update}(\pi_t,\widehat{\nabla J},\text{feedback})
$$

is only a gradient-based method if $\pi$ has a suitable parameterization, $J$ is differentiable with respect to those parameters, and the gradient estimator is specified. Otherwise, this is merely a placeholder for a general policy-update operator. No algorithm or convergence property is specified here.

The gradient notation is conceptual. Human self-regulation is not necessarily gradient descent in a literal neural implementation.

A critical safeguard is that the goal function itself must be reviewable. An intelligent system can optimize the wrong objective with great efficiency.

**Claim-linked evidence register records:** R35, R37, R51, R54, R55. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 50. Goal hierarchy and the reflective controller

A person may have several levels of goals:

- immediate impulse;
- current task;
- daily plan;
- long-term objective;
- values and identity commitments.

These goals can conflict.

Represent the hierarchy as:

$$
G_0\prec G_1\prec G_2\prec G_3
$$

where higher levels constrain or evaluate lower-level goals.

The displayed chain is one illustrative ordering, not a universal or necessarily total hierarchy. Some goals may be incomparable, mutually constraining or context-dependent; a general model would require a partial-order or explicit conflict-resolution rule. A higher-level goal may also be revised when evidence, health or circumstances change.

Self-mastery is not blind obedience to an old plan. It is the capacity to maintain coherent priorities while permitting justified revision.

---

**Claim-linked evidence register records:** R35, R37, R51, R54, R55. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.

# PART X — ROOT CONTROL PROTOCOL: MATHEMATICAL ARCHITECTURE


## 51. The protocol's role

The ROOT Control Protocol is the operational layer of the unified framework.

It is designed to alter the conditions that generate unwanted action, rather than relying solely on a last-second act of resistance.

The seven components are:

- **R — Recognise**
- **O — Obstruct**
- **O — Override**
- **T — Train**
- **C — Correct**
- **O — Optimise**
- **L — Learn**

The protocol is a behavioural engineering architecture, not a claim that all unwanted behaviour can be eliminated by one universal routine.

**Claim-linked evidence register records:** R28, R34. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 52. State estimation

Let the measured state be:

$$
s_t=(c_t,u_t,f_t,d_t,g_t,h_t,e_t)
$$

where:

- $c_t$: cue intensity;
- $u_t$: urge intensity;
- $f_t$: fatigue or physiological load;
- $d_t$: task difficulty or ambiguity;
- $g_t$: goal activation;
- $h_t$: habit strength;
- $e_t$: environmental accessibility of the competing action.

The system estimates $s_t$ using observation and reflection. The estimate need not be perfect; it must be good enough to select a useful intervention. Here $f_t$ is an ordinal self-rating of perceived fatigue, not an objective physiological measurement. In the reduced six-variable model in §39, $z_t$ denotes task demand/difficulty and uncertainty and corresponds only approximately to $d_t$ here; the ROOT vector additionally records competing-action accessibility as $e_t$. The seven ratings remain ordinal and are not assumed to be equally spaced or directly additive.

**Claim-linked evidence register records:** R27. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 53. R — Recognise

The recognition stage detects the earliest reliable signal of the unwanted sequence.

A trigger record can be represented as:

$$
\mathcal{E}_t=(\text{cueID}_t,s_t,a_t,r_t,\tau_t,\mathrm{RTL}_t,\iota_t)
$$

where:

- $\text{cueID}_t$: identifier/description of the trigger or cue context (distinct from the cue-intensity rating $c_t$ inside $s_t$);
- $s_t$: state;
- $a_t$: action taken;
- $r_t$: immediate consequence;
- $\tau_t$: duration.
- $\mathrm{RTL}_t$: return-to-task latency, measured from noticing the diversion to resuming the intended task.
- $\iota_t$: intervention applied during the episode (including no intervention).

Recognition must distinguish the trigger from the behaviour. "I used my phone" is a behaviour description. "I reached for my phone immediately after encountering an ambiguous problem and feeling frustrated" is a potentially useful trigger description.

**Claim-linked evidence register records:** R27, R38, R41, R42, R47, R50, R53. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 54. O — Obstruct

Obstruction changes the transition structure before the habitual response is executed.

Let $p_h(s)$ be the probability of the unwanted action in state $s$. Environmental obstruction changes action accessibility:

$$
e'_t<e_t
$$

and ideally:

$$
p_h(s\mid e'_t)<p_h(s\mid e_t)
$$

Examples:

- place the phone outside the study area;
- disable nonessential notifications;
- block selected applications during planned work;
- remove visual cues;
- use a separate work environment;
- prepare materials before beginning;
- reduce the number of steps needed to start the intended task.

Obstruction is not punishment. It is system design.

**Claim-linked evidence register records:** R33, R34. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 55. O — Override

Override inserts a preselected response between the cue and the habitual action.

An implementation intention is:

$$
\text{If }c\text{ occurs, execute }a_{\mathrm{alt}}
$$

For example:

> If I notice that I am about to open a distracting application during a study block, I will leave the device untouched, identify the next physical step in the study task, and perform that step for two minutes.

The alternative must be concrete and executable. "Be disciplined" is not an action specification.

**Claim-linked evidence register records:** R31, R32, R48, R65. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 56. T — Train

Training repeats the alternative response in the relevant context.

The training objective is not to suppress every urge. It is to increase the probability that the alternative action is selected when the trigger occurs.

Let $H_{\mathrm{alt}}$ represent the strength of the alternative response. A simple update is:

$$
H_{\mathrm{alt},t+1}
=
H_{\mathrm{alt},t}
+
\alpha S_t
-
\beta F_t
$$

where:

- $S_t$: successful practice;
- $F_t$: failure or competing reinforcement;
- $\alpha,\beta$: learning parameters.

The equation is a conceptual learning model. It has no specified state bounds, context-transfer rule or empirically identified parameters, and it does not imply that one failure erases progress.

**Claim-linked evidence register records:** R16, R18, R19, R26, R28, R29, R30, R53. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 57. C — Correct

Correction uses outcome data to identify whether the intervention worked.

Let $y_t$ be the observed outcome and $y_t^*$ the desired outcome:

$$
\varepsilon_t^{\mathrm{out}}=y_t^*-y_t
$$

The intervention is adjusted according to the error and its likely cause.

Examples:

- If the phone remains accessible, strengthen obstruction.
- If the task is ambiguous, define the next action more clearly.
- If fatigue dominates, address sleep and workload.
- If the alternative is too demanding, simplify it.
- If the urge is strong but brief, use a delay and return-to-task routine.
- If the behaviour is compulsive and impairing, seek appropriate clinical assessment rather than escalating self-punishment.

**Claim-linked evidence register records:** R40. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 58. O — Optimise

Optimisation addresses the biological and environmental conditions that influence the controller.

Relevant variables include:

- sleep regularity and adequacy;
- physical activity;
- nutrition and hydration;
- workload;
- study environment;
- task difficulty;
- recovery periods;
- social and emotional stress.

The objective is not to maximize productivity at all times. It is to maintain a state in which chosen goals can be pursued without chronic depletion.

**Claim-linked evidence register records:** R25, R30, R43, R44. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 59. L — Learn

Learning consolidates the system's revised policy.

The controller compares:

- predicted trigger;
- actual trigger;
- selected response;
- immediate consequence;
- delayed consequence;
- functional outcome.

It then updates the personal model.

This closes the recursive loop:

$$
\text{Recognise}\rightarrow
\text{Obstruct}\rightarrow
\text{Override}\rightarrow
\text{Train}\rightarrow
\text{Correct}\rightarrow
\text{Optimise}\rightarrow
\text{Learn}
$$

The output of one cycle becomes the context for the next cycle.

---

# PART XI — STABILITY, CONVERGENCE, AND LIMITS

## 60. What would it mean for self-mastery to become stable?

A stable behavioural system does not require constant high motivation. It has environmental and internal arrangements that make the desired behaviour more likely across ordinary fluctuations.

Let $x_t$ represent deviation from the intended behavioural state. A simple discrete-time control model is:

$$
x_{t+1}=A_{\mathrm{plant}}x_t+B_{\mathrm{plant}}u_t+w_t
$$

where:

- $A_{\mathrm{plant}}$: uncontrolled plant dynamics;
- $B_{\mathrm{plant}}$: effect of the control intervention;
- $u_t$: intervention;
- $w_t$: disturbances.

A feedback controller may choose:

$$
u_t=-K_{\mathrm{fb}}x_t
$$

giving:

$$
x_{t+1}=(A_{\mathrm{plant}}-B_{\mathrm{plant}}K_{\mathrm{fb}})x_t+w_t
$$

In a linear model without disturbances, stability requires the eigenvalues of $A_{\mathrm{plant}}-B_{\mathrm{plant}}K_{\mathrm{fb}}$ to lie inside the unit circle.

Human behaviour is nonlinear, partially observed, and state-dependent. The linear model is an approximation useful for understanding feedback, not a literal complete brain model.

**Claim-linked evidence register records:** R40. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 61. Lyapunov-style formulation

Let $V(x)$ measure deviation from the desired behavioural state. A stable controller aims for:

$$
V(x_{t+1})-V(x_t)<0
$$

for states outside an acceptable region, subject to disturbances and constraints.

A practical candidate is:

$$
V(x)=
w_1(\text{goal deviation})^2+
w_2(\text{unwanted habit activation})^2+
w_3(\text{return latency})^2
$$

The intervention should reduce expected $V$ over repeated cycles.

This gives a possible way to operationalize improvement, not yet a rigorous stability certificate. The displayed $V(x)$ is a candidate monitoring functional over selected proxies; the treatise has not shown that those proxies form a complete state, that the weights make $V$ positive definite, or that the actual transition law decreases it. It must not be called a verified Lyapunov function. Improvement can be reported descriptively without claiming stability.

**Claim-linked evidence register records:** R40. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 62. Behavioural improvement under feedback — testable hypothesis, not a stability theorem

**Hypothesis:** Within a defined operating domain, reliable trigger detection, an available alternative response, an intervention that changes action selection in the intended direction, reinforcement of successful responses, and bounded/manageable disturbances may be associated with a reduction in the expected frequency or duration of the unwanted response.

**Rationale (not a proof):** These conditions identify plausible components of a feedback intervention. They do not, by themselves, establish that the expected behavioural state has negative drift. Changes in opportunity, substitution, measurement, competing goals or later disturbances may offset local improvements.

A mathematical stability result would require a defined state and target set, an explicit transition/update law, a positive-definite candidate measure where a Lyapunov argument is used, and a quantified deterministic decrease or stochastic conditional-drift inequality with appropriate disturbance and invariance assumptions. Those requirements are not supplied by the present protocol description.

This is therefore a behavioural hypothesis, not a formal guarantee. If the operating conditions are exceeded or the behaviour is persistently distressing or impairing, the protocol may be insufficient and professional assessment may be appropriate.

**Claim-linked evidence register records:** R40. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 63. Why no universal guarantee is mathematically justified

A guaranteed cure would require a controller that can overcome every possible disturbance, every biological condition, every environmental change, and every competing objective.

A bounded-actuation controller cannot guarantee target-state maintenance for every possible disturbance in a specified plant if the disturbance set is unrestricted. For example, in $x_{t+1}=x_t+u_t+w_t$ with $|u_t|\leq U$ and no bound on $w_t$, a disturbance can always be chosen large enough to drive the next state outside any fixed bounded target region. This counterexample establishes a limitation for that plant/controller/disturbance class; it does not show that every finite controller fails under bounded disturbances or within a defined operating domain.

A system can encounter:

- illness;
- sleep deprivation;
- trauma;
- severe stress;
- changing obligations;
- medication effects;
- neurological or psychiatric conditions;
- environmental constraints;
- goals that genuinely conflict.

The correct engineering objective is robust improvement within a defined operating domain, with explicit failure detection and escalation when the system leaves that domain.

## 64. Self-mastery is not total suppression

The desired system is not one in which no urge appears. It is one in which an urge does not automatically determine the next action.

Let $U_t$ be urge intensity and $A_t$ the action selected. Self-mastery does not require:

$$
U_t=0
$$

It requires the capacity for:

$$
P(A_t=a_{\mathrm{goal}}\mid U_t>0)
$$

to remain meaningfully high when the goal action is appropriate and feasible.

This is a much more precise definition than "never feel distracted."

---

# PART XII — PERSONAL APPLICATION: STUDY, PHONE USE, SLEEP, AND SEXUAL URGES

## 65. Separate the behaviours before intervening

The original document mentioned several difficulties: inconsistent study, phone and television use, gaming, sleeping excessively, waking late, attraction, and masturbation.

These behaviours should not be collapsed into one diagnosis or one mechanism.

They may involve different triggers and reinforcers.

| Behaviour | Possible mechanism to investigate | Initial measurement |
|---|---|---|
| Phone checking | Cue accessibility, novelty, habit, avoidance | Checks per study hour |
| Gaming | Reward, progression, social reinforcement, escape | Planned vs unplanned play time |
| Television | Low-effort stimulation, routine, fatigue | Context and duration |
| Sleeping late | Circadian timing, schedule, sleep quality | Sleep/wake log |
| Excessive sleepiness | Sleep debt, medical or psychological factors | Duration, quality, daytime impairment |
| Sexual distraction | Normal desire, cue learning, compulsive pattern, avoidance | Trigger, frequency, functional impact |
| Study avoidance | Ambiguity, effort, fear of failure, low immediate reward | Initiation latency and task difficulty |

The table contains hypotheses, not diagnoses.

**Claim-linked evidence register records:** R27. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 66. Sexual attraction and masturbation

Sexual attraction and sexual urges are normal aspects of human biology. Masturbation is not inherently an addiction or evidence of weak intelligence.

The relevant questions are functional:

- Is the behaviour voluntary?
- Does it repeatedly displace important responsibilities?
- Have there been persistent unsuccessful attempts to control it?
- Does it continue despite significant adverse consequences?
- Is distress caused by actual impairment, or solely by moral disapproval?

Compulsive Sexual Behaviour Disorder is a clinical category involving persistent impaired control and significant functional consequences. A person should not self-diagnose from the mere presence of sexual thoughts, attraction, or masturbation.

The ROOT protocol can be used for ordinary unwanted patterns, but persistent, distressing, or impairing behaviour merits professional assessment. The goal is not to wage war against biology; it is to establish a workable relationship between impulses, values, and chosen action.

**Claim-linked evidence register records:** R45, R46, R53, R57. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 67. Sleep is a control-system context variable

Sleep is a relevant biological context for attention and task performance, but the evidence must be stated by exposure and cognitive domain. R43 is a meta-analysis of experimentally manipulated short-term sleep restriction (61 studies, 71 populations): it reports negative average effects on overall cognitive processing, executive function, sustained attention and long-term memory, while finding insufficient evidence for several broader domains. R44 is a separate one-night meta-analysis in healthy adults (44 studies, 1,087 participants; 2–6 h sleep opportunity): it reports increased subjective sleepiness and impaired sustained attention, but no significant pooled effects for choice reaction time, cognitive throughput, working memory or inhibitory control. R44 also reports heterogeneity and a publication-bias signal for sustained-attention reaction time. Neither review establishes the effects of every sleep-timing or sleep-quality pattern, nor explains an individual's performance.

A focus plan should not treat sleep as optional recovery after productivity. Sleep is part of the biological context in which learning and attention operate. The two-week log below is descriptive self-monitoring, not a diagnostic instrument or causal test.

A practical initial procedure:

1. Record sleep and wake times for two weeks.
2. Record daytime sleepiness and naps separately from sleep duration.
3. Observe whether the schedule varies substantially; do not infer a sleep disorder from variation alone.
4. Avoid interpreting persistent excessive sleepiness as laziness.
5. Seek medical evaluation if sleep problems are persistent, severe, or functionally impairing.

**Evidence boundary:** R43 concerns experimentally manipulated short-term restriction; R44 concerns one-night restriction under specified laboratory conditions. Their pooled effects do not provide a personal prediction or a known coefficient for the ROOT fatigue rating. Circadian timing and subjective sleep quality require separate evidence.

**Claim-linked evidence register records:** R25, R43, R44. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 68. Study initiation as a designed transition

A frequent failure point is not sustained concentration but task initiation.

A task such as "study thermodynamics" is underspecified. It creates uncertainty about the first action.

Replace it with a concrete transition:

- open the specified chapter;
- write the heading;
- solve the first example;
- list the known variables;
- work for a short, predetermined interval.

The objective is to reduce initiation cost $K(a)$ and uncertainty $D(a)$ in the action-selection model.

This is an engineering intervention: make the desired transition easier to execute.

**Claim-linked evidence register records:** R15, R24, R31, R32, R48, R65, R66, R68. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 69. A personal experimental protocol

### Phase 1 — Baseline (7 days)

Do not attempt to change every behaviour at once.

Record:

- planned study blocks;
- actual focused minutes;
- initiation latency;
- unplanned phone checks;
- return-to-task latency;
- sleep and wake times;
- principal trigger for each distraction.

### Phase 2 — High-leverage environmental change (7 days)

Choose the single most frequent or costly distraction.

Change its accessibility. For phone checking, this might mean keeping the phone outside the study area and disabling nonessential notifications.

Do not simultaneously redesign every aspect of life; otherwise it becomes difficult to identify what helped.

### Phase 3 — Alternative-response training (14 days)

Write one if–then plan for the main trigger.

Example:

> If I reach for my phone because a study problem feels difficult, I will write the exact point where I am stuck, attempt one smaller step, and only then decide whether a planned break is needed.

Practise the alternative response and record whether it was executed.

### Phase 4 — Review and adaptation (weekly)

Compare the intervention period with baseline.

Keep an intervention if it improves functional outcomes at an acceptable cost. Modify or discard it if it does not.

### Suggested dashboard

| Metric | Baseline | Current | Desired direction |
|---|---:|---:|---|
| Focused minutes/day | Record | Record | Increase |
| Unplanned phone checks | Record | Record | Decrease |
| Return-to-task latency | Record | Record | Decrease |
| Study initiation latency | Record | Record | Decrease |
| Completed planned blocks | Record | Record | Increase |
| Sleep/wake regularity | Record | Record | Improve |

The objective is measured progress, not perfect compliance.

---

**Claim-linked evidence register records:** R27, R31, R34, R38, R41, R42, R47, R48, R50, R65, R68. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.

# PART XIII — THE UNIFIED MASTER FRAMEWORK


## 70. Four proposed foundations and their candidate roles

The four named foundations are assigned distinct proposed roles in a candidate architecture; their interfaces and joint operation have not been validated.

| Foundation | Proposed role | Candidate representation |
|---|---|---|
| Space or Null Theory | Proposed context acquisition and constraints | $O_t, C_t, M_t$ |
| Out of Box Theory | Proposed inference/generation beyond explicit observations | $\mathcal{I}(A,M,K)$ |
| Recursive Intelligence | Proposed self-modeling and policy modification | Candidate update $\Theta_{t+1}=U(\Theta_t,\text{feedback})$ |
| ROOT Control Protocol | Proposed behavioural intervention protocol | Candidate closed-loop controller |

## 71. Schematic joint-state mapping (not an executable transition law)

The entire system can be represented as:

$$
\boxed{
\left(
\mathcal{S}_t,
O_t,
\mathcal{I}_t,
G_t,
R_t,
\mathcal{R}_t
\right)
\xrightarrow{\text{candidate update}}
\mathcal{S}_{t+1}
}
$$

where:

- $\mathcal{S}_t$: current system-level descriptor; not established as a minimal or Markov-sufficient state;
- $O_t$: external observation;
- $\mathcal{I}_t$: internal inference;
- $G_t$: goals and constraints;
- $R_t$: feedback or outcome;
- $\mathcal{R}_t$: available physical and computational resources.

The candidate update is intended to involve four operation families, but their interfaces and coupling rules are unspecified:

$$
\mathcal{O}=
\left\{
\mathcal{F}_{\mathrm{context}},
\mathcal{F}_{\mathrm{inference}},
\mathcal{F}_{\mathrm{control}},
\mathcal{F}_{\mathrm{learning}}
\right\}
$$

The set notation lists candidate operation families without asserting a serial order. The boxed state mapping is therefore a schematic placeholder, not an executable or validated transition law. No domains/codomains, update order, concurrency semantics, clocks, feedback interfaces, resource accounting or coupling rule are yet specified.

## 72. Proposed Context–Inference–Control Cycle (conceptual sequence)

1. **Context enters:** Space or Null Theory.
2. **Representations update:** the system changes its internal model.
3. **Consequences are generated:** Out of Box Theory.
4. **Actions are evaluated:** cost-sensitive control.
5. **A policy is selected:** goal-directed or habitual action.
6. **The world responds:** physical interaction and feedback.
7. **The system evaluates itself:** Recursive Intelligence.
8. **The policy is modified:** ROOT Control Protocol.
9. **The next cycle begins:** the updated system encounters new context.

This is an organizing diagram for the proposed architecture, not a validated necessary/sufficient sequence. The order, concurrency, stage interfaces, termination conditions and incremental contribution of each stage remain to be specified and tested.

## 73. Compatibility result — Contextual processing and internal inference

**Statement:** Space or Null Theory and Out of Box Theory are compatible if context is defined to include both external observations and internal structural information.

**Proof:**

1. Space or Null Theory states that meaningful processing depends on context and system structure.
2. Out of Box Theory states that a system can generate conclusions not explicitly supplied by its observations.
3. Let context include $C=(O,M,A,K)$, where $O$ is external observation, $M$ memory, $A$ architecture, and $K$ formal constraints.
4. A system can perform inference $Y=\mathcal{I}(M,A,K)$ even when new external observation $O=0$.
5. If $K\models p$ and the chosen proof calculus is complete for the specified semantics, the system can derive $p$ without directly observing the event described by $p$; non-vacuity requires that $K$ have at least one model.
6. The derivation depends on internal context, so it does not violate the contextual dependence described by Space or Null Theory.

Therefore, the two theories describe complementary operations: context acquisition and internal consequence generation.

**Claim-linked evidence register records:** R01, R02, R03, R05, R21, R22. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.

## 74. Conditional proposition — Feedback can alter goal-action selection under specified assumptions

**Statement:** In a specified finite-action model with fixed inverse-temperature $\beta>0$, increasing the goal action's score while holding competing scores and the feasible action set fixed increases its softmax selection probability. This is a conditional property of the selector, not proof that ROOT causes the score change.

**Derivation:**

1. Let $P_t(a_g\mid s)$ be the probability of the goal action in state $s$, and let the feasible action set be fixed for the comparison.
2. Let $Q_t(a)$ be the defined local score for each feasible action, with all terms on a commensurable scale.
3. Under softmax selection, $P_t(a_g\mid s)=\exp(\beta Q_t(a_g))/\sum_{a\in\mathcal{A}}\exp(\beta Q_t(a))$.
4. If $Q_t(a_g)$ increases while all competing scores, $\mathcal{A}$ and $\beta$ remain fixed, the goal action's probability increases. A greedy selector requires the goal action to become a maximizer over the full feasible set.
5. Whether a ROOT intervention actually changes the score in this direction is an empirical causal question. Repeated successful execution strengthens a policy only under a separately specified learning/update rule.

The result supports a conditional action-selection model. It does not establish a universal self-mastery law, a distinct Recursive Intelligence mechanism, or the efficacy of a particular intervention.

---

**Claim-linked evidence register records:** R24. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.

# PART XIV — EXPERIMENTAL PROGRAMME AND FALSIFIABILITY

## 75. Why experiments are necessary

A formal framework can be internally consistent and still fail to describe the world accurately.

The next step is to derive predictions that could be falsified.

The experiments below are intended to probe different components rather than merely demonstrate that a productivity routine can help someone. As currently specified, they are component-level tests; they do not yet discriminate the four-component integration from established alternatives.

## 76. Experiment A — Inference without new external observation

**Question:** Can a system derive a result not explicitly represented in its input while receiving no new external observation during inference?

**Design:**

1. Construct problems with a known formal rule system.
2. Provide the system with the rules and initial conditions.
3. Withhold the target conclusion.
4. Prevent access to external information during the inference period.
5. Measure whether the system derives the conclusion.
6. Test the derivation independently.

**Prediction:** Systems with adequate internal representations and inference capacity will derive some conclusions not explicitly supplied as output facts.

**Failure condition:** If a system consistently fails despite adequate representation and computational capacity, the particular inference model may be insufficient. This does not refute all forms of Out of Box Theory.

**Claim-linked evidence register records:** R27, R38, R41, R42, R47, R50. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 77. Experiment B — Structural prediction of unobserved outcomes

**Question:** Can a model predict a physical outcome before direct observation?

**Design:**

1. Define a mathematical model from previously available evidence.
2. Derive a specific, risky prediction.
3. Register the prediction before collecting the target data.
4. Conduct the measurement independently.
5. Compare the result with the prediction and competing models.

**Prediction:** Some model-derived predictions will be confirmed, demonstrating that direct observation of the target event is not necessary for prior derivation.

**Failure condition:** Repeated predictive failure under controlled conditions weakens the model's claimed correspondence with reality.

**Claim-linked evidence register records:** R27, R38, R41, R42, R47, R50. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 78. Experiment C — Energy, task difficulty, and action selection

**Question:** Do effort, fatigue, and task uncertainty change the probability of selecting a habitual distraction?

**Design:**

1. Measure task difficulty and uncertainty.
2. Measure fatigue and sleep state.
3. Record cue exposure and unplanned action selection.
4. Compare conditions while controlling for major confounds.
5. Estimate a model of action probability.

**Prediction:** The probability of selecting a familiar low-initiation-cost action may rise when task effort, fatigue, or uncertainty increases, subject to individual differences and task context.

**Important limitation:** This experiment does not directly prove that thermodynamic entropy causes distraction. It tests a resource-sensitive action-selection model.

**Claim-linked evidence register records:** R13, R14, R15, R24, R25, R27, R38, R41, R42, R43, R44, R47, R50, R62, R63. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 79. Experiment D — Environmental obstruction

**Question:** In a defined target loop, does a specific accessibility manipulation reduce the target action per eligible opportunity, without unacceptable substitution or burden, relative to a credible comparator?

**Evidence boundary:** R33 found that grayscale reduced objectively measured smartphone screen time by about 50 minutes/day relative to a self-monitoring control in a student sample, but found no immediate causal improvement in academic performance or subjective well-being. R34 found that objective use declined in intervention and control groups alike, while self-reported problematic use increased; heightened usage awareness was a possible explanation. These are local and mixed findings, not a universal obstruction law or evidence of sustained-attention improvement.

**Design:**

1. Define one target action, one cue/accessibility manipulation and an eligible opportunity for the target action. Do not use total screen time as a proxy for every form of distraction.
2. Record baseline opportunities, target actions, device-recorded use and return-to-task latency. Keep subjective reports separate from objective device measures.
3. Compare a specific barrier with a credible matched monitoring/sham or randomized/counterbalanced control. If the design is within-person, predefine phase order, carryover and reversal conditions.
4. Keep task, schedule and monitoring intensity as stable as practical. Record awareness/reactivity so that monitoring effects are not mistaken for barrier effects.
5. Measure target actions per eligible opportunity, total device time, substitutions across apps/devices, functional task output, return-to-task latency, adherence, burden and adverse effects.
6. Include a follow-up after barrier removal where maintenance is part of the claim.
7. Predefine the primary estimand, meaningful-effect threshold, missing-data handling and analysis. Preserve null and adverse findings.

**Prediction:** A barrier may reduce a particular access-dependent action in some contexts. It need not improve sustained attention or task performance, and apparent reduction may be offset by substitution, awareness effects or burden. A screen-time change alone is not a functional benefit.

**Claim-linked evidence register records:** R27, R33, R34, R38, R41, R42, R47, R50. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 80. Experiment E — Alternative-response training

**Question:** Does a trigger-specific if–then response improve behavioural recovery beyond a credible active planning comparator?

**Evidence boundary:** If–then implementation intentions are an established intervention family, not a ROOT invention. The meta-analytic evidence is positive but heterogeneous; R48 reports substantial publication bias and a small robust-Bayesian model-averaged estimate (d = .15). Effects are larger for contingent if–then plans, stronger goal motivation and at least one rehearsal. Recording the plan itself was associated with a smaller effect; this is distinct from recording outcome data in the ROOT tracker (R31–R32, R48).

**Design:**

1. Define one target loop, a specific cue, and an eligible opportunity for the cue to occur. Distinguish cue detection from execution of the alternative response.
2. Confirm that the target goal is active, personally endorsed and feasible in the relevant context. Record goal motivation rather than assuming it.
3. Form a genuinely contingent plan in the form “If [specified cue/opportunity] occurs, then I will [one observable, feasible alternative response].” A schedule that merely lists when and what to do is not equivalent to a cue-contingent if–then plan.
4. Rehearse the plan at least once. Record whether the plan itself is written or otherwise recorded, because plan recording may moderate the effect; do not confuse this with outcome logging.
5. Use a credible active comparator matched for attention, time and task exposure (for example, goal intention or schedule-format planning). Hold environmental obstruction constant or factorialize it so that the effect of planning can be distinguished from Experiment D.
6. Measure cue opportunities, cue detection, alternative-response execution per eligible opportunity, return-to-task latency, functional task output, adherence, substitution, intervention fidelity, burden and adverse effects.
7. Predefine the primary estimand, meaningful-effect threshold, missing-data rule and analysis. Preserve null and adverse findings.

**Prediction:** A contingent, rehearsed plan may improve alternative-response execution in some contexts, particularly when goal motivation is sufficient. The expected effect should not be assumed large or universal; the protocol tests a known component, not the ROOT package or a distinct Recursive Intelligence mechanism.

**Claim-linked evidence register records:** R27, R31, R32, R38, R41, R42, R47, R48, R50, R65. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 81. Experiment F — Recursive adaptation

**Question:** Does weekly model revision improve intervention selection compared with a fixed routine?

**Design:**

1. Group episodes by trigger and context.
2. Estimate which interventions worked in each context.
3. Update the personal policy weekly.
4. Compare adaptive and fixed-policy periods.
5. Measure functional outcomes and intervention burden.

**Prediction:** An adaptive controller should outperform a poorly matched fixed routine when triggers and physiological states vary meaningfully.

**Claim-linked evidence register records:** R27, R35, R37, R38, R41, R42, R47, R49, R50, R51, R54, R55. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 82. Measurement and statistical safeguards

All experiments should:

- predefine outcomes;
- distinguish primary from secondary measures;
- record missing data;
- avoid changing multiple variables without tracking them;
- use repeated measurements;
- report uncertainty;
- avoid interpreting correlation as causation;
- test alternative explanations;
- replicate where possible.

Personal experiments can be useful, but they are not equivalent to controlled clinical trials. They can identify practical patterns without establishing universal mechanisms.

---

**Claim-linked evidence register records:** R27, R38, R41, R42, R47, R50. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.

# PART XV — LIMITS, FAILURE MODES, AND SAFEGUARDS


## 83. The framework's limits

The unified framework does not prove:

- that all physical systems are intelligent;
- that consciousness is reducible to information processing;
- that the brain literally minimizes thermodynamic entropy;
- that every unobserved fact can be deduced;
- that every habit is an addiction;
- that willpower can override every biological constraint;
- that ROOT guarantees a permanent cure;
- that a mathematical action-selection model is a complete neuronal description.

These claims do not follow from the axioms.

## 84. Failure mode: Mistaking coherence for truth

A model can be internally consistent and false about the world.

**Safeguard:** derive predictions that could fail, and test them independently.

## 85. Failure mode: Mistaking novelty for discovery

A novel idea may be unsupported or contradicted by evidence.

**Safeguard:** label ideas by epistemic status: possibility, hypothesis, deduction, prediction, or corroborated result.

## 86. Failure mode: Mistaking energy cost for a complete explanation

Physical resource constraints are necessary background conditions, but they do not uniquely explain a particular behaviour.

**Safeguard:** include learning history, task structure, goals, physiological state, and environment.

## 87. Failure mode: Overengineering self-control

A rigid routine can become unsustainable or create unnecessary stress.

**Safeguard:** use the smallest intervention that produces measurable benefit, then adapt.

## 88. Failure mode: Treating a clinical problem as a discipline problem

Persistent sleepiness, attention impairment, compulsive behaviour, depression, anxiety, or other conditions may require professional assessment.

**Safeguard:** do not use ROOT as a substitute for appropriate medical or psychological care.

**Claim-linked evidence register records:** R45, R46, R53. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 89. Failure mode: Optimizing the wrong goal

A system can become highly efficient at pursuing an objective that is outdated, harmful, or externally imposed.

**Design requirement:** Any proposed recursive-control architecture should include periodic review of the goal hierarchy itself. This is a normative safeguard, not an implemented or validated capability of Recursive Intelligence.

---

# PART XVI — FORMAL LAW SET OF THE UNIFIED FRAMEWORK

The following are proposed laws or principles within this treatise. They are formal statements of the framework, not claims that new universal laws of physics have already been experimentally established.

## Law 1 — Contextual Dependence Law (Space or Null Theory)

The output of a meaningful information-processing system depends on its architecture, internal state, and the context available to it.

$$
Y=F(A,M,X,C)
$$

No new external input is required for every internal transformation.

## Law 2 — Internal Consequence Law (Out of Box Theory)

A system can derive a novel proposition from internal representations when that proposition is constrained by the system's premises and inference rules.

$$
K\models p
\Rightarrow
p\text{ is derivable without direct observation of its target event}
$$

## Law 3 — Epistemic Underdetermination Law

If multiple possible worlds satisfy all available information but disagree about a proposition, that proposition is not uniquely determined by that information.

$$
\exists w_1,w_2\models K:
p(w_1)\neq p(w_2)
\Rightarrow
K\not\models p,\ K\not\models\neg p
$$

## Law 4 — Physical Embodiment Law

Every physically realized computation is constrained by the energy, time, memory, noise, and causal properties of its substrate.

## Law 5 — Cost-Sensitive Selection Principle

When action selection accounts for reward and cost, a low-cost habitual action can be selected over a higher-value long-term action if its immediate and control-cost advantages dominate the current selection function.

## Law 6 — Cached-Policy Principle

Repeatedly useful actions can become cached policies that reduce deliberative cost. The same efficiency can preserve a response after the environment or objective changes.

## Law 7 — Recursive Modification Principle

A system capable of estimating aspects of its own operation can use feedback to modify its future policy, provided the relevant variables are observable or estimable and the intervention has causal leverage.

## Law 8 — Closed-Loop Self-Mastery Principle (ROOT)

Behavioural improvement is pursued by detecting triggers, changing access and action costs, executing alternative responses, practising them, measuring outcomes, optimizing biological and environmental conditions, and updating the policy.

## Law 9 — Conditional Stability Principle

A behavioural controller improves stability only within the domain where its state estimates, interventions, learning process, and available resources are adequate.

## Law 10 — Reality-Correction Principle

Generated hypotheses and predictions must remain revisable in response to evidence. Internal coherence is not a substitute for external validation.

---

# PART XVII — FINAL SYNTHESIS

## 90. Current status of Space or Null Theory

Space or Null Theory proposes that meaningful processing depends on context and system structure. Under the treatise's broad definition, context includes internal memory, architecture, goals and constraints as well as newly arriving external stimuli.

A system may therefore perform internal processing in the absence of fresh sensory input. This is a bounded conceptual/computational possibility, not processing from literal nothingness and not, by itself, evidence of semantic truth, external discovery or predictive accuracy. The theory's definitions and distinctive empirical contribution remain to be tested against established context, memory and computation frameworks.

## 91. Current status of Out of Box Theory

Out of Box Theory proposes that a system can derive conclusions that are not explicitly supplied as observations. Its defensible formal core is conditional: if $K\models p$ under specified semantics and a sound, complete proof calculus is available, then $K\vdash p$ (see the corrected Theorem 1). This is derivability from premises, not acquisition of arbitrary facts without information.

A model may in principle anticipate an unobserved consequence when the phenomenon is constrained by premises that adequately represent the target world. Actual-world truth requires that the actual world satisfy those premises; predictive performance requires prospective, calibrated evaluation against competitive baselines. No such predictive performance has yet been empirically validated for this treatise's framework.

## 92. Current status of the physical–cognitive bridge

A brain is a physical system, and its computation is constrained by energy, time, noise and finite resources. Human neural and physiological studies support task- and region-specific energetic responses, but regional, whole-brain, whole-body and subjective-effort measures are not interchangeable.

The proposed link from physical resource constraints to subjective effort, action-score weights, habitual selection and repeated behaviour remains a multilevel hypothesis. The treatise's score coefficients and causal chain have not been identified or validated. This offers a candidate explanation for some cases in which a person repeatedly performs a behaviour they reflectively reject; it is not an established personal explanation or universal law.

Thermodynamic entropy is not psychological distraction. Physical implementation constrains behavioural control, but intermediate mechanisms and task-specific evidence are required for any causal claim.

**Claim-linked evidence register records:** R11, R12, R13, R14, R24, R60, R61, R62, R63, R69. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 93. Current status of Recursive Intelligence

Recursive Intelligence is proposed as a functional construct in which a system uses representations of its own operation to modify future operation. This is a candidate synthesis of self-monitoring, metacognition, meta-control and adaptive policy update.

The treatise has not yet demonstrated a distinct mechanism, a validated measurement model, or incremental predictive advantage over those established constructs. The self-model and update equations remain schematic. The construct should not be presented as a newly established intelligence type until it has operational discriminators and comparative tests.

**Claim-linked evidence register records:** R35, R37, R51, R54, R55. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 94. Current status of ROOT Control Protocol

ROOT is the proposed operational intervention architecture:

- Recognise the trigger.
- Obstruct the automatic pathway.
- Override with a specific alternative.
- Train the replacement.
- Correct using outcome data.
- Optimise biological and environmental conditions.
- Learn and consolidate.

Its intended aim is not the elimination of all impulses, but to increase the probability that chosen objectives govern behaviour despite competing signals. Component-level evidence exists for selected planning and environmental-friction techniques. The integrated ROOT package, its seven-stage sequence, sustained-attention effect, long-term maintenance and controller guarantees have not been validated. The protocol remains a proposal, not an established intervention.

**Claim-linked evidence register records:** R31, R34, R41, R47, R48, R65, R68. Full bibliographic metadata, source-access status, claim-specific mappings and pinpoints are maintained in `CLAIM_EVIDENCE_REGISTER.md`.


## 95. Schematic architecture summary — not a unified state-transition law

The proposed components can be summarized as an architecture-level dependency map. No complete joint state-transition law has been derived:

$$
\boxed{
\left(
\mathcal{S}_t,
O_t,
\mathcal{I}_t,
G_t,
\Pi_t,
R_t,
\mathcal{R}_t
\right)
\xrightarrow{\text{candidate update}}
\mathcal{S}_{t+1}
}
$$

This tuple is a schematic dependency inventory, not a defined transition equation. Its separate $\Pi_t$ term is not yet reconciled with the input list in §71; no equivalence between the two schematics is asserted.

Space or Null Theory proposes how context and structure condition the system.

Out of Box Theory proposes how internal inference can derive consequences not explicitly observed, subject to the validity of its premises and proof system.

Physical constraints bound implementation, while Recursive Intelligence and ROOT remain proposed models for self-directed adaptation and behavioural intervention. None of these summaries implies that the integrated architecture has been empirically validated.

Behavioural learning may change which actions become readily available, but the treatise has not specified or validated a general update law for this process.

Recursive Intelligence is proposed to use feedback and self-representation to modify a system's future operation; the mechanism and its distinct contribution remain unspecified and unvalidated.

ROOT Control Protocol is proposed as an operational method for behavioural redesign. Its relationship to any distinct recursive-intelligence mechanism, and the efficacy of the integrated protocol, remain to be tested.

---

# CONCLUDING STATEMENT

The proposed unifying idea is that an intelligent system can be studied as a physically implemented process in which context, internal representation, inference, action selection and feedback interact. Where a system can modify its own policies or operating conditions, those changes may in turn alter how it responds to later contexts.

**This is the treatise's integrative hypothesis, not an established universal law:**

**An intelligent system is not merely a receiver of context. It is a physically embodied structure that can transform context into models, use models to generate predictions and actions, and—when suitable recursive control is available—use action consequences to modify future responses.**

This proposed synthesis connects questions about knowledge and discovery with physical implementation, behavioural persistence and self-directed adaptation. The links among these domains require further formal specification and empirical discrimination from established alternatives.

For behavioural self-management, one practical hypothesis is that an unwanted impulse need not disappear before a chosen action can occur. Changing cues, access conditions, alternative responses and feedback may alter what follows the impulse. Whether a particular intervention helps must be assessed in its context, with outcomes and adverse effects measured.

The intended objective is not a mind without competing signals, but improved alignment between considered objectives and actual behaviour. The extent to which the four named components provide a coherent and useful framework remains an open research question.

That is the proposed research purpose of **Space or Null Theory**, **Out of Box Theory**, **Recursive Intelligence**, and the **ROOT Control Protocol**.

---

# SELECTED REFERENCES AND SCIENTIFIC FOUNDATIONS

The following ten entries are selected foundational and contextual references, not the complete bibliography for every empirical claim. They are not a substitute for claim-level source mapping. Claim-linked evidence records R01–R70, including bibliographic metadata, source-access status, claim mappings and source pinpoints, are maintained in the companion `CLAIM_EVIDENCE_REGISTER.md`. The register is the controlling source-level audit; its access limitations and qualifications must be preserved. Where a selected entry is used to support a specific treatise claim, that use must be traceable to a stable register record; otherwise it should be treated as contextual reading rather than independent evidence for that claim. These references do not establish the named theories in this treatise as validated scientific laws.

1. Chattopadhyay, P., Misra, A., Pandit, T., & Paul, G. (2025). **Landauer principle and thermodynamics of computation.** *Reports on Progress in Physics, 88*(8), Article 086001. https://doi.org/10.1088/1361-6633/add6b3.  
   Peer-reviewed review of Landauer's principle, thermodynamic costs of computation, error correction and finite-time considerations.

2. Karbowski, J. (2024). **Information thermodynamics: From physics to neuroscience.** *Entropy, 26*(9), Article 779. https://doi.org/10.3390/e26090779.  
   Open-access perspective/review on applying information thermodynamics to neural inference, learning and information storage.

3. Street, S. (2016). **Neurobiology as information physics.** *Frontiers in Systems Neuroscience, 10*, Article 90. https://doi.org/10.3389/fnsys.2016.00090.  
   Review of relationships among information, thermodynamics and neural organization.

4. Kringelbach, M. L., Sanz Perl, Y., & Deco, G. (2024). **The thermodynamics of mind.** *Trends in Cognitive Sciences, 28*(6), 568–581. https://doi.org/10.1016/j.tics.2024.03.009.  
   Review proposing thermodynamic measures for studying brain hierarchy, information flow and brain-state organization.

5. Shenhav, A., Musslick, S., Lieder, F., Kool, W., Griffiths, T. L., Cohen, J. D., & Botvinick, M. M. (2017). **Toward a rational and mechanistic account of mental effort.** *Annual Review of Neuroscience, 40*, 99–124. https://doi.org/10.1146/annurev-neuro-072116-031526.  
   Review of computational and mechanistic accounts of cognitive-control costs and mental effort.

6. Malvaez, M. (2020). **Neural substrates of habit.** *Journal of Neuroscience Research, 98*(6), 986–997. https://doi.org/10.1002/jnr.24552. Published online 6 November 2019.  
   Review of neural substrates of goal-directed and habitual behavioural control. The final journal issue is 2020; 2019 is the online-first date.

7. Averbeck, B., & O'Doherty, J. P. (2022). **Reinforcement-learning in fronto-striatal circuits.** *Neuropsychopharmacology, 47*, 147–162. https://doi.org/10.1038/s41386-021-01108-0.  
   Review of reinforcement learning, state representations, action values and arbitration in fronto-striatal circuits. Published online 5 August 2021; issue date January 2022.

8. Schulkin, J., & Sterling, P. (2019). **Allostasis: A brain-centered, predictive mode of physiological regulation.** *Trends in Neurosciences, 42*(10), 740–752. https://doi.org/10.1016/j.tins.2019.07.010.  
   Review of predictive physiological regulation and the brain's allocation of energy and resources.

9. Stanford, K. (2023). **Underdetermination of scientific theory.** In E. N. Zalta & U. Nodelman (Eds.), *The Stanford Encyclopedia of Philosophy* (Summer 2023 Edition). Metaphysics Research Lab, Stanford University. https://plato.stanford.edu/archives/sum2023/entries/scientific-underdetermination/. First published 12 August 2009; substantive revision 4 April 2023.  
   Explains distinct forms of underdetermination and why available evidence may fail to determine a unique theory or proposition.

10. Maroney, O. (2009). **Information processing and thermodynamic entropy.** In E. N. Zalta (Ed.), *The Stanford Encyclopedia of Philosophy* (Fall 2009 Edition). Metaphysics Research Lab, Stanford University. https://plato.stanford.edu/archives/fall2009/entries/information-entropy/. First published 15 September 2009.  
    Discusses Maxwell's demon, Szilard's engine, Landauer's principle and the relationship between information processing and thermodynamics.

---

## STATUS OF THE FRAMEWORK

**Work products currently present in the draft (not equivalent to validation or completion):**

- Working definitions and conceptual distinctions for context, null conditions, intelligence, novelty, discovery, habit, distraction and self-mastery. Their operational adequacy and distinct contribution remain under review.
- Two bounded formal results: derivability from premises under specified soundness/completeness conditions, and model-theoretic underdetermination where admissible models disagree. Neither establishes arbitrary fact acquisition or predictive performance.
- Candidate action-selection, habit, behavioural-state, feedback and control models. Several remain under-specified; their parameters and causal relations have not been identified in human systems.
- A literature synthesis and source-to-claim register. Source access varies by record; review-level, abstract-only and primary full-text evidence are distinguished, and unresolved provenance gaps remain documented.
- A proposed integration of Space or Null Theory, Out of Box Theory, Recursive Intelligence and ROOT. The joint interfaces, typed state, update semantics and incremental explanatory value have not been established.
- A ROOT process description and operational tracker. These are planning and measurement artifacts, not a validated clinical or behavioural intervention.
- Protocol templates for experiments A–F, including design requirements and disconfirmation conditions. None is represented as executed, preregistered, approved or empirically completed.
- Internal adversarial review across the canonical claim inventory. This is not independent external review.

**Not established; further work remains necessary:**

- A unified, executable state-transition model or validated general law connecting all four components.
- A distinct empirical contribution or incremental predictive advantage over established theories of context processing, inference, metacognition, meta-control, adaptive control and behavioural intervention.
- A causal physical-to-cognitive bridge, individual action-score coefficients, or a validated human behavioural stability model.
- A validated intelligence composite, recursive-intelligence mechanism, or Lyapunov certificate for the human/ROOT system. The Schur-stability result applies only to its specified homogeneous linear time-invariant model.
- Efficacy, durability, generalizability or safety of the integrated ROOT package.
- Execution or empirical results for experiments A–F.
- Resolution of the E17/E18 source-provenance gaps and all remaining source-access limitations.
- Qualified independent review.

**Current editorial status:** this is a substantial conceptual research manuscript with conditional formal results, bounded evidence synthesis, candidate models and an experimental-design programme. It is not a complete or empirically validated unified theory, and it should not be described as review-ready until the governing plan's remaining acceptance and review gates are satisfied.