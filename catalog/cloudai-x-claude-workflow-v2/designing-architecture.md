# designing-architecture

## Identity and versions

* Identifier: `cloudai-x-claude-workflow-v2-designing-architecture`; author: CloudAI-X; type: skill. Scope: [skills/designing-architecture/SKILL.md](https://github.com/CloudAI-X/claude-workflow-v2/blob/3b5a89ec1c106dd387e372aec073f9401336382a/skills/designing-architecture/SKILL.md) in the [repository](https://github.com/CloudAI-X/claude-workflow-v2).
* Catalog analysis: [3b5a89ec1c106dd387e372aec073f9401336382a](https://github.com/CloudAI-X/claude-workflow-v2/commit/3b5a89ec1c106dd387e372aec073f9401336382a), 2026-11-07. The file's Git blob is `e54dc3b29b8507f4ae5261f8683b75e8552378f4`.
* Latest observed: [3b5a89ec1c106dd387e372aec073f9401336382a](https://github.com/CloudAI-X/claude-workflow-v2/commit/3b5a89ec1c106dd387e372aec073f9401336382a), `main`, observed 2026-11-07 through the [branch API](https://api.github.com/repos/CloudAI-X/claude-workflow-v2/branches/main). The head equals the analyzed commit, so the item is unchanged at the observed head.
* Security assessment: `3b5a89ec1c106dd387e372aec073f9401336382a`, 2026-11-07; operational risk: medium; completeness: partial.

## Purpose and contents

The [skill](https://github.com/CloudAI-X/claude-workflow-v2/blob/3b5a89ec1c106dd387e372aec073f9401336382a/skills/designing-architecture/SKILL.md) guides software architects through selecting patterns, defining directory structure, documenting trade-offs, and validating decisions. It is intended for software teams designing systems or project structure, and is less suitable for small changes that do not affect architecture. Its size-based recommendations are heuristics; their applicability and technical accuracy were not validated.

The pinned [recursive tree](https://api.github.com/repos/CloudAI-X/claude-workflow-v2/git/trees/3b5a89ec1c106dd387e372aec073f9401336382a?recursive=1) contains one Markdown instruction file in this item directory. It includes the prompt, checklists, pattern diagrams, example directory structures, and decision template. No item-local scripts, tests, agents, hooks, MCP configuration, assets, or dependencies are present. The broader plugin and its components are outside this item scope.

## Installation

See the [source installation guidance and caution](README.md#installation). The documented command selects a moving repository and uses a separately versioned installer that was not assessed.

## License

The [repository MIT license](README.md#license) applies to the item. The pinned tree contains no item-specific license, and no differing notice was identified in the skill.

## Security

The static assessment covers the pinned item, its tree, and the repository README's skills installation guidance at commit `3b5a89ec1c106dd387e372aec073f9401336382a` on 2026-11-07. Completeness is **partial** and confidence moderate for the visible instructions, limited for runtime behavior. The host, separately downloaded installer, and other plugin components are unassessed.

* The [workflow](https://github.com/CloudAI-X/claude-workflow-v2/blob/3b5a89ec1c106dd387e372aec073f9401336382a/skills/designing-architecture/SKILL.md#L13) calls for architecture selection, directory structure, and documented decisions; it may lead a host to create or modify project files. Review proposed changes before applying them. The prompt declares no tools; host permissions and behavior are unknown.
* No shell commands, fixed network destination, secret collection, destructive instruction, or publication instruction were identified in the item file. The separate README installation command obtains an independently versioned installer and selects a moving source. Its selection behavior and effects were not tested.

**Risk: medium.** Project scaffolding and decision documentation can lead to local writes; this is an assessment of the visible workflow, not a guarantee of safety. Review the prompt and project changes, and validate design choices against the project's constraints.

## Validation

Documented: the pinned README's installation example. Static verification: retrieved the complete item independently through GitHub contents and raw endpoints and compared the responses; inspected the pinned tree, README, license, and observed branch. The [legacy import report](../../imports/cloudai-x-claude-workflow-v2-designing-architecture.md) records the earlier import and its scope. No upstream instructions, installer, plugin, or domain-quality tests were executed; runtime behavior remains unverified.
