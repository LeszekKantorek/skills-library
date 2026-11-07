# systematic-debugging

## Identity and versions

* Identifier: `obra-superpowers-systematic-debugging`; author: obra; type: skill. Assessed item: [skills/systematic-debugging](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/skills/systematic-debugging/SKILL.md) in [obra/superpowers](https://github.com/obra/superpowers).
* Catalog analysis: [8ca22dba9a94f28898bbce59f2537ff4d87c747d](https://github.com/obra/superpowers/commit/8ca22dba9a94f28898bbce59f2537ff4d87c747d), 2026-11-07; item scope: 11 files in the [pinned tree](https://api.github.com/repos/obra/superpowers/git/trees/8ca22dba9a94f28898bbce59f2537ff4d87c747d?recursive=1).
* Latest observed: [22f0b463e7a5e579904dd6211a520321035526f7](https://github.com/obra/superpowers/commit/22f0b463e7a5e579904dd6211a520321035526f7), `main`, observed 2026-11-07 through the [branch API](https://api.github.com/repos/obra/superpowers/branches/main). Comparison of the complete [pinned tree](https://api.github.com/repos/obra/superpowers/git/trees/8ca22dba9a94f28898bbce59f2537ff4d87c747d?recursive=1) and [observed tree](https://api.github.com/repos/obra/superpowers/git/trees/22f0b463e7a5e579904dd6211a520321035526f7?recursive=1) shows the item is changed by paths and blob IDs. The newer head is not security assessed here.
* Security assessment: `8ca22dba9a94f28898bbce59f2537ff4d87c747d`, 2026-11-07; operational risk: high; completeness: partial.

## Purpose and contents

The [skill](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/skills/systematic-debugging/SKILL.md) addresses root-cause debugging and verification. It is intended for developers investigating failures before fixes. It is less suitable for production diagnostics with real credentials or uncontrolled tests. Its advice and factual claims were not independently validated.

Eleven files: instructions, Markdown technique and evaluation fixtures, a TypeScript example, and one executable Bash script. No item-local MCP configuration. Git, Bash, npm, project tests and companion skills are external; example TypeScript imports project-specific types. The [pinned tree](https://api.github.com/repos/obra/superpowers/git/trees/8ca22dba9a94f28898bbce59f2537ff4d87c747d?recursive=1) defines the file inventory. Installation and later use are separate; no installation or item tests were executed.

## Installation

See the [source installation guidance and caution](README.md#installation). Its installer and any separately obtained components are outside this assessment.

## License

The [repository MIT license](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/LICENSE) applies to the item; no separate item license was identified. It requires retaining its copyright and permission notice and disclaims warranties.

## Security

Static assessment covers the 11 pinned item files and the documented source installation route at `8ca22dba9a94f28898bbce59f2537ff4d87c747d` on 2026-11-07. Completeness is **partial** and confidence is moderate for visible source, limited for actual host behavior. Project code, host tools, providers, independently downloaded installers and unbundled companions are excluded.

* The [diagnostic example](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/skills/systematic-debugging/SKILL.md#L91) prints identity values, inspects keychains and invokes signing; a nonempty identity can appear in logs. The [find-polluter script](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/skills/systematic-debugging/find-polluter.sh#L51) runs project-controlled npm tests repeatedly, suppresses failures and splits whitespace in paths. Use disposable resources and redact secrets.
* Source instructions are task guidance and cannot grant new permissions. Untrusted project content or fetched material can redirect an agent; treat it as data and limit accessible context. Review generated commands and changes before use.

**Risk: high.** The examples can expose sensitive identity values and run project-controlled tests. This is not a safety guarantee. Runtime behavior, external integrations, and quality of advice remain unverified.

## Validation

Documented: pinned source installation guidance. Static verification: fetched all item files at the pinned commit, compared their Git blob IDs to local evidence copies, scanned all item files for operational and security terms, inspected the instructions and operation-bearing references and scripts, and observed the upstream branch. The [legacy import report](../../imports/obra-superpowers-systematic-debugging.md) records earlier provenance and its actual scope. No source scripts, installers, project tests, agents, remote actions or examples were executed.
