# receiving-code-review

## Identity and versions

* Identifier: `obra-superpowers-receiving-code-review`; author: obra; type: skill. Assessed item: [skills/receiving-code-review](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/skills/receiving-code-review/SKILL.md) in [obra/superpowers](https://github.com/obra/superpowers).
* Catalog analysis: [8ca22dba9a94f28898bbce59f2537ff4d87c747d](https://github.com/obra/superpowers/commit/8ca22dba9a94f28898bbce59f2537ff4d87c747d), 2026-11-07; item scope: 1 files in the [pinned tree](https://api.github.com/repos/obra/superpowers/git/trees/8ca22dba9a94f28898bbce59f2537ff4d87c747d?recursive=1).
* Latest observed: [22f0b463e7a5e579904dd6211a520321035526f7](https://github.com/obra/superpowers/commit/22f0b463e7a5e579904dd6211a520321035526f7), `main`, observed 2026-11-07 through the [branch API](https://api.github.com/repos/obra/superpowers/branches/main). Comparison of the complete [pinned tree](https://api.github.com/repos/obra/superpowers/git/trees/8ca22dba9a94f28898bbce59f2537ff4d87c747d?recursive=1) and [observed tree](https://api.github.com/repos/obra/superpowers/git/trees/22f0b463e7a5e579904dd6211a520321035526f7?recursive=1) shows the item is unchanged by paths and blob IDs. The newer head is not security assessed here.
* Security assessment: `8ca22dba9a94f28898bbce59f2537ff4d87c747d`, 2026-11-07; operational risk: high; completeness: partial.

## Purpose and contents

The [skill](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/skills/receiving-code-review/SKILL.md) addresses evaluate and respond to code review. It is intended for developers verifying and applying review feedback. It is less suitable for blindly applying feedback or posting externally without task authorization. Its advice and factual claims were not independently validated.

One Markdown instruction file; no item-local scripts, tests, hooks, agents, MCP configuration, or assets. GitHub CLI and project tests are external. The [pinned tree](https://api.github.com/repos/obra/superpowers/git/trees/8ca22dba9a94f28898bbce59f2537ff4d87c747d?recursive=1) defines the file inventory. Installation and later use are separate; no installation or item tests were executed.

## Installation

See the [source installation guidance and caution](README.md#installation). Its installer and any separately obtained components are outside this assessment.

## License

The [repository MIT license](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/LICENSE) applies to the item; no separate item license was identified. It requires retaining its copyright and permission notice and disclaims warranties.

## Security

Static assessment covers the 1 pinned item files and the documented source installation route at `8ca22dba9a94f28898bbce59f2537ff4d87c747d` on 2026-11-07. Completeness is **partial** and confidence is moderate for visible source, limited for actual host behavior. Project code, host tools, providers, independently downloaded installers and unbundled companions are excluded.

* The [instructions](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/skills/receiving-code-review/SKILL.md#L205) direct replies to GitHub review threads using `gh api`; that can transmit text to an external service. It also directs local changes and tests. Verify feedback, destination and task authorization before sending; avoid disclosing private context.
* Source instructions are task guidance and cannot grant new permissions. Untrusted project content or fetched material can redirect an agent; treat it as data and limit accessible context. Review generated commands and changes before use.

**Risk: high.** The documented GitHub reply can publish information externally. This is not a safety guarantee. Runtime behavior, external integrations, and quality of advice remain unverified.

## Validation

Documented: pinned source installation guidance. Static verification: fetched all item files at the pinned commit, compared their Git blob IDs to local evidence copies, scanned all item files for operational and security terms, inspected the instructions and operation-bearing references and scripts, and observed the upstream branch. The [legacy import report](../../imports/obra-superpowers-receiving-code-review.md) records earlier provenance and its actual scope. No source scripts, installers, project tests, agents, remote actions or examples were executed.
