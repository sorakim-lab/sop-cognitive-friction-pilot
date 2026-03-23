# SOP Cognitive Friction — Rule-Based Annotation Prototype

This repository provides a lightweight, rule-based implementation of the sentence-level cognitive friction annotation framework described in:

**Kim, S. (2026). _Structuring Judgment, Stabilizing Responsibility: Cognitive Friction in Procedural Texts._ SSRN Preprint.**

The code demonstrates how structurally embedded judgment demands in procedural language can be operationalized and annotated computationally at the sentence level.

---

## What is an SOP?

In regulated laboratory and biopharmaceutical environments, Standard Operating Procedures (SOPs) define approved workflows, testing steps, and documentation requirements intended to ensure consistency and regulatory compliance.

In practice, SOPs often specify what must be done without fully resolving how ambiguous or exceptional situations should be judged. As a result, practitioners frequently interpret procedures locally during execution, introducing judgment calls that are not explicitly resolved within the written instruction.

---

## What is cognitive friction?

Cognitive friction refers to structurally embedded judgment demands in procedural language that require actors to interpret, reconcile, or condition instructions during execution.

In SOP-like texts, cognitive friction arises not from document length alone but from specific structural features that embed contingent pathways, deferred criteria, or discretionary qualifiers within procedural sentences.

---

## What this prototype does

This prototype performs sentence-level annotation of procedural sentences to demonstrate that predefined structural features associated with cognitive friction can be made observable and consistently identified using transparent, rule-based criteria.

Each sentence is evaluated for the presence of four cognitive friction features:

- conditional branching
- cross-references
- exception structures
- discretionary qualifiers

A composite cognitive friction score is computed as the co-occurrence count of these features within each sentence.

The goal is not to predict cognitive load or performance outcomes, but to demonstrate the feasibility and interpretability of a structured approach for rendering judgment demands embedded in procedural text analytically visible.

---

## Repository Contents

| File | Description |
|------|-------------|
| `CF_corpus500_annotation.ipynb` | Rule-based annotation procedure for sentence-level cognitive friction features across the 500-sentence corpus |
| `CF_corpus500_robustness_check.ipynb` | Robustness analysis replicating core findings on the 400 naturally occurring sentences (excluding synthetic subset) |
| `public_procedural_corpus_500_mixed.xlsx` | Mixed procedural corpus (N=500) combining publicly derived and synthetic SOP-like sentences |

---

## Annotation Logic

Each sentence is evaluated using deterministic lexical–syntactic patterns.

Example cues:

- **Conditional:** `if`, `when`, `unless`, `where applicable`
- **Cross-reference:** `section`, `annex`, `per SOP`, `in accordance with`
- **Exception:** `except`, `otherwise`, `unless otherwise specified`
- **Discretion:** `as appropriate`, `as deemed necessary`, `if needed`

Composite score:
```
friction_score = conditional + cross_reference + exception + discretion
```

---

## Key Findings

- Conditional branching is the most prevalent friction feature (33.8% of sentences)
- Structurally compounded judgment demands concentrate in a smaller subset of sentences (10.6% with friction score ≥ 2)
- Non-zero friction appears consistently across all source categories — including naturally occurring procedural documentation
- Robustness analysis on 400 naturally occurring sentences confirms that core distributional patterns hold independently of the synthetic subset

---

## Scope and Limitations

This implementation reflects the conceptual operationalization presented in the paper and is intentionally simplified.

- Rule-based patterns approximate structural cues rather than full parsing
- Annotation targets sentence-level procedural units only
- Synthetic examples are used for illustration
- No attempt is made to model actor cognition or decision processes

The prototype is intended for methodological transparency and conceptual demonstration rather than predictive or production use.

---

## Related Work

This repository is part of a broader research program on responsibility structuring in regulated sociotechnical systems:

- [Anticipated Accountability Convergence (AAC)](https://ssrn.com) — SSRN Preprint
- [Responsibility Convergence in Organizational Investigations (RC)](https://ssrn.com) — SSRN Preprint
- [Premature Accountability Convergence (PAC)](https://ssrn.com) — SSRN Preprint
- [FDA Warning Letters — PAC Analysis](https://github.com/sorakim-lab/fda-warning-letters-pac-analysis) — GitHub

---

## Source Materials

Procedural sentences in this repository were extracted or adapted from publicly available regulatory and safety documentation, including laboratory and biosafety guidance published by international and academic institutions such as WHO, MIT, and Yale EHS.

All source documents are publicly accessible PDFs. Sentences were parsed and selected solely for non-commercial research and illustrative purposes. Some examples are lightly adapted for clarity, and additional sentences are fully synthetic constructions designed to approximate SOP-like procedural structure.

This repository does not redistribute full original documents and contains no proprietary or confidential SOP content.

---

## Citation

```
Kim, S. (2026). Structuring Judgment, Stabilizing Responsibility:
Cognitive Friction in Procedural Texts. SSRN Preprint.
```

---

## License

MIT License
