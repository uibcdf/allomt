# Design coverage audit

**Round:** R02. **Reviewed:** 2026-11-15. **Phase:** researcher-needs elicitation.
**Owner:** [AlloMT #3](https://github.com/uibcdf/allomt/issues/3).

## Finding

All thirteen explicit researcher needs were represented in N01–N13. No complete
need was omitted. The documents were not a complete specification, and several
scientific distinctions and earlier assistant proposals were too implicit.
This review improves their traceability without treating new ideas as agreements.

## Coverage of the researcher's original statement

| Need | Preserved request | R02 clarification or supporting work |
| --- | --- | --- |
| N01 | Protein target, Sabueso/active-site knowledge, candidate allosteric sites, positive/negative modulation | Separate a bindable pocket, functional coupling and a particular intervention's effect. See Q02 and P01–P03. |
| N02 | Known site, mechanism and atomic path where possible | Preserve conditional resolution and alternative routes; distinguish statistical networks from causal evidence. |
| N03 | Target-specific set of reported allosteric ligands via Sabueso and/or online resources | Distinguish reported evidence from predicted annotations, source coverage and missing information. |
| N04 | Successful predictions with fast, inexpensive methods, including elastic networks | Review PRS/ESSA and require task-specific accuracy/cost comparisons. No method selected. |
| N05 | Propose MD experiments and analyze mechanisms, including information theory | Add sampling/bias, kinetic versus equilibrium data and experiment-discrimination questions. |
| N06 | ML/AI for predicting allostery | Distinguish site prediction, ensemble generation, ligand generation, affinity and functional response tasks. |
| N07 | Permissive third-party tools initially; stronger native algorithms in the near future | Strengthen wording from a mere licensing preference to the requested selection criterion; inspect real licenses and notices. |
| N08 | Relate allosteric activity to orthosteric function/structure loss | Preserve that request while distinguishing activity, local structural change, dynamics and global destabilization. |
| N09 | Bifunctional ortho-allo molecules | Add joint engagement, linker geometry/entropy, cooperativity and comparison with unlinked components as design questions. |
| N10 | Conformation-selective ligands with specific allosteric effects | Separate binding selectivity, population preference and the functional effect on each state. |
| N11 | Ecosystem workflows with PharmacophoreMT, BindingMT and PeptideMT | Preserve the named collaborations, scientific handoffs and provider ownership. |
| N12 | Modulate complex/multimer formation, including associations involving DNA/RNA | Preserve the broad system scope and clarify identifying versus engineering regions and association observables. |
| N13 | Mutations that improve/worsen a known mechanism | Correct the heading's narrower strengthen/weaken wording; improvement is not defined as a larger coupling score. |

The current inventory remains [RESEARCHER_NEEDS.md](RESEARCHER_NEEDS.md).
Need order continues to reflect the original statement, not an agreed priority.

## Earlier assistant proposals and interpretations

| Earlier idea | Coverage before review | R02 treatment |
| --- | --- | --- |
| Prediction, characterization and contrast of hypotheses against computational/experimental references | Prediction/characterization were prominent; contrast was scattered across scope obligations and Q07. | Recovered explicitly as interpretation I07 and proposal P07. It was not an additional researcher-stated need. |
| Public scientific operations, method implementations and traceable results as conceptual views | Partly implied by I03/I05 and the architecture notes. | Recovered explicitly as I06, remaining provisional rather than an agreed package layout. |
| Systems/assemblies, functional reference, independent entry points, alternative paths, backend independence | Recorded as I01–I05. | Retained with their original unconfirmed status. |
| Molecular maps, units, provenance, uncertainty and separation of results/diagnostics/citations | Recorded in scientific scope and canonical guidance. | Retained as applicable scientific/engineering obligations, not invented product features. |
| Independent use, offline/supplied knowledge and optional agent hosting | Present in Q03 and architecture notes. | Retained; the illustrative workflow must not imply mandatory network access. |

## Scientific distinctions made more explicit

1. **Pocket, coupling and effect:** allosteric regions need not all be cavities.
   Geometry/accessibility, communication with a
   functional reference, and a ligand/mutation's measured or predicted effect
   are different questions. A mechanical-response score alone does not define
   PAM/NAM pharmacology. This is a design inference from the output meanings in
   [PRS/ESSA](METHODS_AND_TOOLS.md) and the context-dependent effects in
   [S10](RESEARCH_REFERENCES.md#s10).
2. **Function and structure:** N08 does not require every allosteric effect to
   destroy orthosteric structure. Structural disorder and functional/stability
   separation need explicit consideration; see [S05](RESEARCH_REFERENCES.md#s05),
   [S20](RESEARCH_REFERENCES.md#s20) and [S22](RESEARCH_REFERENCES.md#s22).
3. **Resolution and interpretation:** a network path is a method-conditioned
   hypothesis. Atomic detail, alternative routes, directionality and causal
   interpretations require the corresponding inputs and evidence.
4. **Sampling semantics:** independent generated structures, biased MD,
   equilibrium estimates and time-lagged propagation are distinct inputs.
   Their valid thermodynamic/kinetic interpretations must be assessed separately.
5. **Licensing scope:** root MIT metadata does not settle bundled code/data,
   checkpoints or service permissions. The BioEmu2 notices are a concrete example.

These distinctions clarify scientific meaning; they do not select an algorithm,
public API or final result class.

## New possibilities, not newly agreed requirements

[PROPOSED_EXTENSIONS.md](PROPOSED_EXTENSIONS.md) records P01–P10 with motivation,
possible functions, related needs, evidence and unresolved scope. They include
cryptic pockets, richer functional profiles, quantitative coupling, epistasis,
selectivity/developability, active learning, calibrated validation, dynamic
allostery, other intervention types and generative research workflows.

[METHODS_AND_TOOLS.md](METHODS_AND_TOOLS.md) compares established approaches and
fourteen source-level tool profiles. [RESEARCH_LANDSCAPE.md](RESEARCH_LANDSCAPE.md)
reviews recent work through 2026-11-15. Scientific relevance, license suitability
and a working installation are kept separate; no backend was adopted or tested.

## Remaining incompleteness

Representative systems, use-case priorities, success metrics, experimental
comparisons, resource budgets and acceptable uncertainty remain to be negotiated.
The public API and source layout remain open. Documentary coverage of the stated
needs is complete at this round; product specification and scientific feasibility
are not declared complete. Findings from this review can be revised in later rounds.
