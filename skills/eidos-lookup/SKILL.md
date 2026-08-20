---
name: eidos-lookup
description: Resolve identifiers, decisions, open questions, and cross-references across a federated Eidos corpus. Use to answer "show me PSYCHE-D16", "what cites CLASSIC-0003?", "list ORIGIN open questions", or "give me the current LEXTER index" during authoring or review.
---

# eidos-lookup

Stub. Corpus-aware retrieval skill for the Eidos documentation standard
(the S9 authoring-assistance layer; see `Eidos.md` §22 and §23 S9, tracked
as `EIDOS-DRAFT-authoring-assistance`).

## Intended behavior (to be built)

- Resolve a document `id` or section anchor to its content (§5, §9).
- Resolve `D`/`O` register entries by id (§8) with their host document.
- Answer relationship queries: `relates-to`, `supersedes`, `cites`, and
  inbound backlinks across the federation (§9, §10).
- List a namespace's registry / INDEX (§13) or the federated master INDEX.
- Honor the federation manifest (the same one an S8 site build uses) so
  lookups span all participating repositories.

## Invariants

- Read-only over the corpus; makes no changes.
- Backed by the same front-matter parsing the §22 toolchain performs; does
  not reimplement it where the toolchain can be called.
