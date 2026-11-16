# AlloMT developer guide

The current phase is **researcher-needs elicitation**, with several discussion
rounds expected. The maintained design documents distinguish what the researcher
wants, assistant interpretations, proposals, confirmed agreements and open questions.
Repository code, documentation and issue records use English.

| Document | Purpose |
| --- | --- |
| [Researcher needs](RESEARCHER_NEEDS.md) | Faithful inventory N01–N13; ordering does not imply priority. |
| [Discussion history](DESIGN_DISCUSSION.md) | Dated rounds, source of statements, agreements and significant revisions. |
| [Open questions](DESIGN_QUESTIONS.md) | Unresolved scientific/product questions for later rounds. |
| [Architecture notes](ARCHITECTURE.md) | Provisional implications and possible workflows, awaiting negotiation. |
| [Scientific scope](SCIENTIFIC_SCOPE.md) | Current product vision, inherited obligations and implementation boundary. |
| [Ecosystem map](ECOSYSTEM.md) | Component responsibilities and integration ownership. |
| [Roadmap notes](ROADMAP.md) | Current phase and conditional later work; no agreed feature-delivery order. |

Start with the needs and discussion history. Update these documents together as
the design evolves under [AlloMT #3](https://github.com/uibcdf/allomt/issues/3).

The repository foundation is tracked in
[AlloMT #1](https://github.com/uibcdf/allomt/issues/1), with central admission requested in
[MolSysSuite #202](https://github.com/uibcdf/molsyssuite/issues/202). The first scientific
workflow remains an open design decision under
[AlloMT #2](https://github.com/uibcdf/allomt/issues/2).

The source candidate contains contributor instructions, the
[reporting protocol](reporting_protocol.md), [pending bugs](pending_bugs/README.md),
[pending proposals](pending_proposals/README.md), [archive](archive/README.md)
and [report template](templates/report.md), derived from the official starter.
Run `python devtools/devguide_index.py --check` to validate the offline lifecycle.
Read [admission and bootstrap status](ADMISSION.md) for source provenance,
executed qualification and outstanding gates. Source preparation, accepted member
admission, scientific qualification and public package availability remain distinct.
