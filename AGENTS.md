# AlloMT contributor instructions

## Mandatory MolSysSuite instructions

Read and follow `MOLSYSSUITE_GUIDE.md` before working in this repository.

Within their stated scope, its common rules take precedence over this file
and any nested `AGENTS.md`. Local instructions may refine them; deviations
require the documented policy exception process.

The synchronized guide is owned by `uibcdf/molsyssuite`. It includes the
[reusable-tool ownership rules](MOLSYSSUITE_GUIDE.md#modular-reusable-tools)
and [working-instruction rules](MOLSYSSUITE_GUIDE.md#durable-working-instructions).
For work under `devguide/`, also read `devguide/AGENTS.md` and its local
reporting protocol. Keep repository-specific instructions below.


## Local ownership and publication

AlloMT is registered as an incubating component; central admission is tracked in
`uibcdf/molsyssuite#202`, with local receiving in `uibcdf/allomt#1`.
Keep current admission identities and missing gates in `devguide/ADMISSION.md`.
Registration and guide receipt do not prove official generation, current-policy
adoption or member/scientific qualification; retain their actual executed evidence.

Diego authorizes direct commits and pushes to `uibcdf/allomt`; no PR is needed
for this repository. For changes owned by another UIBCDF repository, use its
owning issue as the normal route. Publishing a PR there is exceptional, rather
than the default route for a proposed fix. Preserve authorization within its
stated scope and follow the inherited validation checkpoints.

Write repository prose, code and issue records in English. Read
`devguide/OBJECTIVES.md`, `devguide/SCIENTIFIC_SCOPE.md` and
`devguide/COMPONENT_RESPONSIBILITIES.md` before scientific design. Keep objective
exploration broad and open to multiple conceptual approaches and applications.
A first implementation example must not define or restrict the overall scope.
Define concrete scientific increments under their owning issues when work is
commissioned; `uibcdf/allomt#2` tracks a future first increment, not a gate on
discovering objectives. No single universal allostery model or pipeline is required.

Reuse provider public operations. TopoMT owns cryptic-pocket detection,
BindingMT owns binding-energy calculation/prediction, ElastNetMT owns reusable
ENM numerical work, and landscape/state/kinetic work is coordinated with
LandscapeMT. AlloMT develops allostery-specific science, interpretation and
composition. Acceptance of goals/method families does not adopt a particular
third-party library, waive licensing or claim implementation/qualification.

## Canonical integration guides

Read the relevant synchronized guide before changing a tool integration:
`SMONITOR_GUIDE.md`, `ARGDIGEST_GUIDE.md`, `DEPDIGEST_GUIDE.md`,
`PYUNITWIZARD_GUIDE.md`, `ACKREDIT_GUIDE.md`, `PYTEST_RECEPTOR_GUIDE.md`, and
`GH_RUN_RECEPTOR_GUIDE.md`. These and `MOLSYSSUITE_GUIDE.md` are read-only
consumer copies. Use the central registered synchronizer for subsequent
distribution; propose changes at the canonical provider source. Guide receipt
does not establish a runtime dependency or accepted central membership.

## Local development commands

The generated `devtools/conda-envs/` files are CI/bootstrap and clean
qualification fixtures. Shared-development eligibility and actual import/closure
receiving are recorded centrally; use the named shared environment when eligible.

Select the applicable commands and test scope for the change:

```bash
ruff check .
ruff format --check .
python -m pytest --receptor=llm
python devtools/devguide_index.py --check
```

The issue-backed lifecycle is mapped to this repository in
`devguide/reporting_protocol.md`. For Discussions triage and resource upkeep,
read `devguide/discussions.md`. Add only accepted repository-specific actions
here, such as scientific contracts, source layouts, specialized gates and local
commands. Keep technical findings in issues, tests and maintained documentation.
