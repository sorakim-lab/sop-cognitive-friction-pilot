# SOP Cognitive Friction Pilot

This repository presents a lightweight, rule-based pilot implementation
exploring sentence-level cognitive friction in SOPs.

## What is an SOP?
In regulatory laboratory environments in the biopharmaceutical field, Standard Operating Procedures (SOPs) define approved workflows, testing steps, and documentation requirements intended to ensure consistency and regulatory compliance.
In practice, however, SOPs often specify what must be done without fully resolving how ambiguous or exceptional situations should be judged. As a result, analysts are frequently required to interpret procedures arbitrarily and make judgment calls that are not explicitly addressed in the written guidance.

## What is cognitive friction?
Cognitive friction refers to the additional mental effort imposed on individuals
when procedural instructions require interpretation, judgment, or reconciliation
across fragmented or ambiguous guidance.
In the context of SOPs, cognitive friction arises not from document length alone,
but from structural features that embed decision-making demands into routine tasks.

## What this pilot does
This pilot performs a sentence-level annotation of representative SOP statements
to examine whether predefined structural features associated with cognitive friction
can be consistently identified using simple, rule-based criteria.

Specifically, each sentence is assessed for the presence or absence of five
theory-driven categories: cross-references to external documents,
conditional branching, exception handling, obligation cues,
and sentence length exceeding a predefined threshold.

The goal of this pilot is not to quantify cognitive load or predict error outcomes,
but to demonstrate the feasibility and interpretability of a structured approach
to making judgment demands embedded in procedural text visible and comparable.

## What this repository includes
- A Jupyter notebook (`sop_cognitive_friction_pilot.ipynb`) demonstrating
  rule-based detection of structural features associated with cognitive friction
  (e.g., conditional branching, exception handling, obligation cues).
- A small set of synthetic SOP sentences used for illustrative analysis.

## Scope and limitations
This repository is intended as an exploratory pilot.
The analysis relies on synthetic examples and lightweight heuristics
to demonstrate feasibility rather than to provide empirical validation.

## Status
# SOP Cognitive Friction Pilot

This repository presents a lightweight, rule-based pilot implementation
exploring sentence-level cognitive friction in SOPs.

## What is an SOP?
In regulatory laboratory environments in the biopharmaceutical field, Standard Operating Procedures (SOPs) define approved workflows, testing steps, and documentation requirements intended to ensure consistency and regulatory compliance.
In practice, however, SOPs often specify what must be done without fully resolving how ambiguous or exceptional situations should be judged. As a result, analysts are frequently required to interpret procedures arbitrarily and make judgment calls that are not explicitly addressed in the written guidance.

## What is cognitive friction?
Cognitive friction refers to the additional mental effort imposed on individuals
when procedural instructions require interpretation, judgment, or reconciliation
across fragmented or ambiguous guidance.
In the context of SOPs, cognitive friction arises not from document length alone,
but from structural features that embed decision-making demands into routine tasks.

## What this pilot does
This pilot performs a sentence-level annotation of representative SOP statements
to examine whether predefined structural features associated with cognitive friction
can be consistently identified using simple, rule-based criteria.

Specifically, each sentence is assessed for the presence or absence of five
theory-driven categories: cross-references to external documents,
conditional branching, exception handling, obligation cues,
and sentence length exceeding a predefined threshold.

The goal of this pilot is not to quantify cognitive load or predict error outcomes,
but to demonstrate the feasibility and interpretability of a structured approach
to making judgment demands embedded in procedural text visible and comparable.

## What this repository includes
- A Jupyter notebook (`sop_cognitive_friction_pilot.ipynb`) demonstrating
  rule-based detection of structural features associated with cognitive friction
  (e.g., conditional branching, exception handling, obligation cues).
- A small set of synthetic SOP sentences used for illustrative analysis.

## Scope and limitations
This repository is intended as an exploratory pilot.
The analysis relies on synthetic examples and lightweight heuristics
to demonstrate feasibility rather than to provide empirical validation.

## Status
This project is part of an ongoing line of inquiry into judgment and cognitive load
in regulated work systems.
