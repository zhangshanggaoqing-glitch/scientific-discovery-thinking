# Scientific Discovery Thinking Skill

A reusable scientific reasoning skill for AI assistants, research agents, and human researchers.

It is designed around a simple question:

> **What observation would force competing explanations apart?**

Most research assistants are optimized for retrieval, summarization, writing, and workflow automation. This skill instead focuses on the reasoning patterns behind scientific discovery: anomalies, competing hypotheses, discriminating experiments, causal intervention, failed expectations, feedback, context dependence, and conceptual reframing.

## Why this exists

The initial framework was distilled from a 2025 lecture deck by Prof. Yongli Yu, Department of Immunology, School of Basic Medical Sciences, Jilin University, titled *Observation/experiment that led to milestone discovery in cancer research*.

The lecture teaches cancer biology through the **observations and experiments that changed scientific models**, rather than by listing established concepts. No slide images or copyrighted slide material are redistributed in this repository.

The reasoning framework is generalized beyond cancer biology and can be used in molecular biology, immunology, pharmacology, bioinformatics, systems biology, and other experimental sciences.

## Core idea

```text
Observation
    ↓
Broken expectation
    ↓
Competing hypotheses
    ↓
Divergent predictions
    ↓
Discriminating experiment
    ↓
Unexpected result?
    ├── no  → strengthen/weaken models
    └── yes → expose hidden assumption
                 ↓
             new model
```

The skill deliberately resists a common failure mode of AI-assisted science:

> turning every dataset into a plausible mechanistic story.

Instead, it asks what evidence would make the story **wrong**.

## Repository structure

```text
scientific-discovery-thinking-skill/
├── SKILL.md
├── README.md
├── LICENSE
├── prompts/
│   └── system_prompt.md
├── frameworks/
│   ├── discovery_loop.md
│   └── discriminating_experiment.md
├── examples/
│   └── cancer_milestones.md
└── evals/
    └── rubric.md
```

## Quick use

Give an AI assistant the content of `SKILL.md`, then provide a research problem such as:

> STK39 knockdown reduces drug resistance in one colorectal cancer cell line but not another. Analyze this using Scientific Discovery Thinking. Do not give me a pathway story first. Build competing explanations and identify the highest-information experiment.

A good response should **not** start with a long list of pathways. It should first identify the observation, the violated expectation, and alternative explanations.

## What this skill is good at

- interpreting unexpected results;
- designing the next experiment;
- evaluating mechanism claims;
- detecting hidden assumptions;
- analyzing contradictory papers;
- converting negative results into new hypotheses;
- distinguishing descriptive from causal evidence;
- exposing feedback and adaptive responses;
- broadening system boundaries only when required;
- generating high-information experiments.

## What it is not

It is not:

- a replacement for domain expertise;
- a statistics package;
- a protocol generator;
- a literature database;
- a guarantee of novelty;
- an excuse to over-interpret weak data.

## Design philosophy

### 1. Science is model competition

A mechanism should compete against alternatives, not against a null narrative only.

### 2. Experiments are information-producing interventions

The best experiment is often not the largest experiment. It is the one where plausible models predict different outcomes.

### 3. Surprises deserve analysis

A result that violates expectation may be the most valuable result in the project.

### 4. Failure can reveal architecture

Drug resistance, missing phenotypes, or context-specific effects can expose feedback, redundancy, hidden states, or environmental dependencies.

### 5. Concepts matter

Some important discoveries do not merely identify a new molecule. They change what kind of explanation scientists consider possible.

## Attribution and intellectual lineage

The cancer examples in `examples/cancer_milestones.md` are derived from classic studies cited in the teaching material, including work associated with Paget, Hart & Fidler, Rous, Ide/Algire/Greenblatt & Shubik, Harris, Vaux/Cory/Adams, Varmus & Bishop, Gorre et al., Prahallad et al., Sakaguchi et al., and Allison and colleagues.

This repository extracts **reasoning patterns**, not slide content.

## License

MIT. See `LICENSE`.
