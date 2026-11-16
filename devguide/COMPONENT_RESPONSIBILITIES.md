# Component responsibilities and coordination

**Updated:** R03, 2026-11-15. **Authority:** the researcher's explicit ownership
directions, existing component responsibilities and applicable suite governance.
This is AlloMT's coordination map, not a unilateral replacement for provider
contracts or the central member registry.

## Allocation by scientific operation

| Reusable operation/domain | Scientific owner or coordination route | AlloMT contribution | Evidence/status boundary |
| --- | --- | --- | --- |
| Molecular representations, acquisition, chemistry, selections, identity maps and general structural operations | MolSysMT | Select scientifically relevant inputs and preserve their identities in allosteric analyses. | Consume qualified public operations; do not recreate molecular infrastructure here. |
| Pocket/cavity/topography detection, including cryptic pockets across conformations | TopoMT; consume structures/ensembles from their owners | Assess allosteric relevance, coupling and intervention opportunities using detected regions and other evidence. | Explicitly assigned to TopoMT by Diego in R03. Detection is not an AlloMT primitive. |
| Docking, binding/complex modeling, binding affinity and binding free-energy calculation or prediction | BindingMT | Define allosteric design questions and state/partner comparisons; consume binding results and interpret functional relevance. | Binding free-energy operations are BindingMT-owned even when used in an allosteric cycle. Current qualified profiles remain narrower than the accepted domain. |
| ENM construction, modes, covariance and reusable mechanical perturbation/spectral-response calculations | ElastNetMT | Develop allostery-specific questions, derived analyses and interpretation using the numerical outputs. | PRS/ESSA-like needs are coordinated here; this map does not assert that every requested public operation already exists. |
| General conformational exploration, metastable states, conformational FELs, reduction/reweighting, kinetics and ensemble inference | LandscapeMT, with owner coordination in [LandscapeMT #1](https://github.com/uibcdf/landscapemt/issues/1) | Define/use allosterically relevant comparisons, hypotheses and functional interpretations of provider results. | Newly introduced provider; scope/preview directions are not implemented API or received scientific evidence. |
| Atom/residue allosteric communication, functional response interpretation, allostery-specific coupling and mutation/mechanism analysis | AlloMT, composing generic molecular, mechanical, binding and landscape tools | Develop reusable native allostery-specific scientific operations and combine appropriate evidence. | Methods and result meanings follow concrete tasks; no single universal allosteric scheme is imposed. |
| Pharmacophore modeling, comparison and library-screening operations | PharmacophoreMT | Supply allosteric regions, state/function objectives and interpret candidate relevance. | Do not create a second generic pharmacophore/screening engine. |
| Peptide generation/redesign and peptide-specific evaluation | PeptideMT; binding/complex questions with BindingMT | Set the desired allosteric effect and integrate peptide, binding and mechanism evidence. | Availability of a peptide modality depends on the actual received provider profile. |
| Scientific knowledge, target/site/ligand reports and source curation | Sabueso and its appropriate source/provider routes | Request and contextualize relevant knowledge and preserve provenance. | The resource catalog stores curation conversations/pointers, not a duplicate target-knowledge database. |
| Molecular rendering and interaction | MolSysViewer/MolSysSketcher and owner-specific add-ons | Present allosteric results and preserve molecular/result correspondence. | Visualization is distinct from scientific inference. |
| Generic developability/ADMET operations | Relevant scientific provider; coordinate ViableMT's intended direction when concrete capabilities exist | Define how such constraints contribute to the allosteric design objective. | ViableMT was conceptual in the reviewed source; no usable API is assumed. |
| Platform/project orchestration and durable scientific project/evidence management | Established MolI/Praxis/Nextia/agent ownership | Expose independently useful allostery operations, local compositions and experiment proposals. | Do not create a second general scheduler/project platform in AlloMT. |

## Distinctions that prevent accidental overlap

- **Binding energy and FEL:** BindingMT owns binding-specific energetic endpoints.
  LandscapeMT's intended general conformational free-energy/state analyses are
  a different operation domain. AlloMT defines the allosteric comparison and
  interprets the corresponding results; it does not duplicate either engine.
- **Two kinds of paths:** state-to-state conformational transition paths/fluxes
  are coordinated with LandscapeMT. Atom/residue communication hypotheses and
  their allosteric interpretation are AlloMT questions, reusing appropriate
  generic providers. A shared word such as path or network does not establish
  identical contracts.
- **Cryptic sites:** LandscapeMT can supply conformational exploration/ensembles;
  TopoMT detects topographic opportunities; AlloMT investigates allosteric relevance.
  This is one possible composition, not the universal shape of an AlloMT workflow.
- **A library is not an ownership boundary:** the same external package may offer
  generic and allostery-specific functions. Route each operation by its scientific
  endpoint instead of importing an entire provider's responsibility into AlloMT.

## Accepted P01–P10 with shared responsibilities

| Objective | Delegated/reused work | AlloMT scientific responsibility |
| --- | --- | --- |
| P01 | TopoMT pockets; MolSysMT/LandscapeMT inputs | Allosteric opportunity, coupling and context-dependent interpretation. |
| P02 | BindingMT binding endpoints; relevant molecular/landscape providers | Functional profiles and allosteric interpretation across suitable approaches. |
| P03 | BindingMT binding energies; LandscapeMT FEL/state/kinetic estimates | Define coupling questions/comparisons and interpret their allosteric significance. |
| P04 | MolSysMT molecular changes; relevant stability/binding/landscape providers | Allosteric mutation, epistasis, rescue and resistance questions/analyses. |
| P05 | PharmacophoreMT, BindingMT, PeptideMT and qualified developability providers | Allosteric selectivity and functional design criteria/comparisons. |
| P06 | Simulation/sampling and platform execution owners | Allostery-specific information utility, hypotheses and next-study proposals. |
| P07 | Provider scientific results, existing developer tools and knowledge sources | Allostery-task validation, metrics, reference cases and scientific comparisons. |
| P08 | Appropriate molecular, sampling, landscape and analysis providers | Allosteric dynamic/condition-dependent mechanisms and interpretation. |
| P09 | BindingMT, PeptideMT and other modality-specific owners | Allosteric intervention/association questions and corresponding evaluation. |
| P10 | LandscapeMT ensemble inference; molecular/binding/design providers | Allosteric objectives, comparisons and scientific criteria for generated candidates. |

## Coordination procedure

Inspect the provider's current public contract and received scope before relying
on an operation. Report a concrete missing capability or proposed change in its
owning repository, link the AlloMT use case and retain the response/contract there.
Use central MolSysSuite coordination when a genuinely shared contract or policy
needs agreement. AlloMT keeps the consuming scientific question and integration work.

LandscapeMT's initial overlapping application descriptions are being coordinated
in its owning issue above. No source changes or PR were made in that repository.
Provider scope, publication and actual implementation remain separate observations.

Possible handoff information includes molecular/state/ensemble identity, maps,
resolution, weights/bias/time semantics, quantities/definitions, uncertainty,
method/source and applicable evidence. Negotiate the fields needed by each
specific boundary; this list does not impose one universal schema.
