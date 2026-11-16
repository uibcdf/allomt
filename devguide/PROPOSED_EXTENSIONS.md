# Proposed objectives and functions

**Round:** R02, 2026-11-15. **Status of every P item:** proposed, not agreed.
These possibilities respond to the request to identify overlooked objectives.
Some make an existing need operational; others broaden the product. They do not
replace [N01–N13](RESEARCHER_NEEDS.md) or establish an implementation order.

Evidence and reasoning are linked through [the research landscape](RESEARCH_LANDSCAPE.md)
and [methods/tools](METHODS_AND_TOOLS.md). Scientific interpretations and proposed
software functions remain distinguished from demonstrated upstream results.

## P01 — Cryptic pockets and separate site assessments

- Related needs: N01, N04, N10. Type: extension/clarification.
- Possible functions: detect intermittent/hidden pockets across supplied or
  generated conformations; assess their accessibility, ligandability and
  coupling to a functional region separately; compare state-dependent opportunities.
- Motivation: ensemble generation and experimental pocket mapping offer
  complementary inputs ([T01](RESEARCH_LANDSCAPE.md#t01--ensembles-and-cryptic-opportunities-beyond-a-single-structure),
  [T06](RESEARCH_LANDSCAPE.md#t06--covalent-and-experimentally-exposed-cryptic-sites)).
- Open: pocket evidence, conformational coverage, experimental support and which
  geometry operations are supplied by TopoMT/MolSysMT.

## P02 — Contextual functional profiles beyond a binary label

- Related needs: N01, N08, N10, N12. Type: operational clarification.
- Possible functions: predict/compare effects on affinity, activity, pathway or
  partner preference; represent neutral/unsupported outcomes, probe conditions
  and uncertainty; fit appropriate dose/response or cooperativity models when data exist.
- Where applicable, separate intrinsic allosteric agonism from modulation of
  another ligand's effect, alongside the pathway-specific profile.
- Motivation: distinct functional profiles in [T03](RESEARCH_LANDSCAPE.md#t03--functional-profiles-and-pathway-selective-modulation).
- Open: requested endpoints, reference state, evidence threshold and the
  distinction between increased affinity and the intended functional benefit.

## P03 — Quantitative energetic and kinetic coupling

- Related needs: N02, N05, N08, N09, N12. Type: extension of quantification.
- Possible functions: construct explicit state/occupancy comparisons, estimate
  model-defined coupling free energies, compare multi-site cooperativity and
  investigate changes in populations, barriers or residence/transition times
  when the inputs and methods support those quantities.
- Motivation: thermodynamic linkage/landscapes, state models and quantitative
  bitopic design ([methods](METHODS_AND_TOOLS.md), [T05](RESEARCH_LANDSCAPE.md#t05--quantitative-design-of-bitopic-ligands)).
- Open: estimands, assumptions and suitable measured/simulated data; a graph
  score, docking score and functional coupling energy are not interchangeable.

## P04 — Epistasis, rescue and resistance-aware mutation design

- Related needs: N08, N12, N13. Type: extension.
- Possible functions: distinguish folding/stability and functional mutation
  effects; analyze combinations/double-mutant couplings; propose suppressor/rescue
  mutations or resistance hypotheses for a declared mechanism.
- Motivation: energetic mutational maps and interpretable DMS inference
  ([T02](RESEARCH_LANDSCAPE.md#t02--experimental-energetic-maps-and-interpretable-learning)).
- Open: mutation space, mechanism/phenotype definitions, available data and
  biological constraints. Larger coupling is not automatically an improvement.

## P05 — Selectivity and developability as explicit design objectives

- Related needs: N09, N10, N11. Type: broadening toward pharmacological potential.
- Possible functions: compare target/isoform/homolog and conformational
  selectivity; carry chemical-quality, solubility, exposure/permeability and
  assay-interference constraints alongside the desired allosteric response.
- Motivation: the linked-ligand selectivity question in [T05](RESEARCH_LANDSCAPE.md#t05--quantitative-design-of-bitopic-ligands)
  and endpoint limits of generated compounds in [T07](RESEARCH_LANDSCAPE.md#t07--generative-molecular-design-and-task-specific-validation).
- Open: modality-specific criteria and actual provider capabilities. Generic
  pharmacophore/binding/peptide work retains its owners; ViableMT is conceptual
  in the reviewed ecosystem, not a usable ADMET API promised by this proposal.

## P06 — Choose informative next experiments under a budget

- Related needs: N05, N06, N13. Type: proposed research direction.
- Possible functions: rank additional simulations, mutations or ligand tests
  by expected information gain and cost; suggest measurements that discriminate
  competing mechanisms, potentially including NMR, HDX, FRET or binding/activity data.
- Motivation: a design inference from the need to compare hypotheses and the
  complementary measurements/models surveyed; no universal active-learning
  algorithm is validated by this review.
- Open: decision utility, costs, feedback data, wet-lab collaboration and host
  orchestration. AlloMT could supply an allostery-specific proposal; execution
  and platform/project management keep their existing owners.

## P07 — Calibrated comparisons and a scientific validation workbench

- Related needs: N01, N02, N04, N06, N07. Type: explicit version of an earlier
  assistant proposal to contrast hypotheses with computational/experimental references.
- Possible functions: curate task-specific benchmark cases and negative/neutral
  evidence; compare methods on controlled inputs/costs; estimate uncertainty,
  calibration, robustness and out-of-domain behavior; preserve experimental
  provenance and failure/unsupported outcomes.
- Motivation: the independent model and energetic-map studies
  ([T02](RESEARCH_LANDSCAPE.md#t02--experimental-energetic-maps-and-interpretable-learning),
  [T07](RESEARCH_LANDSCAPE.md#t07--generative-molecular-design-and-task-specific-validation)).
- Open: benchmark governance, target/family/scaffold/temporal splits and evidence
  quality. Missing annotations must not silently become negative examples.

## P08 — Dynamic and condition-dependent mechanisms

- Related needs: N02, N05, N08, N10. Type: extension/clarification.
- Possible functions: distinguish mean structural change from altered disorder,
  fluctuations, states and function; study how declared protonation, ligand,
  ion, solvent, membrane or modification conditions affect a hypothesis.
- Motivation: dynamic/disorder methods and engineered allosteric switches
  ([T04](RESEARCH_LANDSCAPE.md#t04--engineered-allostery-and-dynamicentropic-mechanisms)).
- Open: which environmental/modification contexts matter first, available inputs
  and the evidence needed to separate effects. No universal mechanism is assumed.

## P09 — Additional intervention types and association mechanisms

- Related needs: N03, N09, N11, N12. Type: optional broadening.
- Possible functions: evaluate covalent versus reversible interventions and
  suitably qualified peptide/macrocycle or association-stabilizing strategies;
  distinguish direct interface engagement from distal allosteric modulation.
- Motivation: covalent discovery examples in [T06](RESEARCH_LANDSCAPE.md#t06--covalent-and-experimentally-exposed-cryptic-sites)
  and the researcher's explicit complex/peptide goals. Molecular-glue-like
  stabilization is an adjacent possibility, not automatically an allosteric mechanism.
- Open: desired modalities, reactive/adduct states, partner contexts and
  concrete provider contracts. These are not implementations or selected campaigns.

## P10 — Generative research with explicit state and functional objectives

- Related needs: N06, N07, N09, N10, N11. Type: proposed workflow specialization.
- Possible functions: generate candidate conformations or ligands under declared
  constraints, then assess their allosteric objectives with separate physical,
  statistical and experimental criteria; compare native and external approaches.
- Motivation: [T01](RESEARCH_LANDSCAPE.md#t01--ensembles-and-cryptic-opportunities-beyond-a-single-structure)
  and [T07](RESEARCH_LANDSCAPE.md#t07--generative-molecular-design-and-task-specific-validation).
- Open: model/data rights, physical validity, functional oracles, training-data
  overlap and validation costs. Generated sample frequency or binding confidence
  must not be silently reinterpreted as calibrated free energy or modulation.

## Suggested topics for the next negotiations

The assistant recommends discussing P01–P03 first as scientific distinctions
that affect the interpretation of N01, and P07 as a way to evaluate future native
improvements. P04–P06 are useful extensions for mutation/design/experiment goals.
This is an order for discussion, not an agreed delivery priority or MVP selection.
All ten proposals remain open to acceptance, revision, combination or rejection.
