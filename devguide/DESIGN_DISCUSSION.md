# Design discussion history

**Current phase:** researcher-needs elicitation.
**Owning issue:** [AlloMT #3](https://github.com/uibcdf/allomt/issues/3).

This is a living record of the negotiation. The current needs are maintained in
[RESEARCHER_NEEDS.md](RESEARCHER_NEEDS.md), open questions in
[DESIGN_QUESTIONS.md](DESIGN_QUESTIONS.md), and architectural interpretations in
[ARCHITECTURE.md](ARCHITECTURE.md). The history explains how those documents evolve.

## Statement status

- **Researcher-stated need:** an outcome or constraint requested by the researcher.
- **Assistant interpretation:** an attempted understanding, awaiting confirmation
  wherever it goes beyond the researcher's words.
- **Proposal:** a possible design, method, priority or implementation choice.
- **Confirmed agreement:** a decision explicitly established in the discussion.
- **Open question:** a point that remains unresolved.

A requested scientific outcome does not by itself select its method, assert
feasibility for every input, or establish an implementation deadline. Priorities
are recorded only when negotiated. Source capability and validation keep their
own evidence in the relevant implementation issues.

## R01 — Researcher vision and discussion process, 2026-11-15

### Researcher statements

Diego supplied the thirteen needs recorded as N01–N13. They cover discovery and
functional prediction, reported knowledge, mechanism/path characterization,
rapid elastic-network methods, simulation experiments and information theory,
ML/AI, permissive third-party tools and stronger native algorithms, orthosteric
function/structure relationships, bifunctional and conformation-selective
ligands, ecosystem workflows, assembly modulation including DNA/RNA, and
mutation effects on known allostery.

Diego then requested a maintained set of developer-guide documents capturing the
design being negotiated. Several rounds are expected, and the present phase is
understanding the researcher's needs. These instructions govern this design work.

### Confirmed process agreements

- G01: The current phase is researcher-needs elicitation.
- G02: The design will be discussed over several rounds.
- G03: The relevant developer-guide documents will accumulate and improve as the
  discussion progresses, preserving needs, proposals, questions and agreements.

### Assistant interpretations awaiting discussion

- I01: A scientific context may need to describe a molecular system/assembly and
  its functional reference, rather than assuming every workflow is a single
  isolated enzyme. This follows from N01, N10 and N12; no class hierarchy is chosen.
- I02: Modulation direction may need a declared intervention, reference and
  functional observable. How the user supplies these or AlloMT proposes them is
  open, as is the handling of unsupported predictions (N01, N08, N10, N12, N13).
- I03: Knowledge retrieval, discovery, characterization, design and simulation
  analysis may be independently useful operations with several composable entry
  points (N01–N13). Workflow boundaries and public API remain open.
- I04: Communication paths may need resolution and uncertainty qualifications,
  and possibly multiple paths rather than one forced answer (N02, N05).
- I05: Backend-independent scientific questions could let native methods be
  compared with and eventually replace selected third-party implementations
  while retaining method-specific meaning (N04, N06, N07).

These interpretations are not confirmed product/architecture decisions.

### Still open after R01

The first scientific workflow, representative target, modulation semantics,
result contracts, numerical methods, ML models, third-party providers, source
layout, public API, performance targets and delivery priorities remain open.
No scientific algorithms or integrations were implemented during this round.

### Document changes in this round

- Captured N01–N13 without treating their order as priority.
- Added the discussion history, question register and provisional architecture
  notes; reconciled the scientific scope and reading path with the expanded vision.
- Kept [AlloMT #2](https://github.com/uibcdf/allomt/issues/2) for the later first
  bounded workflow; this elicitation does not mark its contract selected.

## Continuing the discussion

For each later round, record its date, the researcher's new or corrected
statements, interpretations/proposals, confirmed agreements and unresolved
questions. Update the current needs and design documents in the same increment.
Retain IDs and explain significant changes, including replaced or withdrawn
proposals. Ordinary document correction is allowed; meaningful decision history
and archived issue records retain their respective lifecycle rules.
