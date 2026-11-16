# Recent research landscape

**Cutoff reviewed:** 2026-11-15. **Purpose:** inform requirements discussion,
not declare selected algorithms or a complete systematic review. The scope,
primary sources and publication types are recorded in
[RESEARCH_REFERENCES.md](RESEARCH_REFERENCES.md).

The established foundations are compared in [METHODS_AND_TOOLS.md](METHODS_AND_TOOLS.md).
The possibilities inferred for AlloMT remain proposals in
[PROPOSED_EXTENSIONS.md](PROPOSED_EXTENSIONS.md).

## T01 — Ensembles and cryptic opportunities beyond a single structure

AlphaFlow (ICML 2024) learns structural ensembles, and BioEmu (Science 2025)
emulates selected equilibrium-ensemble properties. These developments motivate
testing conformationally intermittent pockets and state-specific accessibility,
with validation on the intended target/domain rather than assuming a static
structure contains every useful site.
[S12](RESEARCH_REFERENCES.md#s12), [S13](RESEARCH_REFERENCES.md#s13).

The current BioEmu2 release adds documented support for complexes, ligands and
nucleic acids and a separate time-lagged propagation interface. Its model card
explicitly leaves ensemble frequencies uncalibrated for Boltzmann/free-energy
interpretation. Propagation outputs are lagged endpoints; the mere existence
of that API is not independent kinetic validation. The older BioEmu repository
is archived and points to this successor.
[S14](RESEARCH_REFERENCES.md#s14), [tool snapshot](research/tool_inventory_2026_11_15.json).

**Implication to discuss:** keep structures, ensemble weights and temporal
semantics distinct. Candidate-pocket discovery, ligandability and demonstrated
functional allostery need separate evaluations. This supports P01 and P10.

## T02 — Experimental energetic maps and interpretable learning

MoCHI (2024) fits specified biophysical models to DMS data, including energetic
couplings. The 2026 comparative PDZ study provides maps that separate folding
and binding effects and finds protein-specific allosteric mutations among
homologous domains. A separate 2026 study analyzes functional loss separately
from destabilization across several datasets.
[S11](RESEARCH_REFERENCES.md#s11), [S19](RESEARCH_REFERENCES.md#s19),
[S22](RESEARCH_REFERENCES.md#s22).

**Implication to discuss:** mutation design needs a declared functional endpoint
and stability controls. Family similarity alone is not a validated transfer
rule. Data-rich energetic inference and sequence/structure-only predictions
should retain their different input requirements and evidence (P04, P07).

## T03 — Functional profiles and pathway-selective modulation

The 2025 NTSR1 study designs allosteric compounds with distinct G-protein subtype
selectivity profiles by modifying a chemical scaffold. It illustrates a useful
functional objective richer than a single activation/inhibition label.
Earlier probe-dependence experiments also distinguish affinity and signaling
responses for a particular target/modulator context.
[S18](RESEARCH_REFERENCES.md#s18), [S10](RESEARCH_REFERENCES.md#s10).

**Implication to discuss:** represent an intended functional profile under
declared conditions, including the orthosteric probe, pathway/partner and
reference. This does not assume that every target behaves like a GPCR or that
all modulators necessarily have the same kind of probe dependence (P02).

## T04 — Engineered allostery and dynamic/entropic mechanisms

The 2026 artificial-switch study uses ML-designed ligand-binding receptors
without a global conformational change to construct functional allosteric
switches. It complements earlier CARDS work on structural/disorder contributions
to communication.
[S20](RESEARCH_REFERENCES.md#s20), [S05](RESEARCH_REFERENCES.md#s05).

**Implication to discuss:** changes in mean structure, fluctuations, ordering,
state populations and function should be distinguishable outputs. A workflow
focused only on orthosteric structural damage would cover only part of the
researcher's scope. Native protein/region engineering is a possible additional
direction, subject to negotiation (P04, P08).

## T05 — Quantitative design of bitopic ligands

The September 2026 ABL1/EGFR study systematically varies ligand choice, linkage
vector and linker length, relating performance to cooperativity and linker
entropy. It is a particularly direct reference for N09's ortho-allo objective.
[S21](RESEARCH_REFERENCES.md#s21).

**Implication to discuss:** evaluate the linked molecule's joint engagement,
conformational constraints, functional effect and selectivity alongside the
parent ligands and relevant unlinked comparisons. Two separately plausible poses
do not evaluate the complete design. AlloMT would contribute allosteric goals
and hypotheses while molecular-design/binding components retain their roles.

## T06 — Covalent and experimentally exposed cryptic sites

CysMAP (2026) combines cysteine scanning and covalent screening to discover
pockets in KRAS. The 2026 NLRP3 study reports a covalent inhibitor engaging an
allosteric pocket through a chemoproteomics-led approach.
[S23](RESEARCH_REFERENCES.md#s23), [S24](RESEARCH_REFERENCES.md#s24).

**Implication to discuss:** consider experimentally constrained accessibility,
reactive chemistry and adduct/target-state identity. A mapped pocket alone is
not evidence of functional coupling, and engineered probe accessibility must
not be silently equated with wild-type ligandability. Covalent workflows would
need their own qualified contracts, not an assumed noncovalent route (P01, P09).

## T07 — Generative molecular design and task-specific validation

DiffSBDD (2024) conditions molecular generation on a protein pocket. Boltz-2's
2025 preprint combines complex prediction and affinity modeling; an independent
2026 study evaluates that model on defined target/compound datasets.
[S15](RESEARCH_REFERENCES.md#s15), [S16](RESEARCH_REFERENCES.md#s16),
[S17](RESEARCH_REFERENCES.md#s17).

**Implication to discuss:** these are possible inputs to a design workflow,
with distinct endpoints. A generated structure, plausible pose or affinity
estimate does not determine functional allosteric modulation. AlloMT would
need functional/state-specific objectives, realistic controls, chemical-quality
assessment and held-out comparisons for its intended task (P05, P07, P10).

## How to use these trends

These papers establish examples and methods, not a universal validated solution
to N01–N13. Promising directions are opportunities to formulate and test AlloMT
questions. Source availability, permissive rights, maintenance, acquisition,
hardware and actual scientific receiving remain distinct gates. In particular,
BioEmu2's core MIT label does not cover all bundled assets/notices; see the
[source-level tool review](METHODS_AND_TOOLS.md).

The proposed new functions are not automatically part of the agreed product.
Priorities, representative systems and success criteria remain to be negotiated
under [AlloMT #3](https://github.com/uibcdf/allomt/issues/3).
