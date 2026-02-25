# SOP Cognitive Friction — Rule-Based Annotation Prototype

This repository provides a lightweight, rule-based implementation of the
sentence-level cognitive friction annotation framework described in:

**Kim, S. (2026). _Structuring Judgment, Stabilizing Responsibility:
Cognitive Friction in Procedural Texts._**

The code demonstrates how structurally embedded judgment demands in procedural
language can be operationalized and annotated computationally at the sentence level.

---

## What is an SOP?

In regulated laboratory and biopharmaceutical environments, Standard Operating
Procedures (SOPs) define approved workflows, testing steps, and documentation
requirements intended to ensure consistency and regulatory compliance.

In practice, SOPs often specify what must be done without fully resolving how
ambiguous or exceptional situations should be judged. As a result, practitioners
frequently interpret procedures locally during execution, introducing judgment
calls that are not explicitly resolved within the written instruction.

---

## What is cognitive friction?

Cognitive friction refers to structurally embedded judgment demands in
procedural language that require actors to interpret, reconcile, or condition
instructions during execution.

In SOP-like texts, cognitive friction arises not from document length alone but
from specific structural features that embed contingent pathways, deferred
criteria, or discretionary qualifiers within procedural sentences.

---

## What this prototype does

This prototype performs sentence-level annotation of procedural sentences to
demonstrate that predefined structural features associated with cognitive
friction can be made observable and consistently identified using transparent,
rule-based criteria.

Each sentence is evaluated for the presence of four cognitive friction features:

- conditional branching  
- cross-references  
- exception structures  
- discretionary qualifiers  

A composite cognitive friction score is computed as the co-occurrence count of
these features within each sentence.

The goal is not to predict cognitive load or performance outcomes, but to
demonstrate the feasibility and interpretability of a structured approach for
rendering judgment demands embedded in procedural text analytically visible.

---

## Repository contents

- **CF_corpus500_annotation.ipynb**  
  Python notebook implementing the rule-based annotation procedure for
  sentence-level cognitive friction features across the 500-sentence corpus.

- **public_procedural_corpus_500_mixed.xlsx**  
  Mixed procedural corpus (N = 500) combining publicly derived and
  synthetic SOP-like sentences used in the exploratory analysis.
  
---

## Annotation logic

Each sentence is evaluated using deterministic lexical–syntactic patterns.

Example cues:

- Conditional: `if`, `when`, `unless`, `where applicable`  
- Cross-reference: `section`, `annex`, `per SOP`, `in accordance with`  
- Exception: `except`, `otherwise`, `unless otherwise specified`  
- Discretion: `as appropriate`, `as deemed necessary`, `if needed`  

Composite score:
friction_score = conditional + cross_reference + exception + discretion

---

## Scope and limitations

This implementation reflects the conceptual operationalization presented in the
paper and is intentionally simplified.

- Rule-based patterns approximate structural cues rather than full parsing  
- Annotation targets sentence-level procedural units only  
- Synthetic examples are used for illustration  
- No attempt is made to model actor cognition or decision processes  

The prototype is intended for methodological transparency and conceptual
demonstration rather than predictive or production use.

---

## Relation to the paper

This repository accompanies the cognitive friction framework introduced in:

**Kim, S. (2026). _Structuring Judgment, Stabilizing Responsibility:
Cognitive Friction in Procedural Texts._**

The implementation demonstrates that structurally embedded judgment demands in
procedural documentation can be rendered computationally observable using
transparent rule-based annotation at the sentence level.

It supports the paper’s methodological claim that responsibility-bearing
interpretive demands encoded in procedural language can be systematically
identified without reliance on complex NLP models or large-scale corpora.

---

## Status

This repository is part of an ongoing research program on responsibility,
judgment, and documentation in regulated sociotechnical systems.

---

## Source Materials

Procedural sentences in this repository were extracted or adapted from
publicly available regulatory and safety documentation, including
laboratory and biosafety guidance published by international and
academic institutions such as WHO, MIT, and Yale EHS.

All source documents are publicly accessible PDFs. Sentences were
parsed and selected solely for non-commercial research and illustrative
purposes. Some examples are lightly adapted for clarity, and additional
sentences are fully synthetic constructions designed to approximate
SOP-like procedural structure.

This repository does not redistribute full original documents and
contains no proprietary or confidential SOP content.

## License

MIT License
