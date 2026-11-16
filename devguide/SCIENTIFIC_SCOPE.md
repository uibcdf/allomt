# Scientific scope

**Status:** researcher-needs elicitation. The intended product scope is being
negotiated over multiple rounds; architecture, methods, priorities and delivery
commitments remain open. The source currently provides repository infrastructure.

## Researcher vision

AlloMT (Allostery MultiToolkit) is intended to support prediction,
characterization and engineering of allosteric modulation within MolSysSuite
and MolI. The researcher's requested outcomes span target knowledge, candidate
sites and functional effects, mechanistic interpretation, computational
experiments, ligand/peptide design, molecular association and mutation effects.

The complete researcher-stated inventory is [N01–N13](RESEARCHER_NEEDS.md).
It includes individual protein targets, complexes/multimers and associations
involving DNA/RNA, as well as conformation-specific questions. The inventory
preserves the requested scope without selecting an implementation for it.

| Requested area | Needs |
| --- | --- |
| Site discovery, modulation direction and reported ligands | N01, N03, N04 |
| Mechanisms, communication paths and orthosteric function/structure | N02, N08 |
| MD experiment proposals, information-theory analysis and ML/AI | N05, N06 |
| Permissive third-party integration and stronger native algorithms | N07 |
| Bifunctional ortho-allo and conformation-selective molecular design | N09, N10 |
| Coordinated pharmacophore, binding and peptide workflows | N11 |
| Allosteric control of molecular association and mutation effects | N12, N13 |

The desired early use of third-party methods and future stronger native
algorithms are both part of the researcher's vision. Specific providers,
benchmarks, performance criteria, native-method transitions and timing have
not been chosen. Requesting a capability does not establish its validation.

## Negotiation and current design status

[The discussion history](DESIGN_DISCUSSION.md) records researcher statements,
assistant interpretations, proposals and confirmed agreements by round.
[Open questions](DESIGN_QUESTIONS.md) organize unresolved scientific and product
details. [Architecture notes](ARCHITECTURE.md) explore implications while
remaining explicitly provisional.

The current confirmed process is needs elicitation, several discussion rounds
and maintained documents that improve with the discussion. A first bounded
scientific workflow is still to be selected under
[AlloMT #2](https://github.com/uibcdf/allomt/issues/2). The broader negotiation
is tracked in [AlloMT #3](https://github.com/uibcdf/allomt/issues/3).

## Applicable scientific and ecosystem obligations

These inherited obligations remain applicable as the product design evolves:

- Preserve the distinction between a computed observation, its mechanistic
  interpretation and the evidence supporting a scientific claim. Retain
  assumptions, applicability, uncertainty, missing and unsupported outcomes.
- Reuse public provider operations for capabilities owned elsewhere. MolSysMT
  owns shared molecular representation/operations; ElastNetMT owns its
  elastic-network numerical work. Specialized topography, pharmacophore,
  binding, peptide, knowledge and visualization work retains its owning
  component. See [the ecosystem map](ECOSYSTEM.md).
- Preserve molecular identity, selections and resolved ordering, atom/group
  correspondence, chemical states and analyzed structures/frames where relevant.
  Indices and identifiers are distinct.
- Make physical quantities and conversions explicit through the shared
  PyUnitWizard policy; retain each method's actual units or dimensionless meaning.
- Identify method/backend/version, parameters, input preparation, provenance
  and execution status. Keep scientific results, SMonitor diagnostics,
  Ackredit references and optional Recorda execution records distinct.
- Introduce independently useful operations through concrete scientific
  contracts and meaningful checks when their workflows have been selected.

These obligations do not choose a universal allostery score, path model, result
class, method family or workflow architecture.

## R02 coverage review and research-informed proposals

[The design audit](DESIGN_AUDIT.md) confirms coverage of the thirteen stated
needs and makes earlier assistant proposals and scientific distinctions explicit.
It also corrects the initial permissive-license wording and the narrower mutation
heading while preserving the original need identities.

[Established methods/tools](METHODS_AND_TOOLS.md) and
[recent research](RESEARCH_LANDSCAPE.md) motivate
[P01–P10](PROPOSED_EXTENSIONS.md). They include possible operational clarifications
and broader functions; none becomes an agreed objective merely by appearing here.
The [references](RESEARCH_REFERENCES.md) distinguish primary studies, methods,
preprints and source/model documentation, with a review cutoff of 2026-11-15.

## Current implementation boundary

Repository/source receiving remains under
[AlloMT #1](https://github.com/uibcdf/allomt/issues/1).
No scientific predictor, communication-path algorithm, ML model, MD execution
route or molecular-design operation is implemented by this documentation.
Scientific dependencies, result contracts and operations will follow the
negotiated scientific increments.
