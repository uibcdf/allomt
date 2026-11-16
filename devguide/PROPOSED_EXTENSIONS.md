# Accepted extensions and scientific functions

**Introduced:** R02. **Accepted:** R03, 2026-11-15, all ten objective classes.
The historical filename and P01–P10 identities are retained for traceability.
They complement [N01–N13](RESEARCHER_NEEDS.md); they do not close the objective
search or establish an implementation order. See [the scientific objectives](OBJECTIVES.md).

Acceptance concerns scientific scope, not exclusive implementation ownership,
backend adoption or qualification. [The responsibility map](COMPONENT_RESPONSIBILITIES.md)
allocates reusable operations to the owning components. Specific scientific
questions and contracts remain open without forcing one conceptual framework.

Evidence and reasoning are linked through [the research landscape](RESEARCH_LANDSCAPE.md)
and [methods/tools](METHODS_AND_TOOLS.md). Scientific interpretations and proposed
software functions remain distinguished from demonstrated upstream results.

## P01 — Cryptic pockets and separate site assessments

- Related needs: N01, N04, N10. Type: extension/clarification.
- Functions in scope: detect intermittent/hidden pockets across supplied or
  generated conformations; assess their accessibility, ligandability and
  coupling to a functional region separately; compare state-dependent opportunities.
- Motivation: ensemble generation and experimental pocket mapping offer
  complementary inputs ([T01](RESEARCH_LANDSCAPE.md#t01--ensembles-and-cryptic-opportunities-beyond-a-single-structure),
  [T06](RESEARCH_LANDSCAPE.md#t06--covalent-and-experimentally-exposed-cryptic-sites)).
- Open: pocket evidence, conformational coverage, experimental support and
  the concrete TopoMT pocket contract and molecular/ensemble input contracts.
- Allocation: cryptic-pocket detection belongs to TopoMT; ensemble sources may
  include LandscapeMT. AlloMT owns the allosteric relevance/coupling assessment.

## P02 — Contextual functional profiles beyond a binary label

- Related needs: N01, N08, N10, N12. Type: operational clarification.
- Functions in scope: predict/compare effects on affinity, activity, pathway or
  partner preference; represent neutral/unsupported outcomes, probe conditions
  and uncertainty; fit appropriate dose/response or cooperativity models when data exist.
- Where applicable, separate intrinsic allosteric agonism from modulation of
  another ligand's effect, alongside the pathway-specific profile.
- Motivation: distinct functional profiles in [T03](RESEARCH_LANDSCAPE.md#t03--functional-profiles-and-pathway-selective-modulation).
- Open: requested endpoints, reference state, evidence threshold and the
  distinction between increased affinity and the intended functional benefit.
- Allocation: AlloMT owns allosteric profiles/interpretation; BindingMT supplies
  binding-specific endpoints and other providers supply their qualified observations.

## P03 — Quantitative energetic and kinetic coupling

- Related needs: N02, N05, N08, N09, N12. Type: extension of quantification.
- Functions in scope: construct explicit state/occupancy comparisons, estimate
  model-defined coupling free energies, compare multi-site cooperativity and
  investigate changes in populations, barriers or residence/transition times
  when the inputs and methods support those quantities.
- Motivation: thermodynamic linkage/landscapes, state models and quantitative
  bitopic design ([methods](METHODS_AND_TOOLS.md), [T05](RESEARCH_LANDSCAPE.md#t05--quantitative-design-of-bitopic-ligands)).
- Open: estimands, assumptions and suitable measured/simulated data; a graph
  score, docking score and functional coupling energy are not interchangeable.
- Allocation: binding-energy estimation/calculation belongs to BindingMT;
  general FEL/state/kinetic analysis is coordinated with LandscapeMT. AlloMT
  frames and interprets the allosteric coupling/comparison using those results.

## P04 — Epistasis, rescue and resistance-aware mutation design

- Related needs: N08, N12, N13. Type: extension.
- Functions in scope: distinguish folding/stability and functional mutation
  effects; analyze combinations/double-mutant couplings; propose suppressor/rescue
  mutations or resistance hypotheses for a declared mechanism.
- Motivation: energetic mutational maps and interpretable DMS inference
  ([T02](RESEARCH_LANDSCAPE.md#t02--experimental-energetic-maps-and-interpretable-learning)).
- Open: mutation space, mechanism/phenotype definitions, available data and
  biological constraints. Larger coupling is not automatically an improvement.
- Allocation: AlloMT owns allosteric mutation analysis and design questions;
  generic molecular changes, mechanical, binding and landscape operations stay
  with MolSysMT, ElastNetMT, BindingMT and LandscapeMT as appropriate.

## P05 — Selectivity and developability as explicit design objectives

- Related needs: N09, N10, N11. Type: broadening toward pharmacological potential.
- Functions in scope: compare target/isoform/homolog and conformational
  selectivity; carry chemical-quality, solubility, exposure/permeability and
  assay-interference constraints alongside the desired allosteric response.
- Motivation: the linked-ligand selectivity question in [T05](RESEARCH_LANDSCAPE.md#t05--quantitative-design-of-bitopic-ligands)
  and endpoint limits of generated compounds in [T07](RESEARCH_LANDSCAPE.md#t07--generative-molecular-design-and-task-specific-validation).
- Open: modality-specific criteria and actual provider capabilities. Generic
  pharmacophore/binding/peptide work retains its owners; ViableMT is conceptual
  in the reviewed ecosystem, not a usable ADMET API promised by this proposal.
- Allocation: AlloMT defines allosteric design criteria and comparisons; generic
  screening/design/developability calculations remain with their scientific owners.

## P06 — Choose informative next experiments under a budget

- Related needs: N05, N06, N13. Type: accepted research direction.
- Functions in scope: rank additional simulations, mutations or ligand tests
  by expected information gain and cost; suggest measurements that discriminate
  competing mechanisms, potentially including NMR, HDX, FRET or binding/activity data.
- Motivation: a design inference from the need to compare hypotheses and the
  complementary measurements/models surveyed; no universal active-learning
  algorithm is validated by this review.
- Open: decision utility, costs, feedback data, wet-lab collaboration and host
  orchestration. AlloMT could supply an allostery-specific proposal; execution
  and platform/project management keep their existing owners.
- Allocation: generic sampling/conformational exploration is coordinated with
  LandscapeMT and its execution providers; allostery-specific study utility and
  hypotheses remain AlloMT responsibilities.

## P07 — Calibrated comparisons and a scientific validation workbench

- Related needs: N01, N02, N04, N06, N07. Type: explicit version of an earlier
  assistant proposal to contrast hypotheses with computational/experimental references.
- Functions in scope: curate task-specific benchmark cases and negative/neutral
  evidence; compare methods on controlled inputs/costs; estimate uncertainty,
  calibration, robustness and out-of-domain behavior; preserve experimental
  provenance and failure/unsupported outcomes.
- Motivation: the independent model and energetic-map studies
  ([T02](RESEARCH_LANDSCAPE.md#t02--experimental-energetic-maps-and-interpretable-learning),
  [T07](RESEARCH_LANDSCAPE.md#t07--generative-molecular-design-and-task-specific-validation)).
- Open: benchmark governance, target/family/scaffold/temporal splits and evidence
  quality. Missing annotations must not silently become negative examples.
- Allocation: AlloMT owns allostery-task comparisons/validation; provider results,
  generic developer tooling and scientific knowledge retain their owners.

## P08 — Dynamic and condition-dependent mechanisms

- Related needs: N02, N05, N08, N10. Type: extension/clarification.
- Functions in scope: distinguish mean structural change from altered disorder,
  fluctuations, states and function; study how declared protonation, ligand,
  ion, solvent, membrane or modification conditions affect a hypothesis.
- Motivation: dynamic/disorder methods and engineered allosteric switches
  ([T04](RESEARCH_LANDSCAPE.md#t04--engineered-allostery-and-dynamicentropic-mechanisms)).
- Open: which environmental/modification contexts matter first, available inputs
  and the evidence needed to separate effects. No universal mechanism is assumed.
- Allocation: compose qualified molecular, ENM, landscape and sampling operations;
  develop allostery-specific analyses and interpretations in AlloMT.

## P09 — Additional intervention types and association mechanisms

- Related needs: N03, N09, N11, N12. Type: accepted broadening.
- Functions in scope: evaluate covalent versus reversible interventions and
  suitably qualified peptide/macrocycle or association-stabilizing strategies;
  distinguish direct interface engagement from distal allosteric modulation.
- Motivation: covalent discovery examples in [T06](RESEARCH_LANDSCAPE.md#t06--covalent-and-experimentally-exposed-cryptic-sites)
  and the researcher's explicit complex/peptide goals. Molecular-glue-like
  stabilization is an adjacent possibility, not automatically an allosteric mechanism.
- Open: desired modalities, reactive/adduct states, partner contexts and
  concrete provider contracts. These are not implementations or selected campaigns.
- Allocation: modality-specific peptide/binding/design operations keep their
  owners; AlloMT studies their allosteric consequences and design objectives.

## P10 — Generative research with explicit state and functional objectives

- Related needs: N06, N07, N09, N10, N11. Type: accepted workflow family.
- Functions in scope: generate candidate conformations or ligands under declared
  constraints, then assess their allosteric objectives with separate physical,
  statistical and experimental criteria; compare native and external approaches.
- Motivation: [T01](RESEARCH_LANDSCAPE.md#t01--ensembles-and-cryptic-opportunities-beyond-a-single-structure)
  and [T07](RESEARCH_LANDSCAPE.md#t07--generative-molecular-design-and-task-specific-validation).
- Open: model/data rights, physical validity, functional oracles, training-data
  overlap and validation costs. Generated sample frequency or binding confidence
  must not be silently reinterpreted as calibrated free energy or modulation.
- Allocation: generic ensemble generation/inference is coordinated with LandscapeMT;
  binding/molecular generation uses its owning providers. AlloMT contributes
  allosteric scientific objectives, assessment and method development.

## Continuing broad objective exploration

Diego accepted all ten objectives and explicitly requested continued broad
exploration. The earlier suggestion to focus next on a narrow subset is superseded
by R03. Further scientific approaches and applications remain welcome. Precision
for a particular analysis does not require limiting AlloMT to that analysis or
adopting one universal model of allostery. Later implementation increments can
be bounded while the overall objectives stay broad and extensible.
