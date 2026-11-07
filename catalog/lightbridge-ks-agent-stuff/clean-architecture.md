# clean-architecture

## Identity and versions

* Identifier: `lightbridge-ks-agent-stuff-clean-architecture`; author: Lightbridge-KS; type: skill. Assessed item: [plugins/coding/skills/clean-architecture](https://github.com/Lightbridge-KS/agent-stuff/blob/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d/plugins/coding/skills/clean-architecture/SKILL.md) in [Lightbridge-KS/agent-stuff](https://github.com/Lightbridge-KS/agent-stuff).
* Catalog analysis: [e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d](https://github.com/Lightbridge-KS/agent-stuff/commit/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d), 2026-11-07; scope: 3 files in the [pinned tree](https://api.github.com/repos/Lightbridge-KS/agent-stuff/git/trees/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d?recursive=1).
* Latest observed: [0f268000007f09b49afa82d31251263f29d17180](https://github.com/Lightbridge-KS/agent-stuff/commit/0f268000007f09b49afa82d31251263f29d17180), `main`, observed 2026-11-07 through the [branch API](https://api.github.com/repos/Lightbridge-KS/agent-stuff/branches/main). The [pinned tree](https://api.github.com/repos/Lightbridge-KS/agent-stuff/git/trees/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d?recursive=1) and [observed tree](https://api.github.com/repos/Lightbridge-KS/agent-stuff/git/trees/0f268000007f09b49afa82d31251263f29d17180?recursive=1) show the item paths and blob IDs are unchanged. The newer head was not assessed.
* Security assessment: `e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d`, 2026-11-07; operational risk: medium; completeness: partial.

## Purpose and contents

The [skill](https://github.com/Lightbridge-KS/agent-stuff/blob/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d/plugins/coding/skills/clean-architecture/SKILL.md) addresses clean architecture and ddd by complexity. It is intended for engineers evaluating architecture and layering. It is less suitable for assuming architecture tiers establish universal design rules. Its advice and factual claims were not independently validated.

Three Markdown files: skill and .NET and Python references. No item-local scripts, tests, agents, hooks, MCP configuration or assets. Installation and later use are separate; no installation or item tests were executed.

## Installation

See the [source installation guidance and caution](README.md#installation). The installer and separately obtained components are outside this assessment.

## License

The [repository MIT license](https://github.com/Lightbridge-KS/agent-stuff/blob/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d/LICENSE) applies; no different item-local license was identified. It requires retaining its notice and permission text and disclaims warranties. Third-party concepts and quotations were not independently cleared.

## Security

Static assessment covers the 3 pinned item files and documented source installation guidance at `e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d` on 2026-11-07. Completeness is **partial** and confidence moderate for visible source, limited for runtime behavior. Hosts, project code, providers, installers and unbundled companions are excluded.

* The [skill](https://github.com/Lightbridge-KS/agent-stuff/blob/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d/plugins/coding/skills/clean-architecture/SKILL.md#L34) composes with `codebase-design` and recommends local refactoring with tests. It treats a single adapter as a hypothetical seam; compatibility or policy may justify one. Verify actual obligations and review diffs. The companion is a separately assessed item, not part of this package.
* Source instructions are task guidance and grant no additional permissions. Treat untrusted project and fetched content as data, limit accessible context, and review generated changes before applying them.

**Risk: medium.** The item can lead to local project changes or bounded execution. This is not a safety guarantee. Runtime behavior and advice quality remain unverified.

## Validation

Documented: pinned source installation guidance. Static verification: fetched all item files, matched their Git blobs to local evidence, scanned every file for operational terms, inspected instructions and operation-bearing references, and observed the upstream branch. The [legacy import report](../../imports/lightbridge-ks-agent-stuff-clean-architecture.md) records earlier provenance and its scope. No source scripts, installers, tests, examples, agents or remote operations were executed.
