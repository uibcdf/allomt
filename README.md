# AlloMT

**Allostery MultiToolkit** — prediction and characterization of allosteric
mechanisms, being developed as a MolSysSuite scientific component within MolI.

The current source provides the repository foundation and an importable Python
package. A future first scientific increment is tracked in
[AlloMT #2](https://github.com/uibcdf/allomt/issues/2); no scientific workflow is
implemented yet.

We are currently eliciting researcher needs over several design-discussion
rounds. [The developer guide](devguide/README.md) maintains the thirteen stated
needs, accepted objectives, component responsibilities, discussion history, open
questions and provisional architecture under
[AlloMT #3](https://github.com/uibcdf/allomt/issues/3). Objective exploration stays
broad and open to multiple allostery approaches and applications. The
[Discussions catalog](devguide/discussions.md) curates tools, functions, databases,
benchmarks and research without implying adoption or duplicating provider work.

Central admission was published in
[`adaef199`](https://github.com/uibcdf/molsyssuite/commit/adaef199b74c6da72ca43c21401c245990c70727)
under [MolSysSuite #202](https://github.com/uibcdf/molsyssuite/issues/202).
The initial source used official starter sources and `policy-v1.5.12`;
official generation and automatic current-policy receiving remain under
[AlloMT #1](https://github.com/uibcdf/allomt/issues/1). See
[admission and bootstrap status](devguide/ADMISSION.md) for the separate evidence.

## Development

Use Python 3.14 for routine work. The compatibility target is Python 3.11–3.14;
actual qualification is recorded in [the developer guide](devguide/README.md).
The committed Conda YAMLs are bootstrap/CI fixtures with `uibcdf` and
`conda-forge` providers. Shared-workspace receiving remains tracked in
[AlloMT #1](https://github.com/uibcdf/allomt/issues/1).

With the compatible development environment activated:

```bash
python -m pip install --no-deps --no-build-isolation --editable .
python -m pytest --receptor=llm
python devtools/devguide_index.py --check
ruff check .
ruff format --check .
```

Read [AGENTS.md](AGENTS.md), the synchronized
[MolSysSuite guide](MOLSYSSUITE_GUIDE.md), and
[the developer guide](devguide/README.md) before contributing.
Work is tracked through owning issues, local report queues and a permanent archive.
Canonical root integration guides remain owned by their provider repositories.

The source is licensed under [MIT](LICENSE). There is no public AlloMT package
or validated scientific predictor yet; installation above is for source development.
