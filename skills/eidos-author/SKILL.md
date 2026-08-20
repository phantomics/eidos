---
name: eidos-author
description: Scaffold and draft Eidos documents. Use when creating a new Survey, Eval, Plan, Log, Ref, Guide, Spec, Arch, or Glossary document in an Eidos corpus — prompts for genre, scope, and namespace, generates the front-matter block and per-genre section skeleton, and assigns a provisional DRAFT identifier.
---

# eidos-author

Stub. Drafting and scaffolding skill for the Eidos documentation standard
(the S9 authoring-assistance layer; see `Eidos.md` §22 and §23 S9, tracked
as `EIDOS-DRAFT-authoring-assistance`).

## Intended behavior (to be built)

- Prompt for `genre`, `scope`, `namespace`, and `title`; validate against the
  controlled vocabularies (`Eidos.md` §4, §5).
- Emit the YAML front-matter block (§7) and the per-genre section skeleton
  from `templates/` (§10, §14).
- Assign a provisional `<NAMESPACE>-DRAFT-<slug>` identifier (§13); note that
  the canonical `<NAMESPACE>-<NNNN>` is assigned by the steward at merge.
- Genre-specific seeding: prior-art notes for `Survey`/`Plan`; a Files table
  seeded from `git diff --stat` for `Log`.
- Record `provenance:` for LLM-assisted authoring (§7).

## Invariants

- This skill **proposes**; the §22 toolchain **disposes**. Scaffolded output
  is validated by the toolchain before it is considered conformant.
- Until `EIDOS-DRAFT-toolchain` exists, operate in advisory-only mode without
  the deterministic backstop.
