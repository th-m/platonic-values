# AGENTS Operating Guide

This document defines how AI agents should work in this repository.

## Mission

Help build a coherent philosophical book on **Platonic Value Theory** by producing structured, crosslinked notes that are useful to both humans and AI in Obsidian.

## Scope and Non-Goals

- Scope: drafting, refining, linking, and organizing notes inside `notes/`.
- Non-goal: do not auto-delete, auto-merge, or bulk-move notes unless explicitly requested.
- This workflow is documentation-first and graph-first: preserve traceability of ideas.

## Tone Rules for Philosophical Drafting

- Write clearly and precisely, without flattening conceptual nuance.
- Separate assertion from evidence from speculation.
- Steelman rival positions before critique.
- Preserve the author's conceptual vocabulary (virtue-commodities, Platonic value theory, 5x3 framework).

## Canonical Taxonomy

Use these locations when creating new notes:

- `notes/core/`
- `notes/ideation/metalogic/`
- `notes/ideation/philosophy/`
- `notes/ideation/psychology/`
- `notes/ideation/theology/`
- `notes/composition/`

Current repo state may still contain core-candidate notes at `notes/` root. Do not move files unless asked.

## Deterministic Classification Decision Path

When placing a new note, follow this order:

1. If the note defines, revises, or formalizes the five virtue-commodities or core framework primitives, place it in `notes/core/` and set `system_of_study: core`.
2. Else if the note is primarily formal-logical, set-theoretic, meta-mathematical, or proof-structure oriented, place it in `notes/ideation/metalogic/`.
3. Else if the note is primarily conceptual-argumentative (ontology, epistemology, ethics, truth/value theory), place it in `notes/ideation/philosophy/`.
4. Else if the note is primarily psychological (archetypes, cognition, motivation, development, pathology), place it in `notes/ideation/psychology/`.
5. Else if the note is primarily theological/spiritual-anthropological, place it in `notes/ideation/theology/`.
6. Else if the note is mainly about chapter flow, motifs, narrative structure, or presentation strategy, place it in `notes/composition/`.
7. If multiple categories apply, choose the folder matching the **main claim**, then express secondaries in `themes` and crosslinks.

## Required Metadata Contract

Every new or substantially revised note must include frontmatter:

```yaml
---
status: seed
system_of_study: philosophy
themes:
  - platonic-value-theory
aliases: []
---
```

Allowed `status` values:

- `seed`
- `draft`
- `developing`
- `chapter-candidate`
- `canonical`
- `archive`

Allowed `system_of_study` values:

- `core`
- `metalogic`
- `philosophy`
- `psychology`
- `theology`
- `composition`

Status lifecycle expectation:

1. `seed` -> `draft`
2. `draft` -> `developing`
3. `developing` -> `chapter-candidate`
4. `chapter-candidate` -> `canonical` (if foundational) or remain chapter source
5. Any superseded note -> `archive`

## Obsidian Link Standards

Use wikilinks for all internal note references:

- Standard: `[[five-fundamental-values]]`
- Alias: `[[value-framework|5x3 framework]]`
- Heading link: `[[value-framework#The Framework Structure]]`
- Disambiguated path link: `[[ideation/philosophy/theories-of-value]]`

Rules:

- Prefer linking to canonical notes when known.
- If ambiguity exists, use folder-qualified links.
- Keep internal linking in wikilink format only (no Markdown links between notes).

## Crosslink Minimum Policy

For each new standalone note, include links to:

- At least one core concept note.
- At least one note from the same system of study.
- At least one adjacent system note when relevant.

Goal: maintain a dense, navigable knowledge graph instead of isolated essays.

## Duplicate-Handling Protocol

When duplicates or near-duplicates are found:

1. Flag the pair in your response and recommend a canonical target.
2. Prefer the canonical candidate with stronger structure, clearer argument, and richer links.
3. Do not delete either file automatically.
4. Do not rename files automatically unless explicitly requested.
5. If editing is requested, preserve both until the user approves consolidation.

Initial known normalization targets:

- `notes/empirical-validation-spirit.md` vs `notes/empirical-validation-spirit-1.md`
- `notes/ideation/philosophy/theories-of-value.md` vs `notes/ideation/philosophy/theories-values.md`

