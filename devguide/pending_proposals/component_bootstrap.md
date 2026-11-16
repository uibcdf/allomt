---
summary: Establish the AlloMT source foundation and complete central member receiving.
issue: uibcdf/allomt#1
status: partial
opened: 2026-11-15
closed:
verification: inspected
area: [bootstrap, governance]
guard:
normative:
blocked_by: [uibcdf/molsyssuite#202]
supersedes: []
---

# AlloMT component foundation

## What

Prepare AlloMT as a primary, active, incubating scientific Python component
within MolSysSuite, retaining MolI's platform ownership boundary.

## How

Use the official starter sources for the initial candidate. Provide MIT license,
an importable package, scientific scope and component ownership, canonical local
integration guides, report queues/archive/index validation and inherited source
CI. Track the real central admission before claiming successful official
generation or member-policy enforcement.

## Why

A new scientific component needs reusable tools, traceable work and explicit
qualification from its first source increment. A scaffold does not establish
allostery algorithms, scientific results, installed-provider compatibility or
public availability.

## Evidence and current limits

[Admission status](../ADMISSION.md) records exact source provenance and outstanding
gates. The official bootstrap stops at missing central membership, as expected.
The initial PR in MolSysSuite was withdrawn under Diego's issue-first route;
uibcdf/molsyssuite#202 retains the proposed registration. No central merge is
authorized. The first scientific method remains unselected under uibcdf/allomt#2.

Local source receiving on 2026-11-15 used the isolated Conda fixture described in
`ADMISSION.md`: Python 3.14.10, published PytestReceptor 1.1.0 and Ruff 0.16.5.
Editable installation, isolated import-origin inspection and `pip check` passed.
`python -m pytest --receptor=llm` passed **two tests** (import and report lifecycle).
The generated index check, Ruff lint/format and local documentation-link check
passed. All eight guide files match the recorded upstream Git blob identities.

Wheel and source archive builds passed. A separate clean environment imported the
installed wheel from its own site-packages and verified SPDX `MIT`, the declared
license file and the unchanged notice bytes. The source archive contains the
package, license and reporting/devguide inputs. These were unreleased local
development artifacts, not a public package or release candidate.

The genuine central repository checker exits 1 with `[UNREGISTERED]` against the
published source. Formal generation and policy enforcement remain outstanding;
local source checks do not clear them. Hosted results after publication are
maintained in the owning issue rather than inferred from configured workflows.

Temporary qualification resources are retained at `/tmp/allomt-init.IriNNV`
under this issue while admission/bootstrap receiving remains active. This is an
agent-owned fixture, not the shared human environment. Reuse only while its
source/inputs remain applicable; remove it after receiving or when no longer useful.

## Acceptance

- Source import/build metadata, license and meaningful report-lifecycle checks pass.
- Canonical guide copies match their recorded upstream sources.
- Central admission is published and the official generator and frozen member
  gate pass with a genuine admission commit.
- Routine/compatibility CI, repository protection, workspace receiving and
  coverage applicability retain executed evidence or explicit owner-local work.
- No scientific predictor or public package is inferred from source qualification.

## Owning links

- Central registration: uibcdf/molsyssuite#202.
- Latest-policy adoption: uibcdf/molsyssuite#201.
- First scientific contract: uibcdf/allomt#2.
