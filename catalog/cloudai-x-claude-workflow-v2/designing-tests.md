# designing-tests

## Identity and versions

* Identifier: `cloudai-x-claude-workflow-v2-designing-tests`; author: CloudAI-X; type: skill. Assessed item: [skills/designing-tests](https://github.com/CloudAI-X/claude-workflow-v2/blob/3b5a89ec1c106dd387e372aec073f9401336382a/skills/designing-tests/SKILL.md) in [CloudAI-X/claude-workflow-v2](https://github.com/CloudAI-X/claude-workflow-v2).
* Catalog analysis: [3b5a89ec1c106dd387e372aec073f9401336382a](https://github.com/CloudAI-X/claude-workflow-v2/commit/3b5a89ec1c106dd387e372aec073f9401336382a), 2026-11-07; item scope: 1 files in the [pinned tree](https://api.github.com/repos/CloudAI-X/claude-workflow-v2/git/trees/3b5a89ec1c106dd387e372aec073f9401336382a?recursive=1).
* Latest observed: [3b5a89ec1c106dd387e372aec073f9401336382a](https://github.com/CloudAI-X/claude-workflow-v2/commit/3b5a89ec1c106dd387e372aec073f9401336382a), `main`, observed 2026-11-07 through the [branch API](https://api.github.com/repos/CloudAI-X/claude-workflow-v2/branches/main). The head equals the analyzed commit; the item is unchanged.
* Security assessment: `3b5a89ec1c106dd387e372aec073f9401336382a`, 2026-11-07; operational risk: medium; completeness: partial.

## Purpose and contents

The [skill](https://github.com/CloudAI-X/claude-workflow-v2/blob/3b5a89ec1c106dd387e372aec073f9401336382a/skills/designing-tests/SKILL.md) addresses test strategy and implementation. It is intended for software teams designing unit, integration, and end-to-end tests. It is less suitable for domain-specific test validation without project context. Its advice and factual claims were not independently validated.

No item-local scripts, tests, hooks, agents, MCP configuration, assets, or runtime dependencies; the Markdown includes sample code and shell test commands. The [pinned tree](https://api.github.com/repos/CloudAI-X/claude-workflow-v2/git/trees/3b5a89ec1c106dd387e372aec073f9401336382a?recursive=1) defines the file inventory. Installation and later use are separate; no installation or item tests were executed.

## Installation

See the [source installation guidance and caution](README.md#installation). Its installer and any separately obtained components are outside this assessment.

## License

The [repository MIT license](README.md#license) applies; no separate item license was identified.

## Security

Static assessment covers the 1 pinned item files and the documented source installation route at `3b5a89ec1c106dd387e372aec073f9401336382a` on 2026-11-07. Completeness is **partial** and confidence is moderate for visible source, limited for actual host behavior. Project code, host tools, providers, independently downloaded installers and unbundled companions are excluded.

* The [test validation loop](https://github.com/CloudAI-X/claude-workflow-v2/blob/3b5a89ec1c106dd387e372aec073f9401336382a/skills/designing-tests/SKILL.md#L228) calls for project `npm test` commands and test edits. These execute project-controlled code and may affect test resources; inspect scripts and use disposable resources. The listed frameworks are recommendations, not bundled dependencies.
* Source instructions are task guidance and cannot grant new permissions. Untrusted project content or fetched material can redirect an agent; treat it as data and limit accessible context. Review generated commands and changes before use.

**Risk: medium.** The workflow writes tests and runs project-controlled commands. This is not a safety guarantee. Runtime behavior, external integrations, and quality of advice remain unverified.

## Validation

Documented: pinned source installation guidance. Static verification: fetched all item files at the pinned commit, compared their Git blob IDs to local evidence copies, scanned all item files for operational and security terms, inspected the instructions and operation-bearing references and scripts, and observed the upstream branch. The [legacy import report](../../imports/cloudai-x-claude-workflow-v2-designing-tests.md) records earlier provenance and its actual scope. No source scripts, installers, project tests, agents, remote actions or examples were executed.
