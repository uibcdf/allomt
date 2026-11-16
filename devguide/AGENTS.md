# allomt developer-guide instructions

Read `../AGENTS.md` for repository-wide rules and `reporting_protocol.md` for
the local issue and report lifecycle. Active issue-backed analyses live in
`pending_bugs/` and `pending_proposals/`; `archive/` preserves resolved and
superseded history. Use the generated indexes to find current work. Read an
archived report when tracing a decision, then check the current replacement
before treating it as a rule.

Keep technical facts and defect details in maintained documents, tests and
owning issues. Put only lasting working instructions specific to this
directory here, and repository-wide working instructions in the root
`AGENTS.md`. Follow the local reporting protocol to synchronize issues and
report states. After a report lifecycle change, run
`python devtools/devguide_index.py` to regenerate indexes, then run it with
`--check` to verify them.

Follow [the canonical instruction policy](../MOLSYSSUITE_GUIDE.md#durable-working-instructions)
for accepted lasting actions and feedback beyond this component.

## Iterative design records

During the design discussion, maintain `RESEARCHER_NEEDS.md`,
`OBJECTIVES.md`, `COMPONENT_RESPONSIBILITIES.md`, `DESIGN_DISCUSSION.md`,
`DESIGN_QUESTIONS.md` and `ARCHITECTURE.md` as the
relevant rounds progress. Keep the scope and reading path consistent with them.
Distinguish researcher-stated needs, assistant interpretations, proposals,
confirmed agreements and open questions. Record significant revisions and their
reasons with stable need/question identities. Mark a design choice as agreed
only when the discussion establishes that agreement. These records support
several rounds of broad needs exploration before implementation choices are settled.
Do not turn a first example, functional interpretation or conceptual scheme into
an artificial limit on AlloMT's scientific scope. Keep accepted objectives distinct
from provider ownership, backend adoption and actual implementation evidence.

Before working in Discussions, read `discussions.md`. Keep substantive resource
reviews in their authoritative conversations; maintain only the necessary routing,
decision records and thin catalog index here. A catalog entry can describe another
component's operation without transferring its ownership to AlloMT.
