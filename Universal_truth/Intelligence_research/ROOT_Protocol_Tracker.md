# ROOT PROTOCOL TRACKER
## Unified Baseline, High-Leverage Obstruction, Override, and Control-Engineering Diagnostic System

**Version:** 1.0  
**Purpose:** Operational tracking artifact derived from *The Unified Theory of Context, Discovery, and Self-Mastery*, particularly Parts VIII–XII.  
**Design principle:** Estimate the state, identify the transition that produces unwanted action, change the highest-leverage condition, measure the response, and update the controller from evidence.

---

# 1. Operating model

This tracker combines baseline diagnosis and the first obstruction/override experiment in one continuous workflow. The same logs and metrics are used in both periods so that the comparison is interpretable.

```text
PLAN BLOCK
   |
ESTIMATE STATE ---- IDENTIFY TRIGGER / RISK
   |                         |
PREPARE TASK <-------- SELECT ONE OBSTRUCTION
   |
START TASK
   |
CUE OR URGE?
   | yes
RECOGNISE -> OBSTRUCT -> OVERRIDE -> RETURN TO TASK
   |                                      |
   +--------------- LOG -----------------+
                       |
                 DAILY REVIEW
                       |
                WEEKLY MODEL UPDATE
```

## Operating rules

1. Track one principal target loop at a time.
2. Separate observations from explanations. “Opened an app at 10:42” is an observation; “I was avoiding failure” is a hypothesis.
3. Record urge intensity separately from action. An urge can be strong while the response remains effective.
4. Record planned focus and actual focused work separately.
5. Measure return-to-task latency from noticing the diversion to resuming the intended task.
6. Change one principal environmental variable at a time during the first test.
7. Keep raw measures visible; do not let a composite score hide a worsening component.
8. Do not respond to missed targets with punishment, sleep restriction, or extreme compensatory schedules.
9. This is a self-management experiment, not a clinical diagnostic instrument. Persistent impairment, severe distress, or excessive sleepiness may warrant professional assessment.

---

# 2. State estimation and variable dictionary

The ROOT state vector from the treatise is:

$$
s_t=(c_t,u_t,f_t,d_t,g_t,h_t,e_t)
$$

| Variable | Meaning | Consistent 0–5 rating |
|---|---|---|
| $c_t$ | Cue intensity / salience | 0 absent; 5 extremely salient |
| $u_t$ | Urge / motivational activation | 0 none; 5 very strong |
| $f_t$ | Perceived fatigue (ordinal self-rating; not objective physiology) | 0 fresh; 5 severely depleted |
| $d_t$ | Task difficulty, ambiguity, uncertainty | 0 clear/easy; 5 highly difficult/unclear |
| $g_t$ | Goal activation / readiness | 0 inactive; 5 clear and active |
| $h_t$ | Competing habit strength in this context | 0 negligible; 5 strongly established |
| $e_t$ | Accessibility of competing action | 0 effectively inaccessible; 5 immediate access |

These are ordinal self-ratings, not laboratory measurements. Keep their meaning stable across the experiment. In particular, $f_t$ is perceived fatigue; it does not measure neural metabolism or objective physiological load. In the treatise's reduced six-variable model, $z_t$ denotes task demand and corresponds only approximately to this tracker's $d_t$. The seven ratings are not assumed equally spaced or directly additive.

## 2.1 Episode representation

The source treatise defines:

$$
\mathcal{E}_t=(\text{cueID}_t,s_t,a_t,r_t,\tau_t,\mathrm{RTL}_t,\iota_t)
$$

Operationally, $\text{cueID}_t$ identifies the trigger/context, while $c_t$ inside $s_t$ is its cue-intensity rating. Each episode records the trigger identifier, state, action, immediate consequence, duration, return-to-task latency, and intervention used.

## 2.2 Action-cost arbitration

The source action score is:

$$
Q(a)=R(a)+L(a)-\rho E(a)-\gamma C_{\mathrm{ctrl}}(a)
-\delta D(a)-\kappa K(a)
$$

| Term | Practical diagnostic question |
|---|---|
| $R(a)$ | What immediate reward or relief did the competing action provide? |
| $L(a)$ | What delayed value or consequence mattered? |
| $E(a)$ | Was the intended action physically demanding? |
| $C_{\mathrm{ctrl}}(a)$ | Did it require sustained deliberation or inhibition? |
| $D(a)$ | Was the next step uncertain or the reward delayed? |
| $K(a)$ | How much setup, initiation, or switching was required? |

Track the relative score conceptually:

$$
\Delta Q_t=Q(a_{\mathrm{goal}})-Q(a_{\mathrm{habit}})
$$

The intervention seeks to move the relevant situation toward:

$$
\Delta Q_t>0
$$

Do not invent precise coefficient estimates. Record the dominant advantage that appears to have decided the episode.

## 2.3 Return latency and stability model

$$
RTL=t_{\mathrm{resume}}-t_{\mathrm{notice}}
$$

The source's feedback model is:

$$
x_{t+1}=(A_{\mathrm{plant}}-B_{\mathrm{plant}}K_{\mathrm{fb}})x_t+w_t
$$

with a Lyapunov-style target:

$$
V(x_{t+1})-V(x_t)<0
$$

For personal tracking, use the proxy in Section 9. It is a measurement convention, not a validated Lyapunov function.

---

# 3. Unified baseline + intervention experiment

## 3.1 Recommended first 14-day cycle

| Days | Mode | Required activity |
|---|---|---|
| 1–7 | Baseline and diagnosis | Record normal blocks, state, triggers, distraction episodes, output, and RTL. Do not deliberately redesign multiple habits. |
| 8–14 | One obstruction + one override | Keep the same measures. Introduce one principal environmental obstruction and one trigger-specific alternative response. |

Mark every record `BASELINE` or `INTERVENTION`. Keep task type, measurement definitions, and major schedule conditions as stable as practical. If a seven-day baseline already exists, document its source and quality before shortening this phase.

## 3.2 Select one target loop

**Target loop:** ______________________________________________

**Intended goal behaviour:** ___________________________________

**Competing behaviour:** ______________________________________

**Typical context / time / location:** ___________________________

**Why this loop is the priority:** _______________________________

Prioritize a loop that is frequent, time-consuming, blocks initiation, or has high downstream cost. Do not target every behaviour at once.

## 3.3 Pre-register the causal hypothesis

> When **[observable cue/task condition]** occurs in **[context]**, and my state is approximately **[state variables]**, I tend to **[competing action]** because it provides **[immediate reward/relief]** and has lower **[initiation/control/delay cost]** than **[goal action]**.

**Hypothesis:**  
________________________________________________________________  
________________________________________________________________

**Evidence already observed:** __________________________________

**Alternative explanation to test:** _____________________________

A hypothesis is not a fact. The intervention period tests whether changing the proposed cause changes the outcome.

---

# 4. Daily setup and pre-block state sheet

Complete the setup once daily and the state estimate before each focus block, or whenever the state materially changes.

## 4.1 Daily control settings

| Field | Entry |
|---|---|
| Date | |
| Phase | BASELINE / INTERVENTION |
| Main task / subject | |
| Planned work window | |
| Planned focus blocks | |
| Planned focused minutes | |
| First physical task action | |
| Sleep duration / quality | |
| Daytime fatigue (0–5) | |
| Main environmental risk | |
| Primary obstruction (intervention phase) | |
| If–then override | |
| Planned breaks / recovery | |

## 4.2 Pre-block state estimate

| Variable | Rating 0–5 | Evidence / note |
|---|---:|---|
| Cue intensity $c$ | | |
| Urge activation $u$ | | |
| Fatigue $f$ | | |
| Task difficulty / ambiguity $d$ | | |
| Goal activation $g$ | | |
| Habit strength $h$ | | |
| Competing-action accessibility $e$ | | |

**Dominant destabilizing variable:** _____________________________

**Control response selected:** __________________________________

---

# 5. Focus-block log

Use one row per planned block.

| Date | Phase | Block ID | Task / next physical action | Planned min | Focused min | Start latency min | Unplanned shifts | Distraction min | RTL total min | Observable output | Result |
|---|---|---|---|---:|---:|---:|---:|---:|---:|---|---|
| | | | | | | | | | | | |
| | | | | | | | | | | | |
| | | | | | | | | | | | |
| | | | | | | | | | | | |
| | | | | | | | | | | | |

**Definitions**

- Focused minutes: genuinely engaged in the intended task, not merely seated with materials open.
- Start latency: actual start time minus planned start time.
- Unplanned shifts: switches away from the intended task not included in the plan.
- Distraction minutes: total time spent in the competing activity.
- RTL total: sum of return-to-task latencies in the block.
- Observable output: problems solved, calculations completed, notes produced, design work completed, etc.
- Result: COMPLETE / PARTIAL / INTERRUPTED / NOT STARTED.

---

# 6. Trigger and episode log

Create one entry for each meaningful episode. If episodes are extremely frequent, count them per block and describe representative episodes in detail.

| Date/time | Block ID | Phase | Trigger / antecedent | Task state | $c$ | $u$ | $f$ | $d$ | $g$ | $h$ | $e$ | Competing action | Immediate reward / relief | Duration min | RTL min | Response used | Outcome |
|---|---|---|---|---|---:|---:|---:|---:|---:|---:|---:|---|---|---:|---:|---|---|
| | | | | | | | | | | | | | | | | | |
| | | | | | | | | | | | | | | | | | |
| | | | | | | | | | | | | | | | | | |

## 6.1 Trigger classification

- [ ] External cue: notification, visible device, person, sound, open tab.
- [ ] Task ambiguity: unclear next step, missing information, task too large.
- [ ] Task difficulty: repeated error, problem-solving friction, overload.
- [ ] Emotional state: frustration, anxiety, boredom, discouragement.
- [ ] Physiological state: fatigue, hunger, discomfort, restlessness.
- [ ] Reward anticipation: novelty, entertainment, social feedback, game progression.
- [ ] Relief / avoidance: postpones effort or reduces discomfort.
- [ ] Context transition: break ended, location changed, device picked up.
- [ ] Other: __________________________

## 6.2 Immediate consequence

- [ ] Pleasure / stimulation
- [ ] Novelty / curiosity
- [ ] Social feedback
- [ ] Relief from effort or uncertainty
- [ ] Relief from uncomfortable emotion
- [ ] Physical comfort
- [ ] Habitual response; no clear reward identified
- [ ] Other: __________________________

**Diagnostic note:** If the behaviour is reinforced mainly by relief from task discomfort, blocking entertainment alone may not solve the loop. The override must also make task re-entry smaller, clearer, or more manageable.

---

# 7. Obstruction and override register

Use one register per intervention. Select the least burdensome barrier likely to change the cue-to-action transition.

## 7.1 Intervention specification

| Field | Entry |
|---|---|
| Intervention ID | |
| Target cue / trigger | |
| Target competing action | |
| Suspected mechanism | |
| Environmental variable changed | |
| Obstruction installed | |
| Intended accessibility change $e$ | |
| Alternative response | |
| Exact if–then instruction | |
| Installation date/time | |
| Expected benefit | |
| Implementation burden | |
| Possible side effects | |
| Primary success metric | |
| Review date | |

## 7.2 Candidate environmental levers

| Lever | Example | Main variable affected |
|---|---|---|
| Remove cue | Phone outside study area | Cue salience $c$ |
| Increase friction | Log out, remove shortcut, blocker | Accessibility $e$, competing-action initiation cost |
| Separate contexts | Designated study location | Cue-context association |
| Pre-stage task | Open book, calculator, notebook, exact problem | Goal-action initiation cost $K(a_g)$ |
| Reduce ambiguity | Write the next physical action | Task uncertainty $d$, delay cost $D(a_g)$ |
| Add response delay | Pause, stand, read if–then plan | Automatic response opportunity |
| Protect recovery | Stable sleep window and planned breaks | Fatigue $f$, control demand |

Change one principal lever at a time. Record what was actually installed, not merely what was intended.

## 7.3 Override specification

Weak: “I will focus” or “I will be disciplined.”

Operational:

> If **[specific cue]** occurs, I will **[observable alternative action]** for **[small defined interval or unit]**, then reassess.

**My override:**  
________________________________________________________________

**First physical action:** _______________________________________

**Minimum viable response when fatigued:**  
________________________________________________________________

**What counts as successful execution?**  
________________________________________________________________

---

# 8. Daily control dashboard

Complete at the end of each day. Use the same definitions during baseline and intervention.

| Metric | Calculation / definition | Value |
|---|---|---:|
| Planned focus blocks | Count planned | |
| Completed blocks | Count completed | |
| Block completion rate | Completed / planned × 100% | |
| Planned focused minutes | Sum planned | |
| Actual focused minutes | Sum focused | |
| Focus-time attainment | Actual / planned × 100% | |
| Unplanned shifts | Total count | |
| Distraction duration | Total minutes | |
| Mean RTL | Total RTL / episodes with RTL | |
| Median RTL | Median of episode RTL values | |
| Successful overrides | Alternative responses executed | |
| Override opportunities | Episodes where plan could be used | |
| Override success rate | Successful / opportunities × 100% | |
| Initiation latency | Mean or median start latency | |
| Observable output | Work product completed | |
| Sleep duration | Estimated hours | |
| Daytime fatigue | 0–5 | |

If a denominator is zero, record `N/A`, not 0%.

## 8.1 Daily diagnostic review

1. Dominant destabilizing variable: ______________________________
2. Most frequent trigger: _______________________________________
3. Immediate reward or relief: __________________________________
4. Dominant action-cost advantage:
   - [ ] Initiation / switching cost
   - [ ] Task ambiguity / uncertainty
   - [ ] Control / inhibition demand
   - [ ] Fatigue / physiological load
   - [ ] Competing cue accessibility
   - [ ] Delayed reward
   - [ ] Other: ______________________
5. Did obstruction actually change access or cue exposure? ________
6. Was the override executed? If not, what blocked it? ____________
7. Smallest evidence-based adjustment for tomorrow: ______________

---

# 9. Weekly engineering review

Review every seven days. Do not change the system based on one unusually good or bad day.

## 9.1 Baseline-to-intervention comparison

| Measure | Baseline week | Intervention week | Difference | Desired direction |
|---|---:|---:|---:|---|
| Completed blocks / day | | | | Increase |
| Block completion rate | | | | Increase |
| Focused minutes / day | | | | Increase |
| Unplanned shifts / day | | | | Decrease |
| Distraction minutes / day | | | | Decrease |
| Mean RTL | | | | Decrease |
| Median RTL | | | | Decrease |
| Override success rate | | | | Increase |
| Initiation latency | | | | Decrease |
| Observable output / day | | | | Increase |
| Mean fatigue (0–5) | | | | Interpret with context |
| Sleep regularity | | | | Improve |

Use averages for daily totals where appropriate. For skewed duration/latency, report median as well as mean. Preserve raw values.

## 9.2 Environmental leverage

The treatise's leverage concept is:

$$
\Lambda=
\frac{\text{reduction in unwanted-action probability}}
{\text{implementation cost}}
$$

For a personal estimate, choose one stable unwanted-action rate, such as checks per focus hour:

$$
\widehat{\Lambda}=
\frac{r_{\mathrm{before}}-r_{\mathrm{after}}}
{\text{intervention burden}}
$$

Rate burden 1–5 (1 negligible; 5 high ongoing inconvenience). This is a rough within-person comparison index, not a standardized effect size. Do not compare across different outcome units without normalization.

Before rate: ______  After rate: ______  Burden: ______  
Estimated leverage: ______  Interpretation: ____________________

## 9.3 Lyapunov-style deviation proxy

Normalize each component to 0–1 using fixed definitions across weeks:

- $G^{\mathrm{dev}}$: proportion of planned work not completed.
- $H^{\mathrm{activation}}$: competing-action activation rate per planned focus opportunity, normalized to a fixed reference.
- $RTL^{\mathrm{norm}}$: median RTL divided by a fixed reference latency, capped at 1.

Then track:

$$
V_t=w_1G_t^{\mathrm{dev}}+
w_2H_t^{\mathrm{activation}}+
w_3RTL_t^{\mathrm{norm}}
$$

A simple equal-weight starting proxy is:

$$
V_t=\frac{G_t^{\mathrm{dev}}+
H_t^{\mathrm{activation}}+
RTL_t^{\mathrm{norm}}}{3}
$$

| Week | Goal deviation | Habit activation | Normalized RTL | $V_t$ | Change vs prior |
|---|---:|---:|---:|---:|---:|
| Baseline | | | | | |
| Intervention 1 | | | | | |
| Intervention 2 | | | | | |
| Intervention 3 | | | | | |

Interpretation:
- A declining $V_t$ across repeated weeks is consistent with improvement on the selected dimensions.
- A rising $V_t$ signals that the current configuration is not improving those dimensions.
- Inspect all components; a lower composite with one sharply worsening component is not automatically success.
- This proxy is not a validated Lyapunov function and does not prove mathematical stability.

## 9.4 Weekly causal review

**What changed?** ______________________________________________

**Which outcome moved as predicted?** ___________________________

**Which outcome failed to move or worsened?** ____________________

**Mechanism supported?** SUPPORTED / PARTLY / NOT SUPPORTED / INCONCLUSIVE

**Evidence:** ___________________________________________________

**Alternative explanation:** ____________________________________

**Decision:** KEEP / MODIFY / REMOVE / REASSESS

**Reason:** ____________________________________________________

---

# 10. Diagnostic decision table

| Observed failure | Mechanism to test | Engineering response |
|---|---|---|
| Task never starts | High initiation cost; unclear first action | Pre-stage materials; define one physical next step; reduce block size |
| Repeated reach for phone | Cue-response chain starts before appraisal | Remove phone from reach; add physical separation; use visible if–then cue |
| Phone is inaccessible but attention drifts | Internal cue, ambiguity, fatigue, worry | Write exact point of difficulty; define one smaller problem-solving action; check state |
| Blocker is bypassed | Barrier too weak or avoidance reward too strong | Increase friction modestly; identify bypass reward; redesign task re-entry |
| Urge strong, no competing action | Override is working despite urge | Retain intervention; do not escalate unnecessarily |
| Distraction occurs but RTL falls | Recovery process improving | Retain response; continue measuring frequency and duration |
| Frequency falls but duration rises | Fewer but longer episodes | Inspect context; define stop/return action; track total lost time |
| Override not executed | Alternative vague, costly, or unavailable | Reduce to smaller physical action; rehearse outside trigger context |
| Fatigue predicts failures | Physiological load dominates | Adjust workload/recovery; assess persistent sleep problems appropriately |
| Task difficulty predicts failures | Uncertainty / control cost dominates | Break task into steps; use worked examples; define help-seeking rule |
| No measure improves | Wrong hypothesis, weak intervention, inconsistent use, confound | Reassess trigger model; change one variable; seek support if impairment persists |

Do not respond to persistent impairment by indefinitely increasing restrictions. Consider whether sleep, attention, mood, anxiety, compulsivity, health, or external demands require professional assessment or another form of support.

---

# 11. ROOT execution checklist

## R — Recognise
- [ ] Noticed the earliest cue, not only the completed distraction.
- [ ] Identified the task state / internal condition preceding it.
- [ ] Separated urge from action.

## O — Obstruct
- [ ] Competing action is less accessible.
- [ ] Intended task is physically ready to start.
- [ ] Obstruction is proportionate and sustainable.

## O — Override
- [ ] Used the specified if–then response.
- [ ] Alternative was observable and small enough to execute.
- [ ] If not used, recorded why.

## T — Train
- [ ] Rehearsed the alternative in the relevant context.
- [ ] Counted successful substitutions, not only failures.
- [ ] Treated episodes as learning data.

## C — Correct
- [ ] Compared outcome with intended result.
- [ ] Changed the suspected cause, not just the symptom.
- [ ] Avoided uncontrolled multi-variable changes.

## O — Optimise
- [ ] Considered sleep, fatigue, workload, and recovery.
- [ ] Reduced task ambiguity and initiation friction.
- [ ] Kept the plan sustainable.

## L — Learn
- [ ] Updated trigger hypothesis from evidence.
- [ ] Retained interventions with useful benefit.
- [ ] Revised or removed ineffective interventions.

---

# 12. Reusable daily record

## Daily record — Date: __________

**Phase:** BASELINE / INTERVENTION  
**Target loop:** _______________________________________________

### Setup
- Main task:
- Planned work window:
- Planned blocks / focused minutes:
- First physical task action:
- Sleep duration / quality:
- Fatigue (0–5):
- Obstruction active:
- If–then override:

### Pre-block state

| $c$ | $u$ | $f$ | $d$ | $g$ | $h$ | $e$ |
|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | |

### Block outcomes

| Block | Planned min | Focused min | Start latency | Shifts | Distraction min | RTL | Output |
|---|---:|---:|---:|---:|---:|---:|---|
| 1 | | | | | | | |
| 2 | | | | | | | |
| 3 | | | | | | | |
| 4 | | | | | | | |

### Episode notes

| Time | Trigger | State / urge | Competing action | Reward / relief | Duration | RTL | Override? | Result |
|---|---|---|---|---|---:|---:|---|---|
| | | | | | | | | |
| | | | | | | | | |

### End-of-day metrics
- Completed blocks:
- Actual focused minutes:
- Unplanned shifts:
- Total distraction minutes:
- Mean / median RTL:
- Successful overrides / opportunities:
- Observable output:
- Dominant trigger:
- Dominant action cost:
- One evidence-based adjustment:

**One-sentence learning:**  
> The strongest predictor of my focus failure/success today was __________________, as shown by ________________________________.

---

# 13. Reusable weekly review

## Weekly review — Week of: __________

**Phase / intervention ID:** ___________________________________

| Measure | This week | Previous week | Direction |
|---|---:|---:|---|
| Focused minutes / day | | | |
| Completed blocks / day | | | |
| Unplanned shifts / day | | | |
| Distraction minutes / day | | | |
| Median RTL | | | |
| Override success rate | | | |
| Initiation latency | | | |
| Observable output | | | |
| Mean fatigue | | | |

**Most common trigger:** ________________________________________

**Highest-risk state combination:** _____________________________

**Most influential action cost:** _______________________________

**Strongest immediate reward / relief:** _________________________

**Most useful obstruction:** ____________________________________

**Most useful override:** _______________________________________

**Main failure mode:** _________________________________________

**Stability proxy $V_t$:** ______  **Change:** ______

Decision:
- [ ] Retain unchanged
- [ ] Retain but simplify
- [ ] Strengthen obstruction
- [ ] Redesign override
- [ ] Reduce task ambiguity / initiation cost
- [ ] Address fatigue / recovery
- [ ] Abandon intervention
- [ ] Reassess hypothesis
- [ ] Seek additional support

**Evidence and rationale:**  
________________________________________________________________

**One principal change for next week:**  
________________________________________________________________

**Prediction:** If this change addresses the actual mechanism, I expect __________________ to change from ______ to ______ over __________________.

---

# 14. Success criteria and interpretation

The tracker is useful if it increasingly answers:

1. Which cues and contexts precede unwanted action?
2. Which state variables make the system vulnerable?
3. What immediate reward or relief reinforces the competing action?
4. Which action cost makes the intended task lose?
5. Which environmental change has the greatest practical leverage?
6. Does the override increase successful alternative responses?
7. Is return-to-task latency decreasing?
8. Is actual task output improving?
9. Is the improvement sustainable at acceptable burden?
10. Does the updated model better predict when the next failure is likely?

Do not define success as zero urges, zero mistakes, or uninterrupted concentration. Prefer a combined pattern of increased intended-task execution, reduced costly distraction, shorter RTL, higher override success, improved output, and sustainable recovery.

A single metric must not dominate. Lower phone-check frequency accompanied by worse sleep and lower task output is not a successful system-level result.

---

# 15. Engineering summary

The tracker implements the recursive control cycle:

$$
\text{Observe}\rightarrow\text{Estimate}\rightarrow\text{Intervene}
\rightarrow\text{Measure}\rightarrow\text{Update}
$$

The operating strategy is:

1. Estimate the state.
2. Identify the earliest reliable trigger.
3. Diagnose the local reward and action-cost advantage.
4. Reduce access to the competing action.
5. Lower initiation cost and ambiguity for the goal action.
6. Execute a specific alternative response.
7. Measure focused work, distraction duration, and return latency.
8. Review evidence weekly.
9. Keep only interventions that improve functional outcomes at acceptable cost.
10. Update the model when evidence contradicts the original explanation.

**Final operating principle:** Do not ask only, “How can I force myself to resist?” Ask, “What state transition is producing this behaviour, what variable has the greatest leverage, and what measurable evidence would show that changing it worked?”

---

*This tracker is an operational research and self-management aid derived from the treatise. Its rating scales, composite scores, and proxy stability measure are proposed personal measurement conventions, not validated clinical instruments or experimentally established laws.*
