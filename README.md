# SOP Cognitive Friction Pilot

This repository presents a lightweight, rule-based pilot implementation
exploring sentence-level cognitive friction in SOPs.

## What is an SOP?
In regulatory laboratory environments in the biopharmaceutical field,
Standard Operating Procedures (SOPs) define approved workflows, testing steps,
and documentation requirements intended to ensure consistency and regulatory compliance.
In practice, however, SOPs often specify what must be done without fully resolving
how ambiguous or exceptional situations should be judged.
As a result, analysts are frequently required to interpret procedures independently
, introducing judgment calls that are not explicitly addressed in the written guidance.

## What is cognitive friction?
Cognitive friction refers to the additional mental effort imposed on individuals
when procedural instructions require interpretation, judgment, or reconciliation
across fragmented or ambiguous guidance.
In the context of SOPs, cognitive friction arises not from document length alone,
but from structural features that embed judgment demands within routine tasks.

## What this pilot does
This pilot performs a sentence-level annotation of representative SOP sentences
to examine whether predefined structural features associated with cognitive friction
can be made observable and consistently identified using simple, rule-based criteria.

Specifically, each sentence is assessed for the presence or absence of five
theory-driven categories:
- cross-references to external documents  
- conditional branching  
- exception handling  
- obligation cues  
- sentence length exceeding a predefined threshold  

The goal of this pilot is not to quantify cognitive load or predict error outcomes,
but to demonstrate the feasibility and interpretability of a structured approach
for making judgment demands embedded in procedural text visible and comparable.

## What this repository includes
- A Jupyter notebook (`sop_cognitive_friction_pilot.ipynb`) demonstrating
  rule-based detection of sentence-level structural features associated with cognitive friction
  (e.g., conditional branching, exception handling, obligation cues).
- A small set of synthetic SOP sentences used for illustrative analysis.

## Scope and limitations
This repository is intended as an exploratory pilot
and relies on synthetic examples and lightweight heuristics
to demonstrate feasibility rather than to provide empirical validation.

## Status
This project is part of an ongoing line of inquiry into judgment and cognitive load
in regulated work systems.

## How this connect to the paper
This repository accompanies the exploratory pilot study
**“Sentence-Level Cognitive Friction in SOPs: An Exploratory Pilot.”**

The code implements a lightweight, rule-based version of the sentence-level
annotation framework described in the paper. Its purpose is not to automate
judgment or to evaluate model performance, but to demonstrate that the proposed
concept of cognitive friction can be rendered observable and computationally
expressible at the sentence level.

Specifically, the repository:
- mirrors the five structural features introduced in the paper,
- applies them to synthetic SOP sentences for illustrative analysis, and
- supports the paper’s methodological claim that judgment demands embedded in
procedural language can be systematically identified without reliance on
complex models or large datasets.

The implementation is intended for transparency and conceptual demonstration
rather than for production use or empirical deployment.
