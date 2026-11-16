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

## R02 — Coverage audit, methods and research-informed possibilities, 2026-11-15

### Researcher request

Diego asked whether the documents captured every proposal, requested corrections
and improvements, and asked for possible overlooked objectives/functions informed
by traditional methods and recent allostery/pharmacological-design research.

### Coverage findings and corrections

[The audit](DESIGN_AUDIT.md) finds all thirteen explicit needs represented.
It strengthens N07's permissive-license wording to the requested initial selection
criterion and restores N13's broader improve/worsen meaning. The need to compare
orthosteric function/structure is preserved without assuming allostery necessarily
damages the site. Other scientific distinctions are clarified in the audit and
questions; no new function is counted as implemented.

### Recovered earlier assistant proposals

- I06: Public scientific operations, method implementations and traceable results
  were previously suggested as conceptual views. They are now explicit; no module
  tree, API or result schema follows automatically from them.
- I07: Contrasting hypotheses against computational/experimental references was
  an earlier proposed objective. It was too implicit and is now explicit in P07.

I06/I07 remain assistant proposals, not confirmed architecture or additional
researcher-stated requirements. I01–I05 keep their original status.

### Research and new proposals

[Methods/tools](METHODS_AND_TOOLS.md) compares established approaches and
fourteen repository/license snapshots. [The landscape](RESEARCH_LANDSCAPE.md)
discusses recent work through 2026-11-15, including peer-reviewed 2026 studies
and distinctly labeled preprint/software sources. The bibliography records
29 primary paper/documentation references. This was source inspection and a
targeted scoping review; no package/model installation or scientific benchmark ran.

[P01–P10](PROPOSED_EXTENSIONS.md) propose cryptic-pocket assessment, richer
functional profiles, quantitative coupling, mutation/rescue/resistance analysis,
selectivity/developability, informative experiments, calibrated comparisons,
dynamic/conditional mechanisms, other interventions and generative workflows.
All remain proposed. Their discussion order is a recommendation, not agreed
delivery priority. Scientific relevance, license suitability and runtime
qualification are kept separate.

### Agreement status and next discussion

The confirmed process G01–G03 continues. No scientific architecture, algorithm,
backend, public API, model, benchmark or first workflow has been agreed in R02.
Questions Q01–Q10 are refined; Q11/Q12 capture evaluation and proposal-scope choices.
Later rounds can accept, revise or reject these possibilities using concrete cases.

## Continuing the discussion

For each later round, record its date, the researcher's new or corrected
statements, interpretations/proposals, confirmed agreements and unresolved
questions. Update the current needs and design documents in the same increment.
Retain IDs and explain significant changes, including replaced or withdrawn
proposals. Ordinary document correction is allowed; meaningful decision history
and archived issue records retain their respective lifecycle rules.
