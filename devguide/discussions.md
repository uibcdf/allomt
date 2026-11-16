# AlloMT Discussions and scientific resource catalog

**Live entry point:** [catalog and resource index](https://github.com/uibcdf/allomt/discussions/5).
**Setup/receiving owner:** [AlloMT #4](https://github.com/uibcdf/allomt/issues/4).
**Accountability:** AlloMT maintainers, currently Diego Prada Gracia, until
explicitly delegated. There is no response-time commitment.

The catalog supports broad, open-ended exploration: tools, algorithms, functions,
databases, datasets, benchmarks, papers and other resources. A resource may concern
another component's operation. Cataloging it does not transfer ownership, adopt
software or limit AlloMT to one framework. Read [the responsibility map](COMPONENT_RESPONSIBILITIES.md)
and the common [Discussions policy](../MOLSYSSUITE_GUIDE.md#github-discussions).

## Actual category routes and purposes

Discussions was enabled on 2026-11-15. Before activation, the API reported no
categories or conversations. Generated defaults were retained; no content,
category or conversation was removed. AlloMT maintainers own triage in every route.

| Category / observed slug | Use and useful opening information | Durable destination |
| --- | --- | --- |
| Announcements / `announcements` | Maintainer updates with a link to an existing release, accepted contract or decision. | The linked release/decision record remains authoritative. |
| Q&A / `q-a` | Usage/interpretation; include versions, scientific question, permitted minimal input and expected/observed result. | Mark useful answers; actionable findings go to owning issues, lasting clarifications to maintained guidance. |
| Ideas / `ideas` | Scientific functions and possible workflows, including provider handoffs. Use the function form for objectives, ownership, evidence and questions. | Canonical idea thread; concrete work becomes an owning issue, decisions a linked issue/versioned record. |
| General / `general` | Resource catalog intake: tools, methods, databases, datasets, benchmarks, papers and review pointers. Use the resource form and canonical source/key. | Canonical resource thread, linked from the catalog; actionable work and decisions keep their owning records. |
| Show and tell / `show-and-tell` | Reproducible studies, examples or visualizations with versions, sources and evidence limits. | Link the study/artifact and relevant resource thread or issue; a showcase is not scientific qualification. |
| Polls / `polls` | Informal preferences with the question and context stated. | Link any resulting decision to its owning issue/versioned record; votes alone accept no contract or method. |

Keep the common Announcements, Q&A and Ideas categories even when empty. General
is purposeful local catalog intake rather than three additional resource categories.
Separate tool/data/literature categories can be considered if volume warrants them.
No additional labels are selected; none were applied to the seeds.

## Storage and discoverability

- The [catalog Discussion](https://github.com/uibcdf/allomt/discussions/5) is the
  human entry point; each resource/function has an authoritative conversation.
- [catalog.json](discussions/catalog.json) is a thin routing index: stable key,
  kind, source, scientific owner, related objectives and actual Discussion identity.
  It does not duplicate review bodies, status histories or evidence assessments.
- Initial keys use `kind:short-name`, such as `tool:prody`,
  `function:cryptic-pockets` and `benchmark:allostery-tasks`. Search the source,
  key and existing discussions before adding an entry. Titles use readable types
  such as [Tool], [Function], [Database] or [Benchmark]; these are not GitHub labels.
- Store datasets, trajectories, weights and benchmark artifacts in their appropriate
  sources/archives, with versioned identifiers/checksums when available. This catalog
  stores pointers and curation, not large or restricted assets. Target-specific
  biological knowledge remains coordinated with Sabueso.

The R02 [bibliography](RESEARCH_REFERENCES.md) and
[immutable license snapshot](research/tool_inventory_2026_11_15.json) retain dated
research evidence. Subsequent substantive reviews belong in threads; relevant
accepted decisions and reproducible artifacts retain their durable destinations.
Do not make every conversation finding a compulsory duplicate document.

## Intake and assessment

Source forms are [General](../.github/DISCUSSION_TEMPLATE/general.yml) and
[Ideas](../.github/DISCUSSION_TEMPLATE/ideas.yml), matching observed slugs.
Use the same information for API/manual posts. Unknown values are acceptable when
stated; no complete implementation contract is needed to catalog an early idea.

Include scientific use, canonical source, exact version/commit where relevant,
review date/reviewer, scientific owner or unresolved ownership, related goals if
useful, and evidence with its limits. Distinguish code, weights, data, bundled
notices and service/access terms. For benchmarks, state the task, reference/negative
evidence, provenance, proposed splits and rights; unknown metrics/thresholds stay
open. Related objectives are links, not an exhaustive allowed scope.

Keep these independent claims distinct in the conversation:

| Claim | Meaning |
| --- | --- |
| Interest/objective | Why a resource/function matters; link N/P acceptance to R03 when relevant. |
| Scientific ownership | Component supplying each reusable operation; allocate package functions individually when needed. |
| Assessment evidence | Suggested, source-inspected, installed, executed or benchmarked, with version/date and actual evidence. |
| Rights/access | Known terms or unresolved review of the intended code/model/data/service route. |
| Adoption/disposition | Unselected, candidate, deferred/held, rejected for a stated use, or adopted under a linked decision. |

Use descriptive wording rather than forcing every resource into a numerical score.
A GPL tool can be a scientific reference while outside the initial permissive
integration criterion. A relevant family can be accepted with no package selected.
A planned provider feature is not a working public API.

## Upkeep, duplicates and conversion to work

Maintainers check new entries for a canonical thread, sources, ownership and
actionable work. Update the live index and thin JSON when an entry is added,
merged by reference or relocated. Review on new evidence, upstream releases,
reported errors and concrete integration use; there is no automatic freshness
guarantee.

Append dated review comments with version/source, reviewer, changed evidence and
reason. Correct mistakes visibly; retain useful historical claims with their date
and correction. Reuse an existing thread for ordinary version updates. A separate
entry needs a materially different resource/task and a link to its predecessor.
Link duplicates to the canonical conversation, preserving useful content and links.

Concrete suspected defects, missing provider operations and implementation proposals
go to their owning repository, even when uncertain or nonblocking. Link the thread
from that issue and the issue back from the thread. AlloMT keeps its consuming
question. Ownership is not transferred by a vote/title/catalog entry; shared
contracts use the normal owner process.

Record accepted/deferred/rejected decisions with date and reason in an owning
issue or named versioned record. Deferral includes a concrete revisit trigger.
Link both directions; mark answered or close when useful with the disposition.
Neither closure nor a source review establishes scientific performance. Follow
existing authorization/disclosure rules; catalog reading grants no subscriptions
or implementation work.

## Observation limits and remaining receiving

On 2026-11-15 native API readback verified activation, six category names/slugs
and default descriptions, Q&A `isAnswerable=true`, the index and eleven initial
entries with actual IDs/categories/content. These observations are separate from
committed forms and local guidance.

The available API does not expose Announcement/Open-ended format settings,
category editing or pinning; no browser/UI verification was performed. Source
validation does not establish rendered form behavior. No category description
edits or pinning are claimed; standard descriptions remain unchanged.

**Bounded receiving follow-up:** [AlloMT #4](https://github.com/uibcdf/allomt/issues/4),
responsible maintainer Diego Prada Gracia; review by **2026-12-15**. Scope: verify
Announcements/Ideas formats in the UI, confirm General/Ideas forms render, and
adapt descriptions if useful. Reason: these settings are not exposed by the
available API/editor. Interim route: live General/Ideas threads and the fields
above. Remove the pending state once actual UI evidence is recorded there;
source delivery/API category names alone do not clear it. Catalog curation
is already available.
