# Open design questions

**Status:** all questions below are open after discussion round R01.
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

## Q04 — Mechanisms, paths and resolution

Related needs: N02, N05, N08.

What should a characterized mechanism contain beyond a path visualization?
Should the product report individual paths, alternative routes, networks,
conformational transitions or combinations? What qualifies atomic detail, and
what should be returned from residue-level or coarse-grained inputs? What
evidence is needed for directional/causal interpretations and uncertainty?

## Q05 — Accuracy, cost and rapid screening

Related needs: N01, N04, N07.

What makes a site prediction successful, and against which references? What
computational budgets, hardware, runtimes and input requirements are acceptable?
How should speed/accuracy tradeoffs, candidate rankings and escalation to more
expensive analyses be evaluated? No numerical method is selected by this question.

## Q06 — Simulation experiments and their analysis

Related needs: N02, N05, N08, N10, N12.

What should an MD experiment proposal deliver: hypotheses, system preparation
requirements, controls/comparisons, sampling/replica plans, observables and
analysis/uncertainty criteria? Which information-theory questions matter first?
Who would execute simulations and how would that integrate with the ecosystem?
How should results distinguish functional changes, local structural changes and
global effects? The current request establishes planning and analysis needs;
simulation execution is a separate topic to negotiate.

## Q07 — Third-party methods, native research and ML

Related needs: N04, N06, N07.

Which initial methods/models fit the desired tasks and permissive licensing?
How should code, model weights, data and online-service permissions be assessed
for actual intended use? Are pretrained inference, model training and fine-tuning
all desired? What tasks, reference datasets, generalization tests, uncertainty
and cost comparisons would establish that our native algorithms improve on the
adopted baselines? How should native and third-party routes coexist or evolve?

## Q08 — Molecular design and conformational selectivity

Related needs: N09, N10, N11.

What should AlloMT contribute to ligand, pharmacophore, peptide and bifunctional
design, and what should the existing scientific components supply? What objects
and scientific requirements pass between them? For ortho-allo molecules, how
should simultaneous engagement, linker geometry and the desired effect be
evaluated? What defines the target and competing conformations for selectivity?

## Q09 — Assembly modulation and mutation design

Related needs: N08, N12, N13.

Does designing an allosteric region mean identifying a region for a modulator,
engineering the region through mutations, or both? Which association states and
measurements matter for protein complexes, multimers and DNA/RNA-containing
associations? Which mutations and contextual comparisons should be considered,
and what would count as strengthening or weakening the known mechanism?

## Q10 — Representative cases and priorities

Related needs: N01–N13.

Which concrete examples best express the researcher's needs? Which outputs make
them useful, and which success criteria would the researcher use? When enough
of the need is understood, which bounded case should become the first scientific
increment under [AlloMT #2](https://github.com/uibcdf/allomt/issues/2)?
The need inventory's ordering does not answer this priority question.
