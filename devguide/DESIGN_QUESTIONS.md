# Open design questions

**Status:** all questions below remain open after discussion round R02.
Q01–Q10 originate in R01 and are refined here; Q11/Q12 are added by the review.
They organize future conversations; they are not a questionnaire that must be
answered at once or a selected architecture. See [the needs](RESEARCHER_NEEDS.md)
and [the discussion history](DESIGN_DISCUSSION.md).

## Q01 — Target inputs and scientific context

Related needs: N01, N02, N03, N10, N12.

What may the researcher supply initially: a target identifier, sequence,
structure/model, prepared assembly, ensemble or existing trajectories? How are
relevant conformations, partners, biological assembly, conditions and known
functional regions established? Which cases need to work with incomplete knowledge?

## Q02 — Functional reference and modulation direction

Related needs: N01, N08, N10, N12, N13.

What does positive or negative modulation mean for each requested workflow:
catalytic activity, orthosteric binding, another functional response, stability,
state preference or molecular association? What is the reference intervention,
ligand/state and comparison? How should unknown/unsupported outcomes and
uncertainty be presented? How is orthosteric structural change measured alongside
functional change and broader stability?

Should the outputs distinguish affinity, efficacy, pathway/partner bias and
kinetics, including intrinsic allosteric agonism where applicable? Which labels
describe a supported neutral result versus insufficient
evidence? How should site geometry and mechanical susceptibility be kept distinct
from intervention-specific pharmacology? See proposals P01–P03.

As scientific motivation, a primary study of LY2033298 at muscarinic receptors
reported different modulation signs depending on the orthosteric probe and
measured pathway, and differences between affinity and signaling effects.
This motivates retaining context in the discussion; it is not an AlloMT method
or a prediction validated for other target classes.
[Valant et al., Molecular Pharmacology (2012)](https://pubmed.ncbi.nlm.nih.gov/21989256/).

## Q03 — Knowledge retrieval and reported modulators

Related needs: N01, N03, N11.

Which knowledge should AlloMT request from Sabueso, and which direct data-source
access, if any, should be maintained elsewhere or locally? How should reported
ligands, sites, evidence, conditions, target/sequence numbering and conflicting
claims be represented? What constitutes useful coverage of the reported ligand
set? What must work with supplied/offline knowledge?

How should predicted pocket/resource annotations remain separate from reported
experimental modulators, including negative or conflicting results? What source
coverage is actually known for each retrieval?

## Q04 — Mechanisms, paths and resolution

Related needs: N02, N05, N08.

What should a characterized mechanism contain beyond a path visualization?
Should the product report individual paths, alternative routes, networks,
conformational transitions or combinations? What qualifies atomic detail, and
what should be returned from residue-level or coarse-grained inputs? What
evidence is needed for directional/causal interpretations and uncertainty?

How should path/network stability be assessed across replicas, alternative
estimators, resolutions and functional states? What intervention would help
discriminate a proposed communication mechanism from a correlation pattern?

## Q05 — Accuracy, cost and rapid screening

Related needs: N01, N04, N07.

What makes a site prediction successful, and against which references? What
computational budgets, hardware, runtimes and input requirements are acceptable?
How should speed/accuracy tradeoffs, candidate rankings and escalation to more
expensive analyses be evaluated? No numerical method is selected by this question.

Would PRS/ESSA-like baselines be informative on the selected cases, and how should
their outputs be compared with site ML and more expensive physical analyses?

## Q06 — Simulation experiments and their analysis

Related needs: N02, N05, N08, N10, N12.

What should an MD experiment proposal deliver: hypotheses, system preparation
requirements, controls/comparisons, sampling/replica plans, observables and
analysis/uncertainty criteria? Which information-theory questions matter first?
Who would execute simulations and how would that integrate with the ecosystem?
How should results distinguish functional changes, local structural changes and
global effects? The current request establishes planning and analysis needs;
simulation execution is a separate topic to negotiate.

What analysis is valid for biased versus unbiased trajectories, independent
generated conformers and learned time-lagged propagation? Which experiments
would most reduce uncertainty for a given budget, and which complementary
measurements would test the mechanism (P03, P06, P08, P10)?

## Q07 — Third-party methods, native research and ML

Related needs: N04, N06, N07.

Which initial methods/models fit the desired tasks and permissive licensing?
How should code, model weights, data and online-service permissions be assessed
for actual intended use? Are pretrained inference, model training and fine-tuning
all desired? What tasks, reference datasets, generalization tests, uncertainty
and cost comparisons would establish that our native algorithms improve on the
adopted baselines? How should native and third-party routes coexist or evolve?

How should mixed bundled notices, model/checkpoint terms and dataset/service
rights be evaluated against the requested permissive criterion? The reviewed
BioEmu2 notices illustrate why the core license alone is insufficient. No
external route is selected by the [tool screening](METHODS_AND_TOOLS.md).

## Q08 — Molecular design and conformational selectivity

Related needs: N09, N10, N11.

What should AlloMT contribute to ligand, pharmacophore, peptide and bifunctional
design, and what should the existing scientific components supply? What objects
and scientific requirements pass between them? For ortho-allo molecules, how
should simultaneous engagement, linker geometry and the desired effect be
evaluated? What defines the target and competing conformations for selectivity?

How should joint engagement, linker entropy/cooperativity, off-target selectivity
and modality-specific developability be balanced? Which of those quantities
can actually be evaluated by the available providers (P03, P05, P09, P10)?

## Q09 — Assembly modulation and mutation design

Related needs: N08, N12, N13.

Does designing an allosteric region mean identifying a region for a modulator,
engineering the region through mutations, or both? Which association states and
measurements matter for protein complexes, multimers and DNA/RNA-containing
associations? Which mutations and contextual comparisons should be considered,
and what would count as strengthening or weakening the known mechanism?

Does improving a mechanism mean changing its magnitude, desired activity,
specificity or another endpoint? Are epistasis, suppressor/rescue mutations and
resistance forecasts useful extensions, with folding/stability controls (P04)?

## Q10 — Representative cases and priorities

Related needs: N01–N13.

Which concrete examples best express the researcher's needs? Which outputs make
them useful, and which success criteria would the researcher use? When enough
of the need is understood, which bounded case should become the first scientific
increment under [AlloMT #2](https://github.com/uibcdf/allomt/issues/2)?
The need inventory's ordering does not answer this priority question.

## Q11 — Evidence, uncertainty and native-method evaluation

Related needs: N01, N02, N04, N06, N07; proposal P07.

Which reference measurements and negative/neutral cases define success for each
task? How should target/family, ligand-scaffold and temporal separation limit
training/test overlap? What calibration, robustness, out-of-domain and cost
criteria should support comparisons and the goal of improving native methods?
How should unresolved, failed and contradictory results be presented?

## Q12 — Scope of the proposed extensions

Related needs: N01–N13; proposals P01–P10.

Which proposals should become product objectives, scientific research directions,
optional collaborations or out-of-scope ideas? Which merely clarify an existing
need? What concrete cases would make each useful? None is accepted by appearing
in [the proposal register](PROPOSED_EXTENSIONS.md).
