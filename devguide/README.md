# AlloMT developer guide

The current phase is **researcher-needs elicitation**, with several discussion
rounds expected. The maintained design documents distinguish what the researcher
wants, assistant interpretations, proposals, confirmed agreements and open questions.
Repository code, documentation and issue records use English.

| Document | Purpose |
| --- | --- |
| [Scientific objectives](OBJECTIVES.md) | Current R03 agreement: broad accepted scope, multiple approaches and continued exploration. |
| [Researcher needs](RESEARCHER_NEEDS.md) | Faithful inventory N01–N13; ordering does not imply priority. |
| [Component responsibilities](COMPONENT_RESPONSIBILITIES.md) | Delegated operations and AlloMT science; TopoMT, BindingMT, ElastNetMT and LandscapeMT coordination. |
| [Discussion history](DESIGN_DISCUSSION.md) | Dated rounds, source of statements, agreements and significant revisions. |
| [Open questions](DESIGN_QUESTIONS.md) | Unresolved scientific/product questions for later rounds. |
| [Coverage audit](DESIGN_AUDIT.md) | Traceability of all thirteen needs, R02 corrections and the R03 second revision. |
| [Accepted extensions](PROPOSED_EXTENSIONS.md) | P01–P10, accepted in R03; historical filename retained, provider work allocated. |
| [Methods and tools](METHODS_AND_TOOLS.md) | Established approaches and fourteen source-level tool/license profiles. |
| [Research landscape](RESEARCH_LANDSCAPE.md) | Recent developments through 2026-11-15 and their potential implications. |
| [Research references](RESEARCH_REFERENCES.md) | Primary sources, publication types and the immutable tool snapshot. |
| [Architecture notes](ARCHITECTURE.md) | Provisional implications and possible workflows, awaiting negotiation. |
| [Scientific scope](SCIENTIFIC_SCOPE.md) | Current product vision, inherited obligations and implementation boundary. |
| [Ecosystem map](ECOSYSTEM.md) | Component responsibilities and integration ownership. |
| [Roadmap notes](ROADMAP.md) | Current phase and conditional later work; no agreed feature-delivery order. |
| [Discussions upkeep](discussions.md) | Live scientific resource/function catalog, intake forms, triage and evidence/decision routing. |
| [Catalog routing index](discussions/catalog.json) | Thin machine-readable pointers to authoritative resource conversations. |

Start with accepted objectives, needs, responsibilities and the discussion history.
Use the methods/research and live catalog to continue broad exploration.
Update the relevant documents together as
the design evolves under [AlloMT #3](https://github.com/uibcdf/allomt/issues/3).

The repository foundation is tracked in
[AlloMT #1](https://github.com/uibcdf/allomt/issues/1), with central admission published under
[MolSysSuite #202](https://github.com/uibcdf/molsyssuite/issues/202). The first scientific
increment remains a later open implementation decision under
[AlloMT #2](https://github.com/uibcdf/allomt/issues/2); it does not bound objectives.

The source candidate contains contributor instructions, the
[reporting protocol](reporting_protocol.md), [pending bugs](pending_bugs/README.md),
[pending proposals](pending_proposals/README.md), [archive](archive/README.md)
and [report template](templates/report.md), derived from the official starter.
Run `python devtools/devguide_index.py --check` to validate the offline lifecycle.
Read [admission and bootstrap status](ADMISSION.md) for source provenance,
executed qualification and outstanding gates. Source preparation, accepted member
admission, scientific qualification and public package availability remain distinct.
