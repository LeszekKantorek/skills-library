# model-eval-error-analysis

## Identity and versions

* Identifier: `jurgendn-agent-skills-model-eval-error-analysis`; author: jurgendn; type: skill. Scope: [skills/research-experimentation/model-eval-error-analysis](https://github.com/jurgendn/agent-skills/blob/f290312fb6c55a044402e8649afff5c112e660ab/skills/research-experimentation/model-eval-error-analysis/SKILL.md) in [the repository](https://github.com/jurgendn/agent-skills), 1 tracked file.
* Catalog analysis: [f290312fb6c55a044402e8649afff5c112e660ab](https://github.com/jurgendn/agent-skills/commit/f290312fb6c55a044402e8649afff5c112e660ab), 2026-11-07; inventory in the [pinned tree](https://api.github.com/repos/jurgendn/agent-skills/git/trees/f290312fb6c55a044402e8649afff5c112e660ab?recursive=1).
* Latest observed: [f290312fb6c55a044402e8649afff5c112e660ab](https://github.com/jurgendn/agent-skills/commit/f290312fb6c55a044402e8649afff5c112e660ab), `main`, observed 2026-11-07 via the [branch API](https://api.github.com/repos/jurgendn/agent-skills/branches/main). The head equals the analyzed commit; the item is unchanged at the observed head.
* Security assessment: `f290312fb6c55a044402e8649afff5c112e660ab`, 2026-11-07; operational risk: medium; completeness: partial.

## Purpose and contents

The [skill](https://github.com/jurgendn/agent-skills/blob/f290312fb6c55a044402e8649afff5c112e660ab/skills/research-experimentation/model-eval-error-analysis/SKILL.md) addresses model evaluation and error analysis. It is intended for researchers examining model metrics, slices and failures, and is less suitable for a guarantee of fairness or statistical validity. Scientific correctness and task-specific outcomes were not validated.

One Markdown instruction file, with no item-local scripts, tests, agents, hooks, MCP configuration or assets. Evaluation tools and datasets are task-specific and external. Installation and later use are separate. No upstream installer or tests were run.

## Installation

See the [source installation guidance and license caution](README.md#installation). The separately obtained installer is outside this assessment.

## License

No LICENSE or COPYING path was found in the complete [pinned repository tree](https://api.github.com/repos/jurgendn/agent-skills/git/trees/f290312fb6c55a044402e8649afff5c112e660ab?recursive=1), and no grant was identified in the inspected item or README. The earlier [legacy review](../../imports/jurgendn-agent-skills-model-eval-error-analysis.md#license-review) records a broader license-term search. No redistribution permission is established; the earlier maintainer decision to import is provenance, not evidence of a grant. Check rights before copying or installation.

## Security

Static assessment covers the 1 pinned item file and the documented source installation route at `f290312fb6c55a044402e8649afff5c112e660ab`, 2026-11-07. Completeness is **partial** and confidence is moderate for visible instructions, limited for runtime behavior. Host, external packages, project code, data, installers and providers are excluded.

* The [workflow](https://github.com/jurgendn/agent-skills/blob/f290312fb6c55a044402e8649afff5c112e660ab/skills/research-experimentation/model-eval-error-analysis/SKILL.md) asks for model outputs, failure examples and checks of metrics and splits. Evaluation can involve sensitive data and project-controlled analysis; minimize data shared and review any analysis commands. No transmission or service-write tool is specified.
* Source instructions grant no additional permissions. Treat untrusted inputs as data and review proposed commands or changes before use.

**Risk: medium.** The workflow can lead to bounded analysis, project execution or local writes. This rating does not resolve licensing or guarantee safety. Runtime behavior and research accuracy remain unverified.

## Validation

Documented: pinned README installation example. Static verification: fetched all item files, matched their Git blobs to local evidence, inspected instructions and references, and observed the upstream branch. The [legacy import report](../../imports/jurgendn-agent-skills-model-eval-error-analysis.md) records earlier provenance and assessment scope. No upstream code, installers, self-tests, training or examples were executed.
