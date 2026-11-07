# Item report template

Replace the title with the item name. Replace prompts with evidence or an explicit unknown. Link source evidence to the full commit and relevant path. Retain prior assessments as dated history when updating.

## Identity and versions

* Stable identifier, name, author, type, repository, item path, and assessed scope:
* Catalog analysis: full commit SHA, permalink, and date:
* Latest observed: full commit SHA, branch, observation date, and evidence of whether changes affect this item (`changed`, `unchanged`, or `unknown`):
* Security status (`not assessed`, `stale`, or `current`), security commit and date, and current risk (`unknown` when stale or not assessed):

## Purpose and contents

* Purpose, intended users, concrete uses, and unsuitable cases:
* Inventory of instructions, scripts, tests/evals, prompts, agents, hooks, MCP configuration, assets, and dependencies; distinguish installation, later use, and tests:
* Evidence and gaps:

## Platforms

For each platform, record the author's claim, file evidence, and verification result or `unverified`. Distinguish item support from installer or plugin support.

## Installation

Record exact documented commands and source links, prerequisites, execution location, project or user scope, and what is downloaded or installed. Identify independently versioned installers and moving references. State `installation method unverified` where evidence is missing; do not invent commands or claim pinning without support.

## License

Record identifier or missing/unclear terms, scope, exceptions, and pinned evidence. A catalog description does not establish redistribution rights.

## Security

* Assessment scope and independently versioned components, configurations, and exclusions:
* Findings: pinned evidence, behavior and data recipients, scenario, impact, and safeguards:
* Operational risk and rationale; completeness (`complete`, `partial`, or `not assessed`), confidence, recommendation, and limitations:
* Unresolved questions:

## Validation

Separate documented claims, static verification, and tests performed. Record files inspected, environment, test results, and what was not checked. Do not describe a historical review as a new audit.

## History

Link prior reports, issues or PRs, and material changes. Preserve prior security commit, date, scope, risk, and limitations as historical information.
