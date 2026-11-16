# Scientific objectives

**Current agreement:** discussion round R03, 2026-11-15.
**Scope:** broad, open-ended exploration of allostery and its applications.
**Owner record:** [AlloMT #3](https://github.com/uibcdf/allomt/issues/3).

AlloMT is intended to be a versatile and powerful scientific multitool for
predicting, characterizing, understanding and engineering allostery. Drug design
is a major application; the design must accommodate multiple scientific questions,
conceptual approaches, representations, interventions and workflows. Objective
exploration remains open to further needs and applications.

## Accepted objectives and scientific breadth

The original researcher needs [N01–N13](RESEARCHER_NEEDS.md) remain the source of
the initial vision. Diego accepted all ten additional objective classes P01–P10
in R03. Their detailed register retains its historical filename
[PROPOSED_EXTENSIONS.md](PROPOSED_EXTENSIONS.md), but their status is now
**accepted scientific objectives**, with implementation responsibilities allocated
across the ecosystem.

The resulting scope includes:

- discovery and assessment of allosteric sites/regions, including opportunities
  exposed by alternative conformations;
- reported ligands, biological/experimental knowledge and evidence comparisons;
- functional profiles, mechanisms, communication hypotheses, energetic/kinetic
  coupling, dynamics, disorder and condition dependence;
- mutation, epistasis, rescue, resistance and molecular-association questions;
- simulation/experimental proposals, information-based analysis, active learning
  and scientific validation;
- conformation-selective, bifunctional, peptide and other molecular-design
  objectives, selectivity and developability constraints;
- native scientific algorithm development and qualified reuse of physical,
  statistical, information-theoretic, experimental and ML/AI methods.

This list can grow. It is not a closed ontology or a requirement that every
operation follow one pocket-to-ligand, perturbation-response, network-path,
thermodynamic-cycle or other universal scheme. Each scientific operation can
use the assumptions, quantities and evidence appropriate to its purpose.

## Scientific ambition through ecosystem composition

An objective can be in AlloMT's scientific scope while a reusable constituent
operation belongs to another component. For example, TopoMT detects cryptic
pockets and BindingMT estimates/calculates binding energies. AlloMT poses the
allosteric question, combines relevant outputs and develops the corresponding
allostery-specific analysis, interpretation and design criteria.

[COMPONENT_RESPONSIBILITIES.md](COMPONENT_RESPONSIBILITIES.md) allocates these
responsibilities, including ElastNetMT and the new LandscapeMT. Native research
on generic provider capabilities is coordinated in that provider; native
allostery-specific methods remain a substantive AlloMT development direction.
Composition does not reduce AlloMT to a fixed pipeline or a thin collection of
external command wrappers.

## What acceptance establishes

Acceptance establishes the objectives and their broad scientific relevance.
It does not declare every provider operation implemented, select a third-party
package/model, waive the requested permissive-license criterion, define a public
API or establish scientific/runtime qualification.

The surveyed traditional method families are accepted as relevant to explore.
Generic ENM, landscape, pocket and binding work keeps its owning component.
Method-specific contracts, compatible inputs and received evidence are negotiated
when concrete integrations are needed; they do not gate further objective exploration.

## Continuing exploration and later implementation

Keep eliciting goals and exploring different applications and conceptual routes.
Examples, priorities and a bounded implementation increment can be chosen later
without shrinking the overall product scope. [AlloMT #2](https://github.com/uibcdf/allomt/issues/2)
tracks a future first increment, not the definition or closure of AlloMT's objectives.

Keep resource discovery open through the [Discussions catalog process](discussions.md).
Catalog interest, goal acceptance, provider ownership, tool adoption and executed
evidence are independent statements. Record agreements and revised interpretations
in [the discussion history](DESIGN_DISCUSSION.md).
