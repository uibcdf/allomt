# Ecosystem and ownership

This map records the repository review used to start AlloMT and the R03 ownership
clarifications on 2026-11-15. [The responsibility matrix](COMPONENT_RESPONSIBILITIES.md)
is the detailed coordination route for the accepted objectives.
It guides reuse; it does not certify installed compatibility. The central
[suite registry](https://github.com/uibcdf/molsyssuite/blob/main/suite.toml)
owns current membership and applicability. Each provider owns its actual public
contracts, implementation and qualification.

## Platform and scientific components

| Repository | Responsibility relevant to AlloMT |
| --- | --- |
| [MolI](https://github.com/uibcdf/moli) | Platform architecture and contracts between platform components. MolSysSuite has delegated governance of its members. |
| [MolSysSuite](https://github.com/uibcdf/molsyssuite) | Shared engineering/modeling rules, member registry, official starter, guide inventories and coordinated adoption. |
| [MolSysMT](https://github.com/uibcdf/molsysmt) | Molecular systems, topology/chemical-state/structure boundaries, selection, identity maps, structural analysis and interoperability. |
| [MolSysViewer](https://github.com/uibcdf/molsysviewer) | Molecular visualization and supported scientific add-on integration; presentation does not own AlloMT's scientific results. |
| [TopoMT](https://github.com/uibcdf/topomt) | Molecular topography, pockets, surfaces and interfaces, including cryptic-pocket detection across conformations. AlloMT consumes these results for allosteric assessment. Actual supported profiles retain their own qualification. |
| [BindingMT](https://github.com/uibcdf/bindingmt) | Binding modeling and characterization. Docking and initial interface profiles exist; broader complex prediction/refinement and free-energy directions have separate qualification. |
| [PharmacophoreMT](https://github.com/uibcdf/pharmacophoremt) | Pharmacophore features/shapes, model construction, comparison and screening through its implemented profiles. |
| [ElastNetMT](https://github.com/uibcdf/elastnetmt) | Elastic-network numerical modeling. Preserve its actual normalization, units, supported modes and backend boundaries. |
| [LandscapeMT](https://github.com/uibcdf/landscapemt) | New provider direction for conformational exploration, FEL/state/kinetic analysis and ensemble inference. Coordinate boundaries with TopoMT, BindingMT, ElastNetMT and AlloMT; preview/scope does not establish a working public API. |
| [PeptideMT](https://github.com/uibcdf/peptidemt) | Peptide design and functional evaluation. Retain candidate occurrence identity, original outcomes, provider scope and model limitations. |
| [Sabueso](https://github.com/uibcdf/sabueso) | Scientific knowledge under direct MolI governance; neither a suite member nor AlloMT's execution engine. |
| [MolSysSketcher](https://github.com/uibcdf/molsyssketcher) | Reusable molecular 2D representations and interaction-diagram direction. Bounded TypeScript/document/SVG foundations exist; suite admission is tracked in [MolSysSuite #199](https://github.com/uibcdf/molsyssuite/issues/199). |
| [ViableMT](https://github.com/uibcdf/viablemt) | Conceptual ADMET/developability direction. The reviewed repository supplies a README, not an implemented provider API. |

AlloMT owns the allostery-specific scientific layer and develops it across broad
conceptual approaches/applications. Accepted scientific objectives can depend on
operations owned elsewhere. Integration interest does not create a dependency,
an adapter, a received provider API or a second implementation of provider work.

## Support and developer tools

| Provider | Responsibility and integration boundary |
| --- | --- |
| [SMonitor](https://github.com/uibcdf/smonitor) | Catalogued diagnostics and scoped capture; preserve application configuration. Diagnostics are distinct from scientific results. |
| [ArgDigest](https://github.com/uibcdf/argdigest) | Public argument contracts, validation and normalization; keep heavy provider imports lazy. |
| [DepDigest](https://github.com/uibcdf/depdigest) | Declared dependencies, optional-route guards and installer hints. Availability does not prove compatible execution. |
| [PyUnitWizard](https://github.com/uibcdf/pyunitwizard) | Shared physical-quantity policy and explicit conversions; preserve the application's active policy. |
| [Ackredit](https://github.com/uibcdf/ackredit) | Optional scientific attribution with application-owned capture. References remain distinct from scientific evidence and diagnostic events. |
| [Recorda](https://github.com/uibcdf/recorda) | Experimental semantic execution recording under direct MolI governance. It is not introduced as a scaffold dependency or integration. |
| [PytestReceptor](https://github.com/uibcdf/pytest-receptor) | Test reporting; preserve actual collection, test results and native exit status. The starter pins a published tool version. |
| [GHRunReceptor](https://github.com/uibcdf/gh-run-receptor) | Read-only CI capture/inspection. Native GitHub run, attempt, job and executed-step outcomes determine the claim. |

The registered root guides are canonical synchronized copies. Consult the
relevant guide before introducing or changing an integration; guide receipt alone
does not mean that its provider is a runtime dependency. Do not edit consumer
copies. Guide ownership and delivery follow MolSysSuite's registered synchronizer.

## Issue ownership

Use `uibcdf/allomt#N` for AlloMT's code and scientific contracts,
`uibcdf/molsyssuite#N` for shared member rules/admission, and the provider's own
issue for a provider limitation. Link the consumer and provider work in both
directions. Changes to inter-platform contracts belong to MolI. Use stable
repository/issue identities in maintained prose rather than sibling paths.
