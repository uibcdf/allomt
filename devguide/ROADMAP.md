# Initial roadmap

These are planning notes. The current phase is researcher-needs elicitation;
the full scientific scope, architecture and feature priorities are being
negotiated. Need ordering is not a delivery order, and no scientific-method
timeline has been agreed.

## W0: component foundation

Owner: [AlloMT #1](https://github.com/uibcdf/allomt/issues/1).
Central admission: [MolSysSuite #202](https://github.com/uibcdf/molsyssuite/issues/202).
The initial PR #203 was withdrawn when Diego selected an issue-first contribution
route in other UIBCDF repositories. Admission is pending; see [status](ADMISSION.md).

Establish the official Python scaffold, MIT license, local contributor routes,
issue-backed report queues and archive, canonical guide relationships and
explicit scientific scope. Qualify local import/build/reporting/quality and
repository checks. Record hosted compatibility, branch protection, developer
workspace receiving and coverage applicability with their actual evidence.
The source foundation alone has no scientific or public-release qualification.

## W1: researcher needs and negotiated design

Current owner: [AlloMT #3](https://github.com/uibcdf/allomt/issues/3).

Maintain [the needs](RESEARCHER_NEEDS.md), [discussion history](DESIGN_DISCUSSION.md),
[questions](DESIGN_QUESTIONS.md) and [provisional architecture](ARCHITECTURE.md)
over the planned discussion rounds. Faithfully capture the broad scientific
vision, clarify concrete contexts and distinguish proposals from agreements.

### Later first scientific contract

Owner: [AlloMT #2](https://github.com/uibcdf/allomt/issues/2).

Select one concrete allostery question, a representative input, an appropriate
method and the smallest useful output. Specify interpretation, assumptions,
uncertainty, provenance, units and correspondence through the actual workflow.
Inspect reusable provider APIs and link missing capabilities to their owners.
No first method, public API, source-module layout or generalized plugin/result
architecture is selected yet. Selection follows the needs discussion.

## W2: first reproducible scientific increment

After W1 selects the contract, implement its reusable operation, example and
meaningful numerical/scientific checks. Keep dependency acquisition, optional
execution, saved-result reading and attribution scoped to the implemented use.
Record installed-provider and scientific evidence separately from source tests.
Create an owning implementation issue when the accepted method is concrete.

## Later integration and delivery

Assess visualization, additional mechanisms/methods, portable results, scientific
benchmarks and distribution when actual workflows justify them. A first public
release needs its own reviewed version, package plan and installed-artifact
evidence. No package publication or additional scientific campaign is authorized
or claimed by this roadmap.
