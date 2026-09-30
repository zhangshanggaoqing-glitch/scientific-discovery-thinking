# Evaluation Rubric

Use this rubric to evaluate whether an AI response actually demonstrates scientific-discovery reasoning.

Score each category 0–2.

## 1. Observation / interpretation separation

- **0**: mixes measured facts and mechanistic claims.
- **1**: partially separates them.
- **2**: clearly distinguishes observation, inference, and hypothesis.

## 2. Competing hypotheses

- **0**: provides one preferred explanation only.
- **1**: lists alternatives without meaningful differences.
- **2**: provides mechanistically distinct alternatives that explain the same observations.

## 3. Discriminating predictions

- **0**: no explicit predictions.
- **1**: predictions are vague or shared by all hypotheses.
- **2**: hypotheses predict meaningfully different outcomes.

## 4. Experiment quality

- **0**: lists assays or markers.
- **1**: proposes an intervention but interpretation remains ambiguous.
- **2**: proposes a high-information experiment with clear causal and discriminating logic.

## 5. Unexpected-result handling

- **0**: dismisses surprises as noise or repeats.
- **1**: acknowledges surprise but does not update the model.
- **2**: treats a validated surprise as evidence about a hidden assumption or missing variable.

## 6. Causal discipline

- **0**: treats association as mechanism.
- **1**: mentions causality but does not operationalize it.
- **2**: uses perturbation, rescue, timing, necessity/sufficiency, or alternative-explanation logic appropriately.

## 7. System-boundary reasoning

- **0**: assumes the chosen biological scale is sufficient.
- **1**: lists environment/immune/context generically.
- **2**: expands the system boundary only when a specific anomaly requires it.

## 8. Model update

- **0**: conclusions do not change after evidence.
- **1**: updates are qualitative but vague.
- **2**: explicitly states what gained/lost support and what remains unresolved.

## 9. Falsifiability

- **0**: the preferred model can explain every result.
- **1**: some potential falsification is mentioned.
- **2**: clearly states observations that would weaken or contradict each leading hypothesis.

## 10. Information efficiency

- **0**: more assays = better.
- **1**: some prioritization.
- **2**: explicitly prefers decisive, interpretable experiments over unnecessary complexity.

## Interpretation

- **17–20**: strong discovery-oriented scientific reasoning.
- **13–16**: useful but still partly confirmation-oriented.
- **8–12**: descriptive research assistance rather than discovery reasoning.
- **0–7**: mechanistic storytelling with weak epistemic control.

The numeric score is a training/evaluation aid, not a substitute for expert judgment.
