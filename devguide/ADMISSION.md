# Admission and bootstrap status

AlloMT is a **source candidate** for MolSysSuite membership. Registration and
guide-consumer relationships are requested in
[MolSysSuite #202](https://github.com/uibcdf/molsyssuite/issues/202).
The member-policy gate and accepted component admission remain pending.

## Source provenance

The candidate uses the official Python component template and instruction
renderer from central commit `e4d97ba1ac5341aa2d1cd50b56096098e59bb940`.
Engineering values were read from the genuine local immutable `policy-v1.5.12`
snapshot. The MIT license and its notice are retained from that source.

The accepted-member generator was attempted against that clean central checkout:

```text
bootstrap_component.py ... --repository uibcdf/allomt ...
exit 2: 'uibcdf/allomt' must be registered in suite.toml first
```

It has **not passed**. Template files were rendered as a pre-admission source
candidate; no member was inserted into a published registry, no admission SHA
was invented, and no successful formal generation is claimed. The original Git
history and owner-authored scope documents are retained.

## Local adaptations

- Concrete AlloMT purpose, scientific scope, ownership map and issue routes.
- Explicit English guidance and Diego's authorization for direct AlloMT pushes;
  owning issues are the normal route in other UIBCDF repositories.
- Byte-identical provider guides received from immutable upstream snapshots via
  the central synchronizer's `process` operation and proposed guide relationships.
  Central relationship acceptance is still pending; provenance is retained in
  [the source receipt](validation/bootstrap_sources.json).
- All canonical guide paths excluded explicitly from local Ruff ownership.
- Full source reporting/import tests; routine Linux Python 3.14 CI and
  scheduled/manual Linux 3.11–3.14 lanes, following the starter.
- The frozen policy caller is manual and requires a real published
  `admission_sha`. Automatic member-policy enforcement must be activated after
  central registration. Ordinary source CI does not replace this missing gate.

## Receiving and qualification

Local qualification uses a temporary isolated Conda environment with only
`uibcdf` and `conda-forge` acquisition, Python 3.14.10, PytestReceptor 1.1.0,
Ruff 0.16.5, pytest 9.2.0, versioningit 3.3.0 and Setuptools 84.2.1. It is a
bootstrap fixture, not joint receiving into a shared daily-development profile.
Executed checks and hosted results are recorded under
[AlloMT #1](https://github.com/uibcdf/allomt/issues/1) and its
[local record](pending_proposals/component_bootstrap.md).

There is no claimed macOS/Windows support, scientific qualification, measured
coverage percentage, public package or release. Coverage applicability must be
reviewed when meaningful scientific production code exists; no percentage badge
is supplied by this import/reporting scaffold.

## Central completion route

The central owner accepts the classification and guide relationships, reconciles
the review/publisher/archival/coverage/dependency inventories and publishes the
registration on `main`. Keep ecosystem/CI/distribution evidence states accurate.
Then retain the real full admission commit and use the official generator in an
empty stage with `--admission-sha`, reviewing integration against this candidate.

Restore the starter's automatic push/PR policy triggers with the immutable
admission input, verify the real shared gate and live guide synchronization,
and record the applicable hosted compatibility and workspace receiving.
Branch protection and GitHub Discussions configuration also need actual
repository-side verification; generated files do not establish either.
Keep source and scientific follow-up in AlloMT #1 and
[AlloMT #2](https://github.com/uibcdf/allomt/issues/2).
