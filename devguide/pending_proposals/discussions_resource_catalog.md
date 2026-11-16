---
summary: Establish and maintain a Discussions catalog of scientific resources and functions.
issue: uibcdf/allomt#4
status: active
opened: 2026-11-15
closed:
verification: inspected
area: [scientific-design, discussions, resources]
guard:
normative:
blocked_by: []
supersedes: []
---

# Discussions scientific resource catalog

## What

Begin a maintained storage/curation mechanism for tools, methods, functions,
databases, datasets, benchmarks, literature and other resources of interest.
The researcher requested this alongside broad AlloMT objective exploration in R03.

## How

Enable Discussions, inspect existing content/categories, preserve useful history,
publish a discoverable catalog with representative conversations, and maintain
intake forms, upkeep guidance and a thin source-controlled routing index.
Substantive reviews remain in conversations, with decisions and actionable work
linked to their owning issues or versioned records.

## Why

Resources and functions span several MolSysSuite components. Recording scientific
interest, operation ownership, rights, assessment evidence and adoption separately
prevents the catalog from becoming a duplicate provider implementation, a second
Sabueso knowledge base or an implicit dependency list.

## Evidence and current status, 2026-11-15

- Native GitHub API initially reported Discussions disabled and no content or
  categories. Activation generated six defaults; all were retained, with no
  deletions. Names/slugs/default descriptions and Q&A answerability were observed.
- [Catalog #5](https://github.com/uibcdf/allomt/discussions/5) links eleven entries
  (#6 through #16): ProDy, MoCHI, PASSer2.0,
  AlloViz, PRS/ESSA, TopoMT pockets, BindingMT binding energies, LandscapeMT
  coordination, ASD, task-specific benchmarks and the research dossier.
  Each actual identity is in [catalog.json](../discussions/catalog.json).
- [Upkeep guidance](../discussions.md) assigns General to resources and Ideas
  to functions/workflows; it defines sources, canonical keys, duplicates, dated
  reviews, rights/evidence, owner routing and reciprocal issue/decision links.
- Source forms match observed `general` and `ideas` slugs. The available API
  exposes creation/update of discussions but no category-format editor or pinning.
  No rendered form, Announcement/Open-ended format, description edit or pinning
  is certified by source/API checks.

These are catalog/source observations. No scientific package, model, dataset,
algorithm or provider integration was installed, executed or adopted by this work.

## Remaining receiving and bounded follow-up

Owner: Diego Prada Gracia. Review by **2026-12-15**. Verify Announcements/Ideas
formats and General/Ideas form rendering in GitHub's UI; consider description
adaptation there. The available API/editor cannot provide this evidence.
Interim communication uses the live General/Ideas threads and documented fields.
Remove the pending state when UI observations are recorded in the owning issue.
The catalog remains available for curation while this receiving evidence is pending.

## What was refuted

Creating source forms alone does not configure or verify remote category formats.
Catalog inclusion, votes and closure are not software adoption or scientific
qualification. A resource for another component does not transfer its ownership.

## Scope and exclusions

Own catalog setup and receiving, not completion of the scientific inventory,
method selection, data mirroring or implementation. Objectives/design remain
under uibcdf/allomt#3. Missing provider capabilities retain their own issues.

## Acceptance criteria

- Activation/categories/content have actual observation evidence.
- A live index links representative resource and function conversations.
- Forms, upkeep guidance and thin routing index are committed and checked.
- Reviews preserve sources, rights, owner allocation, evidence and dated decisions.
- UI-only receiving is observed or retained as an owned, bounded follow-up;
  unobserved settings are never marked verified.

This record stays active for remaining UI receiving and catalog refinement.
