# Researcher needs

**Current phase:** researcher-needs elicitation, with several discussion rounds
expected. **Source:** Diego's complete thirteen-point statement on 2026-11-15,
recorded as round R01 in [the discussion history](DESIGN_DISCUSSION.md).
R02 audits coverage and adds research-informed possibilities in separate documents;
the thirteen researcher-stated needs retain their identities.

These are researcher-stated goals. They describe the intended scientific product;
they are not claims of implemented capability, a finalized specification or an
agreed delivery order. Need numbers preserve the original ordering, not priority.
Details, scope refinements and interpretation questions remain open for negotiation.

**R03 update:** the original needs remain in scope, and all ten additional P
objective classes have been accepted. Objective exploration stays broad and
open-ended. [OBJECTIVES.md](OBJECTIVES.md) records the current scientific direction;
[COMPONENT_RESPONSIBILITIES.md](COMPONENT_RESPONSIBILITIES.md) allocates reusable
operations without reducing the intended capabilities.

## N01 — Discover allosteric sites and predict modulation direction

Given a protein molecular target, obtain relevant functional knowledge, including
the active site when the target is an enzyme, for example by consulting Sabueso.
Report candidate allosteric sites suitable for designing an allosteric modulator,
and predict whether the modulation would be positive or negative.

This need includes both site discovery and the desired functional prediction.
The meaning of modulation direction, its reference and the information needed
to support it are discussion topics [Q02](DESIGN_QUESTIONS.md#q02--functional-reference-and-modulation-direction).
R02 makes pocket accessibility/ligandability, functional coupling and a particular
intervention's signed effect explicit as separate assessments in
[the audit](DESIGN_AUDIT.md).

## N02 — Characterize a reported mechanism and its communication paths

Given a protein and a reported allosteric site, characterize the allosteric
mechanism and provide its communication path, with atomic detail when possible.
The requested atomic resolution is conditional on what the method and evidence
can support. Mechanism/path outputs and their interpretation remain to be
specified in [Q04](DESIGN_QUESTIONS.md#q04--mechanisms-paths-and-resolution).

## N03 — Retrieve previously reported allosteric ligands

Given a molecular target, collect its reported allosteric ligands from Sabueso
and/or resources that consult databases and online sources. Preserve this as a
useful research workflow in its own right. Source coverage, identification,
experimental context and conflicting reports are open topics in
[Q03](DESIGN_QUESTIONS.md#q03--knowledge-retrieval-and-reported-modulators).

## N04 — Use rapid, inexpensive methods effectively

Given a target, predict allosteric sites as successfully as possible using fast,
inexpensive methods, including elastic-network models. Scientific success and
computational economy are both desired. Specific methods, cost limits and
evaluation criteria remain open in
[Q05](DESIGN_QUESTIONS.md#q05--accuracy-cost-and-rapid-screening).

## N05 — Propose and analyze molecular dynamics experiments

Propose molecular dynamics simulation experiments and analyze their results to
uncover and quantify allosteric mechanisms. Information-theory algorithms are
an explicit example of the desired analysis methods. Planning, simulation
execution, analysis and the eventual scientific conclusions need their own
definitions; automatic execution is not selected by this request. See
[Q06](DESIGN_QUESTIONS.md#q06--simulation-experiments-and-their-analysis).

## N06 — Integrate machine learning and AI

Use machine-learning and AI tools to predict allostery. The researcher has not
restricted this goal to one model family or one prediction endpoint. Inputs,
available pretrained models, training/fine-tuning needs and their evaluation
remain open in [Q07](DESIGN_QUESTIONS.md#q07--third-party-methods-native-research-and-ml).

## N07 — Begin with permissive third-party tools and develop stronger native methods

Initially integrate workflows with third-party tools under permissive licenses
for the intended use. Permissive licensing is the requested initial selection
criterion; availability or an open-source label alone does not establish it. In the
near future, develop our own algorithms to exceed the predictive capability of
the adopted third-party methods and better fit our scientific needs.

Native scientific development is an explicit ambition, not only adapter work.
The meaning of improvement, its evidence, timing and migration strategy are
still to be negotiated. No backend, model, dataset or benchmark has been selected.
See [Q07](DESIGN_QUESTIONS.md#q07--third-party-methods-native-research-and-ml).
The [source-level tool review](METHODS_AND_TOOLS.md) distinguishes core licenses,
bundled notices, models/data and unqualified routes. It selects no integration.

## N08 — Relate allosteric activity to orthosteric function and structure

Correlate allosteric activity with loss of function and/or structure at the
orthosteric site. Define the relevant functional and structural measurements,
comparisons and interpretation in later rounds. The distinctions among local
orthosteric changes, global stability and the measured activity are discussion
topics in [Q02](DESIGN_QUESTIONS.md#q02--functional-reference-and-modulation-direction)
and [Q06](DESIGN_QUESTIONS.md#q06--simulation-experiments-and-their-analysis).
This preserves the requested loss-of-function/structure comparison; it does not
define every allosteric mechanism as structural damage. Dynamic/entropic and
stability-versus-function distinctions are discussed in R02 and accepted objective P08.

## N09 — Help design bifunctional ortho-allo molecules

Support the design of long bifunctional molecules that engage an orthosteric
site and an allosteric site. Desired outputs, linked-molecule geometry,
simultaneous engagement and functional evaluation remain open in
[Q08](DESIGN_QUESTIONS.md#q08--molecular-design-and-conformational-selectivity).

## N10 — Design modulators selective for protein conformations

Use MolSysSuite tools to design ligands with specific allosteric effects on
specific protein conformations. This includes conformation-selective design,
with the desired state and functional effect made explicit during negotiation.
See [Q08](DESIGN_QUESTIONS.md#q08--molecular-design-and-conformational-selectivity).

## N11 — Compose multiple workflows with the scientific ecosystem

Integrate into the ecosystem so multiple workflows can be assembled. Explicit
examples are coordination with PharmacophoreMT to model a candidate allosteric
site pharmacophorically and screen compound libraries, and coordination with
BindingMT or PeptideMT when the allosteric modulator is a peptide.

These are requested collaborations, not assertions that every required provider
operation already exists. Workflow responsibilities and scientific handoffs are
open in [Q08](DESIGN_QUESTIONS.md#q08--molecular-design-and-conformational-selectivity)
and [the architecture notes](ARCHITECTURE.md).

## N12 — Modulate molecular association through allosteric regions

Given a protein complex, help design allosteric regions that affect and modulate
its ability to form. Extend this goal to multimers and associations involving
nonprotein molecules such as DNA or RNA. The intended regions, interventions,
assembly states and association measurements need clarification in
[Q09](DESIGN_QUESTIONS.md#q09--assembly-modulation-and-mutation-design).

## N13 — Predict mutations that improve or worsen a known allosteric mechanism

Predict mutations that improve or worsen a known allosteric mechanism. The
baseline mechanism and the meaning of improvement/worsening are part of the
scientific question. Mutation scope and evaluation are open in
[Q09](DESIGN_QUESTIONS.md#q09--assembly-modulation-and-mutation-design).
Improvement has not been defined as increasing a coupling-score magnitude.
The revised heading preserves the researcher's broader wording; potential
epistasis, rescue and resistance functions are accepted extensions in P04.

## Current coverage and next rounds

All thirteen stated needs are recorded. Priorities, representative cases, success
criteria, public operations, result contracts, source layout and method choices
remain under discussion. [Q10](DESIGN_QUESTIONS.md#q10--illustrative-cases-and-later-implementation-priorities)
supports broad exploration with diverse examples; a later implementation choice
does not define or close the objectives.

Update this inventory as the researcher clarifies the needs. Retain stable IDs,
record significant changes and their reasons in [the discussion history](DESIGN_DISCUSSION.md),
and distinguish a revised need from an assistant's proposed implementation.
The design discussion is tracked in [AlloMT #3](https://github.com/uibcdf/allomt/issues/3).

The R02 [coverage audit](DESIGN_AUDIT.md) traces all thirteen needs and earlier
assistant proposals. [P01–P10](PROPOSED_EXTENSIONS.md), introduced as possibilities
in R02, are accepted objective classes as of R03; their historical IDs remain.
[Methods/tools](METHODS_AND_TOOLS.md)
and [recent research](RESEARCH_LANDSCAPE.md) provide their evidence and limits.
