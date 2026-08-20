---
name: eidos-review
description: Review an Eidos document or pull request for judgment-level conformance the deterministic toolchain cannot check — genre fit, section-shape adherence, decision-record quality, prior-art coverage, cross-reference plausibility, and README-transclusion drift. Use before accepting or merging an Eidos document.
---

# eidos-review

Stub. Judgment-level review skill for the Eidos documentation standard
(the S9 authoring-assistance layer; see `Eidos.md` §22 and §23 S9, tracked
as `EIDOS-DRAFT-authoring-assistance`).

## Intended behavior (to be built)

- Assess **genre fit**: does the document match its declared genre (§4), or
  does its content suggest another (e.g. a Plan with no roadmap)?
- Check **section-shape adherence** against the §14 templates — sections
  present, correctly ordered, and carrying the right content.
- Evaluate **decision-record quality** (§8): real context, seriously
  considered alternatives, a decision that follows.
- Flag **cross-reference plausibility**: does a cited `id`/`D`/`O` actually
  concern what the citing text claims?
- Check **prior-art coverage** for `Survey`/`Eval`; **README-transclusion
  drift** for compiled fixtures (§10, S7).
- Produce a review report for a human editor (§6).

## Invariants

- This skill **proposes**; it is never the approval authority. Human
  editorial review (§6) sets `approved-by`; the §22 toolchain sets
  conformance.
