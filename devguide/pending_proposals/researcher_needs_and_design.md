---
summary: Maintain researcher needs and the negotiated AlloMT design across discussion rounds.
issue: uibcdf/allomt#3
status: active
opened: 2026-11-15
closed:
verification: inspected
area: [scientific-design, requirements]
guard:
normative:
blocked_by: []
supersedes: []
---

# Researcher needs and iterative design

## What

Maintain the scientific/product needs and the evolving AlloMT design throughout
several discussion rounds. The current phase is understanding the researcher's
needs; it does not finalize architecture, methods or implementation priorities.

## How

Use [the need inventory](../RESEARCHER_NEEDS.md),
[discussion history](../DESIGN_DISCUSSION.md),
[open questions](../DESIGN_QUESTIONS.md) and
[architecture notes](../ARCHITECTURE.md) as the maintained design surface.
Distinguish researcher statements, assistant interpretations, proposals, confirmed
agreements and unresolved questions. Retain stable IDs and reasons for significant
changes; reconcile each new round into the current documents and its history.

## Why

The researcher supplied thirteen needs spanning knowledge, prediction,
mechanisms, experiments, native/third-party methods, ML and molecular engineering,
and explicitly requested that the negotiated design be documented and improved.
This scope must remain recoverable without reconstructing the conversation.

## Evidence and current status

R01 records the complete researcher statement and the agreement to iterate in
developer-guide documents. N01–N13 are captured; Q01–Q10 and interpretations
I01–I05 remain open. Only the discussion process G01–G03 is explicitly confirmed.
No algorithm, provider, scientific result contract or source layout was selected.
Verification concerns document/source inspection, not scientific execution.

R02 audits all thirteen needs and earlier assistant proposals, corrects N07/N13
wording and records interpretations I06/I07, proposed extensions P01–P10 and
refined/open questions Q01–Q12. The supporting method/tool and recent-research
review cites 29 primary paper/documentation references and fourteen immutable
repository/license snapshots. This is a targeted scoping/source review, with
publication types and limitations explicit. No scientific benchmark, model
download, third-party installation or runtime qualification was performed.
No new proposal was recorded as an agreed objective or method choice in R02.

R03 records Diego's acceptance of P01–P10 and the traditional method families,
while explicitly retaining open-ended objective exploration and multiple
conceptual approaches/applications. [OBJECTIVES.md](../OBJECTIVES.md) and the
[responsibility matrix](../COMPONENT_RESPONSIBILITIES.md) distinguish accepted
goals from provider operations, adoption and executed scientific evidence.
TopoMT owns cryptic-pocket detection, BindingMT binding energetics, ElastNetMT
reusable ENM work, and general landscape/state/kinetic work is coordinated with
LandscapeMT. Its owning coordination issue is uibcdf/landscapemt#1; no source
changes or PR were made there. Catalog receiving/upkeep belongs to uibcdf/allomt#4.

G04–G07 record accepted breadth, operation ownership, continued exploration and
Discussions curation. The previous recommendation to focus discussion on a
subset is superseded. A later implementation increment does not restrict global
objectives. Software architecture, APIs, backends and priorities remain open;
acceptance of method families does not waive the permissive licensing criterion.

## What was refuted

No scientific method or architecture was evaluated and rejected in R01. The
earlier seed scope and examples do not constrain the newly stated needs.

## Scope and exclusions

This issue owns the ongoing design conversation and its documents. The first
bounded scientific workflow remains uibcdf/allomt#2; repository/member receiving
remains uibcdf/allomt#1. Provider changes retain their owning issues. Capturing a
need does not implement it or commission an experiment, model download or release.

## Acceptance criteria

- All researcher-stated needs are faithfully recorded and can be traced to a round.
- The reading path exposes current needs, questions, proposals and agreements.
- New rounds update the relevant documents and preserve significant rationale.
- Methods, API, priorities and architecture are marked according to their actual
  discussion status; confirmed choices are not inferred from assistant suggestions.
- Local report metadata, links and generated indexes remain consistent.

This theme stays active while the design is being negotiated.
