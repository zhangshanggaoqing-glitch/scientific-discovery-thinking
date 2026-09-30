---
name: scientific-discovery-thinking
description: A rigorous scientific reasoning skill for turning observations, anomalies, failed expectations, and conflicting evidence into competing hypotheses and high-information discriminating experiments. Designed for research planning, paper reading, experimental interpretation, mechanism discovery, and AI-assisted science.
version: 0.1.0
license: MIT
maintainer: Stone
---

# Scientific Discovery Thinking

## Purpose

This skill is not a literature-summary template and not a generic "design an experiment" prompt.

Its job is to help a researcher reason like a discovery scientist:

> Observation → anomaly → competing explanations → discriminating prediction → decisive experiment → model update → new concept.

The central principle is:

> Do not ask only whether a hypothesis can explain the data. Ask what other hypotheses can also explain the data, and what observation would force those explanations apart.

Use this skill when:

- interpreting unexpected experimental results;
- deciding what experiment should come next;
- evaluating whether a mechanism is actually supported;
- reading a paper for scientific logic rather than for facts;
- identifying contradictions across datasets or papers;
- turning a negative result into a more informative question;
- searching for hidden feedback, context dependence, or missing system variables;
- designing experiments that maximize information gain rather than assay count.

Do **not** use this skill to fabricate mechanistic stories from weak data. It must preserve uncertainty and explicitly separate observation from interpretation.

---

## Non-negotiable epistemic rules

### 1. Separate observation from interpretation

Always write these separately.

**Observation**: what was directly measured or seen.

**Interpretation**: what the observation may mean.

**Hypothesis**: a model that generates testable predictions.

Never rewrite an interpretation as if it were a measured fact.

### 2. An anomaly is information, not an inconvenience

When data contradict expectation, do not automatically label the result as noise, technical failure, or "needs repetition".

First ask:

- If the result is real, what assumption is wrong?
- What hidden variable could make both the old model and the new result coherent?
- Does the anomaly reveal a missing feedback loop, state, compartment, timescale, environmental dependency, or alternative function?

Technical failure remains possible, but it is one hypothesis among others.

### 3. Never evaluate only one hypothesis

For every important claim, construct at least two plausible competing explanations whenever the evidence permits.

Avoid:

> H1 is plausible, therefore H1 is true.

Prefer:

> H1, H2, and H3 all explain the current observations. Which future observation would differ among them?

### 4. Prefer discriminating experiments over confirmatory accumulation

A strong experiment is one whose possible outcomes would produce different updates for competing hypotheses.

A weak experiment often produces the same conclusion regardless of outcome, or merely adds another correlated marker.

Ask:

> What is the smallest experiment that would make nature choose between the leading explanations?

### 5. A negative result can falsify the framing, not merely the assay

When an expected phenotype is absent, consider:

- the proposed mechanism is wrong;
- the mechanism is context-dependent;
- the readout is downstream but non-essential;
- compensation or feedback restores the phenotype;
- the perturbation changes survival rather than proliferation, state rather than abundance, timing rather than endpoint, or one compartment rather than another;
- the system boundary is too narrow.

### 6. Causality requires intervention logic

Correlation is not mechanism.

Prefer evidence structures such as:

- perturbation → predicted change;
- rescue → reversal of phenotype;
- dose/time ordering compatible with causality;
- orthogonal perturbations converging on the same mechanism;
- necessity and sufficiency tested separately when meaningful;
- alternative explanations explicitly weakened.

### 7. Mechanisms are models, not diagrams

A pathway cartoon is not a mechanism unless it generates risky predictions.

A useful mechanism should specify:

- entities;
- direction of influence;
- context;
- timing;
- expected intervention response;
- conditions under which the mechanism should fail.

### 8. Expand the system boundary when local explanations fail

If a cell-intrinsic model fails, consider:

- microenvironment;
- immune system;
- stromal cells;
- microbiota;
- nutrients and oxygen;
- drug pressure;
- tissue architecture;
- organismal physiology;
- evolutionary adaptation;
- temporal dynamics.

Do not expand the boundary arbitrarily; expand it because a narrower model cannot explain the evidence.

### 9. Search for conceptual inversion

Ask whether the accepted function suggests an opposite intervention.

Examples of inversion patterns:

- activate → inhibit;
- inhibit → release inhibition;
- driver → vulnerability;
- resistance → hidden dependency;
- proliferation → survival;
- cell intrinsic → environmental;
- harmful process → therapeutic leverage.

Conceptual inversion is not wordplay. It must produce a testable consequence.

### 10. Update models explicitly

After each major result, state:

- what was learned;
- which hypothesis gained support;
- which hypothesis lost support;
- what remains unresolved;
- what experiment now has the highest information value.

Do not let the narrative remain unchanged after contradictory data.

---

# Core workflow: DISCOVERY LOOP

## Step 1 — Define the phenomenon

Write the phenomenon in one sentence without mechanism language.

Bad:

> STK39 promotes colorectal cancer by activating pathway X.

Better:

> Under condition C, perturbing STK39 changes phenotype P by magnitude M relative to control.

If the phenomenon itself is not robust, stop and resolve measurement quality first.

## Step 2 — Build the observation ledger

Create a table:

| Evidence | Direct observation | Context | Reliability | What it does NOT prove |
|---|---|---|---|---|

Include discordant evidence rather than averaging it away.

## Step 3 — Identify the broken expectation

Complete:

> If the current model were sufficient, we would expect ______. Instead, we observe ______.

If no expectation is being violated, there may be useful science, but there is not yet a clear anomaly-driven discovery problem.

## Step 4 — Expose hidden assumptions

List assumptions required by the current interpretation.

Typical hidden assumptions:

- expression implies function;
- target engagement implies pathway dependence;
- a phenotype in one cell line generalizes to another;
- endpoint measurements reflect the causal event;
- a single pathway dominates;
- cells are in a stable state;
- treatment does not induce feedback;
- tumor cells can be studied independently of their environment.

## Step 5 — Construct competing hypotheses

Create 2–5 hypotheses that explain the same observations.

For each hypothesis provide:

- mechanism;
- unique prediction;
- expected observation if false;
- key confounder.

Do not make hypotheses trivially different descriptions of the same mechanism.

## Step 6 — Build a prediction matrix

| Experiment/Observation | H1 predicts | H2 predicts | H3 predicts |
|---|---|---|---|

Search for rows where predictions diverge strongly.

Those rows contain candidate discriminating experiments.

## Step 7 — Choose the highest-information experiment

Score candidate experiments qualitatively on:

- **Discrimination** — do leading hypotheses predict different outcomes?
- **Causal leverage** — is there an intervention rather than mere association?
- **Interpretability** — will each possible result have a clear meaning?
- **Robustness** — can the result survive technical artifacts?
- **Cost/time** — is there a simpler experiment with similar information value?
- **Boundary value** — could the experiment reveal that the current system model is incomplete?

Prefer the experiment with the best information-to-cost ratio, not the experiment with the most assays.

## Step 8 — Pre-register interpretation

Before seeing the result, write:

- If result A → update H1/H2 how?
- If result B → update H1/H2 how?
- If result C → what new hypothesis becomes necessary?

This reduces post-hoc storytelling.

## Step 9 — Treat surprises as first-class outputs

If the result is unexpected:

1. audit technical validity;
2. do not discard it merely because it violates expectation;
3. identify which assumption failed;
4. generate a new hypothesis set;
5. repeat the prediction matrix.

## Step 10 — Convert result into a model update

Output:

- **What changed in our understanding?**
- **What explanation is now less plausible?**
- **What new variable or relationship entered the model?**
- **What is the next decisive experiment?**

---

# Discovery heuristics

## A. Arrival vs growth

When an outcome is enriched in one location, do not assume preferential arrival.

Separate:

1. exposure/arrival;
2. retention;
3. survival;
4. proliferation;
5. niche compatibility.

Design experiments that hold arrival constant while varying environment, or measure arrival independently from later growth.

## B. Contact vs diffusible signal

When two compartments interact, distinguish:

- direct contact;
- short-range signaling;
- diffusible factors;
- systemic effects.

Physical separation or conditioned-medium logic can be more informative than measuring dozens of downstream markers.

## C. Proliferation vs survival

If a perturbation changes cell number, separate:

- proliferation rate;
- death rate;
- quiescence;
- senescence;
- differentiation/state transition;
- adhesion/detachment artifacts.

A failure to proliferate is not equivalent to cell death.

## D. Driver vs feedback

When targeted inhibition fails despite target dependence, ask:

- Is the target incompletely inhibited?
- Is the pathway reactivated by feedback?
- Is a parallel pathway recruited?
- Has the cell entered a target-independent state?

Drug failure can function as a perturbation that exposes hidden network structure.

## E. Gain-of-function vs loss-of-suppression

A malignant phenotype can arise because something is activated or because a suppressive function is lost.

Do not search only for "accelerators"; search for missing brakes.

## F. Cell intrinsic vs ecological

When otherwise similar cells behave differently across tissues or treatment contexts, investigate environmental selection and interaction effects.

The relevant unit of explanation may be the cell, niche, tissue, host, or ecosystem.

## G. Static pathway vs adaptive system

Biological systems respond to perturbation.

Always consider:

- feedback;
- compensation;
- redundancy;
- selection;
- state transition;
- adaptation over time.

A mechanism measured before treatment may not describe the post-treatment system.

---

# Anti-patterns

Flag these explicitly when detected.

### Marker accumulation

"Gene X changes marker A, B, C, D" is not automatically a mechanism.

### Tool-first science

Do not choose single-cell, spatial omics, AI, CRISPR, or proteomics merely because the technology is impressive.

Start with the scientific uncertainty and ask which measurement resolves it.

### One-story bias

Do not write a polished pathway story before competing hypotheses have been tested.

### Negative-result dismissal

"No effect" may reveal incorrect assumptions, context dependence, or an alternative biological role.

### Rescue theater

A rescue experiment is only informative if the rescue variable is mechanistically specific enough to discriminate alternatives.

### Correlation laundering

Multiple correlated datasets do not become causal evidence merely by being numerous.

### Endpoint blindness

The same endpoint can arise from different trajectories. Consider time-resolved measurements when dynamics matter.

### Complexity worship

A complicated experiment is not necessarily a strong experiment.

Prefer a simple decisive perturbation over an elaborate descriptive dataset when possible.

---

# Required response format

When this skill is invoked, respond using the following structure unless the user requests otherwise.

## 1. Phenomenon

One-sentence description of what is directly observed.

## 2. What is actually known

Separate direct evidence from interpretation.

## 3. Broken expectation / anomaly

State the key mismatch between prediction and observation.

## 4. Competing hypotheses

Provide 2–5 plausible explanations.

## 5. Prediction matrix

Show what each hypothesis predicts under the most informative candidate tests.

## 6. Highest-information next experiment

Explain why this experiment discriminates hypotheses.

Do not merely list assays.

## 7. Alternative outcomes

Explain what each major result would mean **before** the experiment is performed.

## 8. Hidden assumptions and confounders

List the assumptions most likely to invalidate interpretation.

## 9. Model update

If results already exist, state what changed in the causal model.

## 10. Discovery opportunity

Ask whether the result suggests:

- a new biological state;
- feedback mechanism;
- context dependence;
- missing suppressor;
- environmental interaction;
- conceptual inversion;
- broader system boundary.

---

# Confidence language

Use calibrated terms:

- **Observed** — directly supported by the stated measurement.
- **Supported** — evidence is consistent with the hypothesis and alternatives have been partly weakened.
- **Plausible** — compatible with evidence but not discriminated from alternatives.
- **Speculative** — proposed mechanism lacks direct evidence.
- **Contradicted** — current evidence conflicts with a prediction of the hypothesis.
- **Unknown** — available information cannot distinguish explanations.

Avoid "proves" unless the logical and experimental standard truly warrants it.

---

# Final principle

The goal of scientific reasoning is not to produce the most coherent story from existing data.

The goal is to design observations that make incorrect stories increasingly difficult to maintain.
