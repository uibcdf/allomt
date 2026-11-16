# Scientific scope

AlloMT (Allostery MultiToolkit) is being developed to predict and characterize
allosteric mechanisms within MolSysSuite, the molecular modeling ecosystem of
MolI. Its scientific scope is broader than any single method or backend.

## Intended scientific boundary

AlloMT will connect explicit molecular inputs, states and perturbations to
testable descriptions of allosteric responses. Candidate tasks include comparing
states or ensembles, characterizing coupling between molecular regions, studying
responses to perturbations, and assembling method-specific support for proposed
communication mechanisms. Each task needs its own question, method, applicability
and validation before it becomes an implemented capability.

The first workflow and numerical method are still to be selected in
[AlloMT #2](https://github.com/uibcdf/allomt/issues/2). This scaffold provides no
predictor, allosteric score, pathway algorithm, trained model or scientific API.

## Interpretation and evidence

Keep a computed observation separate from its mechanistic interpretation. A
correlation, elastic mode, contact network, visual pattern or method-specific
score must retain its actual meaning and limitations. Do not present one as
experimental confirmation, a causal mechanism or a physical free energy without
the corresponding method and evidence.

For every implemented workflow, state the biological question, analyzed states,
input preparation, assumptions, reference/comparison, supported systems and
unresolved uncertainty. Numerical correctness, installed-engine execution and
biological validation are separate qualification claims. Negative, missing,
unsupported and failed outcomes must remain distinguishable.

## Reusable component ownership

Use public provider operations for capabilities already owned elsewhere:

- MolSysMT: molecular representation, acquisition, selections, atom/group maps,
  chemical states, structural operations and trajectory access.
- ElastNetMT: elastic-network construction and its numerical methods, when a
  selected workflow requires them.
- TopoMT, BindingMT and PharmacophoreMT: their specialized topography, binding
  and pharmacophore calculations when applicable.
- MolSysViewer and, when applicable, MolSysSketcher: presentation and interaction
  through their supported interfaces.

AlloMT owns the allostery-specific operations, comparisons, interpretation and
result contracts that compose those tools. Inspect available public APIs before
adding a primitive; report an actual missing provider capability in its owning
repository with linked AlloMT evidence.

See [the ecosystem map](ECOSYSTEM.md) for membership and integration distinctions.

## Result design constraints

Apply these to the first concrete workflow; they do not prescribe a generic
result framework before one is needed:

- Preserve molecular identity, selection expression and resolved ordering,
  atom/group correspondence, chemical-state identity and analyzed structure or
  trajectory-frame association wherever relevant. Indices and identifiers are
  distinct; do not silently remap a provider's output.
- Make quantities and conversions explicit through the shared PyUnitWizard
  policy. Preserve the actual units or dimensionless meaning of each method.
- Identify the method, backend, version, parameters, input provenance, preparation
  and execution status. Retain supplied uncertainty and explain absent estimates.
- Keep scientific data/results, SMonitor diagnostics, Ackredit references and
  optional Recorda execution records distinct. Reading a saved result must not
  imply a new calculation or new scientific evidence.
- Define the smallest reusable public operation needed by the accepted workflow,
  with meaningful numerical/scientific checks and a reproducible example.

## Current implementation boundary

The initial milestone is repository and engineering infrastructure under
[AlloMT #1](https://github.com/uibcdf/allomt/issues/1). Scientific algorithms,
runtime provider dependencies and result schemas will be introduced only as
required by the selected workflow. No public package, biological benchmark,
frontend integration or platform-support result follows from this scaffold.
