# Platonic Values Book Workspace

This repository is the working vault for a philosophical book on **Platonic Value Theory**: five fundamental virtue-commodities (Physical, Others, Self, Mental, Spirit) that structure human flourishing, distortion, and meaning.

## Project Thesis

The book develops and tests a central claim:

- Human value can be mapped through five foundational domains (virtue-commodities).
- Virtues and vices are patterns of right or distorted relation to those domains.
- Cross-disciplinary analysis (metalogic, philosophy, psychology, theology) clarifies and stress-tests the model.

## Canonical Notes Taxonomy

All writing lives under `notes/`.

- `notes/core/`
  Foundational canon for the Platonic value theory and the five virtue-commodities.
- `notes/ideation/metalogic/`
  Formal and meta-mathematical framing, logical structure, proof-theoretic implications.
- `notes/ideation/philosophy/`
  Ontology, epistemology, ethics, theories of truth/value, conceptual argumentation.
- `notes/ideation/psychology/`
  Archetypes, motivational structure, developmental and cognitive framing.
- `notes/ideation/theology/`
  Theological grounding, spiritual anthropology, comparative religious insight.
- `notes/composition/`
  Book architecture, motifs, chapter strategy, narrative flow.

This pass is docs-only: current files remain in place even when they are future `core` candidates.

## Obsidian Setup and Linking Rules

Recommended vault root: `notes/`

- Use Obsidian wikilinks for internal references: `[[five-fundamental-values]]`
- Use alias links for prose readability: `[[value-framework|5x3 framework]]`
- Use heading anchors for precision: `[[value-framework#The Framework Structure]]`
- For disambiguation, use folder-qualified links (from vault root): `[[ideation/philosophy/theories-of-value]]`
- Do not use Markdown links for internal note-to-note references.

## Required Note Metadata

Every new or substantially revised note should begin with YAML frontmatter:

```yaml
---
status: seed
system_of_study: philosophy
themes:
  - platonic-value-theory
  - virtue-commodities
aliases: []
---
```

Allowed `status` values:

- `seed` (raw capture)
- `draft` (structured but incomplete)
- `developing` (expanding evidence, objections, synthesis)
- `chapter-candidate` (near manuscript quality)
- `canonical` (accepted core reference)
- `archive` (retired or merged out)

Allowed `system_of_study` values:

- `core`
- `metalogic`
- `philosophy`
- `psychology`
- `theology`
- `composition`

## Human Writing Workflow

Use this flow for each idea:

1. `Capture`  
   Create or append to a note in the best-fit folder with `status: seed`.
2. `Classify`  
   Set `system_of_study` and `themes` so the note has a clear intellectual home.
3. `Link`  
   Add wikilinks to at least one core concept and adjacent supporting notes.
4. `Refine`  
   Improve argument clarity, evidence, objections, and conceptual distinctions.
5. `Chapter-ready`  
   Promote to `chapter-candidate` once the note can be used directly in manuscript drafting.

## Split / Merge Guidance

Split a note when:

- It contains more than one main thesis.
- It mixes systems-of-study without a clear primary argument.
- It grows too broad to link and navigate cleanly in Obsidian.

Merge notes when:

- They are near-duplicates or materially overlap.
- One note is clearly the stronger canonical version.

## Initial Normalization Targets (Guidance Only)

These are known duplicate pairs to normalize in a later cleanup pass:

- `notes/empirical-validation-spirit.md` and `notes/empirical-validation-spirit-1.md`
- `notes/ideation/philosophy/theories-of-value.md` and `notes/ideation/philosophy/theories-values.md`

For now, do not delete or move either file automatically. Flag and recommend a canonical merge target.

