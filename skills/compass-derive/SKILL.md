---
name: compass-derive
description: Invoke Compass derivation pipelines with LLM curation where required — compile a project README from its template, produce a static-site build, or draft a Diátaxis-shaped end-user doc set from typed project docs. Use to generate derived artifacts from an Compass corpus.
---

# compass-derive

Stub. Derivation-driver skill for the Compass documentation standard (the S9
authoring-assistance layer; see `Compass.md` §22 and §23 S9, tracked as
`COMPASS-DRAFT-authoring-assistance`).

## Intended behavior (to be built)

- Run the README/fixture compiler with transclusion resolution (§10, S7).
- Drive a federated static-site build (§16 Astro target, S8).
- Seed an end-user doc set via audience projection, then assist curation
  (§21, S5) — derivation seeds, a writer finishes.
- Wrap the deterministic derivation tooling (§16 pipeline, §22 toolchain)
  behind a conversational interface, adding LLM curation only where the
  pipeline requires human/assistant judgment.

## Dependencies

- Depends on S1/S2 (toolchain + Markdown→Lexis importer), S5 (audience
  projection), S7 (fixture compilation), and S8 (site build). It is the
  last skill to complete, as its dependencies land in the other Plans first.

## Invariants

- This skill **proposes** derived drafts; authoritative source remains the
  project docs, and derived artifacts are never edited in place (§16).
