# Methods and tools for discussion

**Reviewed:** 2026-11-15. **Status:** research/options, not selected integrations.
Primary references are in [the bibliography](RESEARCH_REFERENCES.md); immutable
license observations are in [the tool snapshot](research/tool_inventory_2026_11_15.json).
No tool/model was installed, executed, benchmarked or qualified for AlloMT here.

Here, ligandability concerns a site's suitability for ligand engagement;
functional coupling and pharmacological effect require additional definitions.
PAM/NAM mean positive/negative allosteric modulation relative to a declared
functional context. Neither is assigned merely from a cavity or network score.
These distinctions motivate the review rather than selecting a result schema.

## Established method families

| Method family | Useful inputs and outputs | Interpretation/validation needed | References |
| --- | --- | --- | --- |
| MWC/KNF and related state/occupancy models | Functional/binding measurements interpreted with explicit state and interaction assumptions | Model fit and identifiable parameters; alternative mechanisms may fit limited observations. | [S25](RESEARCH_REFERENCES.md#s25), [S26](RESEARCH_REFERENCES.md#s26) |
| GNM/ANM and normal-mode covariance | Structure-derived collective motions and susceptibility hypotheses; coordinate numerical work with ElastNetMT | Resolution, normalization, null modes and units; mode amplitudes do not themselves specify functional activation. | [S01](RESEARCH_REFERENCES.md#s01), [S02](RESEARCH_REFERENCES.md#s02) |
| Perturbation response scanning (PRS) | Covariance-based response maps, sensitivity and effectiveness profiles | Perturbation/reference definitions and normalization; response magnitude is not a PAM/NAM label. | [S01](RESEARCH_REFERENCES.md#s01), [S03](RESEARCH_REFERENCES.md#s03) |
| Essential site scanning analysis (ESSA) | Changes in global-mode spectra after local perturbation; possible site/pocket rankings | Distinguish mechanical importance, pocket geometry and ligand-specific functional effects. | [S02](RESEARCH_REFERENCES.md#s02) |
| Contact/correlation networks, communities and suboptimal paths | Structure/trajectory-dependent residue networks and alternative communication hypotheses | Edge definitions, mapping, sampling, contact filters and robustness; a graph path is not a measured signal trajectory. | [S03](RESEARCH_REFERENCES.md#s03), [S04](RESEARCH_REFERENCES.md#s04) |
| Mutual information, dihedral/disorder analysis and CARDS | Statistical coupling and structural/disorder contributions from sampled ensembles | Estimator bias, correlated sampling, state definitions and uncertainty; dependence is not automatically directional causation. | [S05](RESEARCH_REFERENCES.md#s05), [S08](RESEARCH_REFERENCES.md#s08) |
| Transfer entropy and conditional time-lagged analysis | Direction-sensitive statistical dependencies from time-resolved data | Lag, conditioning, finite samples and hidden variables; causal claims require additional assumptions/evidence. | [S28](RESEARCH_REFERENCES.md#s28) |
| State models, dimensional reduction and transition analysis | Metastable states, populations and kinetic hypotheses from suitable trajectories | Sampling coverage, lag/model validation and input time semantics. Arbitrary order of independent generated conformers is not an ordinary kinetic trajectory. | [S27](RESEARCH_REFERENCES.md#s27) |
| Enhanced sampling and free-energy analysis | Targeted exploration of states/barriers; metadynamics is one established option | Record bias, collective variables and valid estimators; biased sampling and unbiased kinetics require different treatment. Execution remains an open ownership/workflow question. | [S29](RESEARCH_REFERENCES.md#s29), [S08](RESEARCH_REFERENCES.md#s08) |
| Thermodynamic linkage/coupling and explicit state comparisons | Energetic coupling between defined events/states, using appropriate measurements or physical/inference models | State/condition definitions, uncertainty and reference cycles; docking scores are not a substitute for a measured/model-defined coupling free energy. | [S08](RESEARCH_REFERENCES.md#s08), [S11](RESEARCH_REFERENCES.md#s11) |
| Sequence coevolution/sectors (SCA) | Alignment-derived patterns suggesting functionally connected residues | Alignment quality, phylogeny and experimental checks; conserved covariation alone does not identify an atomic causal route. | [S06](RESEARCH_REFERENCES.md#s06) |
| DMS and interpretable biophysical inference | Fit folding/binding/coupling effects from mutational/phenotypic data | Requires suitable measurements and a specified model; it is distinct from sequence-only prediction of an unseen system. | [S11](RESEARCH_REFERENCES.md#s11), [S19](RESEARCH_REFERENCES.md#s19) |
| Site ML/ranking and complementary geometric analysis | Candidate pockets/residues with method-specific rankings; PASSer2.0 is a possible historical baseline | Training/test separation, known-site bias, calibration and target generalization. Pocket rank is not a functional response probability. | [PASSer official site](https://passer.smu.edu/), [source snapshot](research/tool_inventory_2026_11_15.json) |

The MWC/KNF papers are historical theoretical foundations, not a requirement that
AlloMT force every mechanism into a two-state/concerted model. The PyEMMA paper
documents a method family; its software was not license-screened or selected in
this fourteen-tool inventory.

## Tool/license screening

The table refers to the exact repositories/revisions in the snapshot, not to
every implementation of a named algorithm. A permissive core license is an
initial filter, not completed review of dependencies, model/data rights or a
working public installation route. The requested permissive criterion excludes
the identified GPL implementations from the initial default integration shortlist;
they remain useful scientific references. No conclusion about a different
implementation or a specially negotiated future route is implied.

| Tool/repository | Scientific role | Observed license/status | Current disposition |
| --- | --- | --- | --- |
| [ProDy](https://github.com/prody/ProDy) | PRS, ESSA and normal-mode reference | MIT for ProDy core; composite bundled notices explain GitHub's `NOASSERTION` metadata | Candidate for method comparison; reuse/coordinate ENM ownership, with selected-route qualification pending. |
| [PASSer2.0](https://github.com/smu-tao-group/PASSer2.0) | Automated-ML allosteric-site baseline | MIT in this repository | Candidate; model/data/pocket-feature and runtime review pending. This does not license every PASSer service/version. |
| [MoCHI](https://github.com/lehner-lab/MoCHI) | Interpretable DMS/energetic inference | MIT | Candidate for data-rich mutation studies and benchmarking, not a replacement for missing experimental inputs. |
| [pySCA](https://github.com/ranganathanlab/pySCA) | Coevolution/sectors | BSD-3-Clause | Candidate comparative route; biological alignment and generalization controls remain necessary. |
| [WISP](https://github.com/durrantlab/wisp) | Alternative/suboptimal graph paths | AFL-3.0 in `LICENSE.md` | Additional terms/route review; not silently treated as an MIT/BSD dependency. |
| [MD-TASK](https://github.com/RUBi-ZA/MD-TASK) | Networks, PRS and cross-correlation | GPL-3.0 | Outside initial permissive integration filter; methods/reference only at this stage. |
| [AlloViz](https://github.com/frannerin/AlloViz) | Comparative network/delta-network wrapper | GPL-3.0; multiple underlying packages | Outside initial permissive filter; wrapper adoption would also need underlying-route review. |
| [PyInteraph2](https://github.com/ELELAB/pyinteraph2) | Ensemble interaction networks | GPL-3.0-or-later in the actual notice, despite `NOASSERTION` metadata | Outside initial permissive filter. |
| [enspara/CARDS implementation](https://github.com/bowman-lab/enspara) | Structural/disorder information analysis | GPL-3.0 | Outside initial permissive filter. The mathematical CARDS method is not itself labeled by this software license observation. |
| [AlphaFlow](https://github.com/bjing2016/alphaflow) | Generative protein ensembles | MIT code; checkpoint/closure unqualified here | Research candidate with domain-specific ensemble validation. |
| [BioEmu](https://github.com/microsoft/bioemu) | Monomer-ensemble reference | MIT core/model; repository archived and README points to BioEmu2 | Historical/comparative reference; do not present it as the current maintained route. |
| [BioEmu2](https://github.com/microsoft/bioemu2) | All-atom ensembles and separate learned propagation mode | MIT core/model; `NOTICES.md` identifies LGPL patches/data and geostd notices | Hold default adoption pending full route/asset review. Model-card calibration limits also matter scientifically. |
| [Boltz-2 repository](https://github.com/jwohlwend/boltz) | Complex/affinity hypotheses | MIT code and weights according to the upstream README | Coordinate relevant binding/complex operations with BindingMT; affinity/pose predictions do not establish an allosteric functional effect. |
| [DiffSBDD](https://github.com/arneschneuing/DiffSBDD) | Pocket-conditioned molecular generation | MIT code; checkpoint/data route not qualified | Optional design research with the owning molecular-design components; generated ligands need chemical and functional evaluation. |

The machine-readable snapshot supplies commit, license path/blob, observed
classification and archived state for each row. BioEmu2's precise bundled
notices are linked under [S14](RESEARCH_REFERENCES.md#s14). No Python 3.14,
platform, packaging, model accuracy or installed compatibility is certified here.

AlloSigMA 2 is an additional service/method reference for model-derived energetic
responses to ligand/mutation perturbations [S07](RESEARCH_REFERENCES.md#s07).
An accessible server does not establish a permissively licensed redistributable
backend or an admitted API/service route; those terms were not established here.

## Knowledge and practical composition

ASD2023, published in the 2024 journal issue, includes allosteric resources
covering PPI and dual-steric contexts [S09](RESEARCH_REFERENCES.md#s09). It is
a relevant provider-side resource to investigate with Sabueso. Resource names,
predicted pocket annotations and reported experimental modulators must retain
their actual evidence categories. Bulk/API availability and use rights remain
separate questions; this review does not establish a complete target ligand set.

A useful candidate experiment for later negotiation is to compare a fast
ElastNetMT-compatible perturbation analysis with one externally described
baseline, then evaluate site recovery, functional relevance, uncertainty and
cost on declared cases. Pocket generation/geometry would use its scientific
owner. This is a proposal, not the selected first AlloMT workflow.

Native-method development should compare like-for-like questions, input budgets,
splits and observables. Preserve method-specific outputs and named backends;
agreement among heterogeneous scores is not automatically calibrated confidence.
