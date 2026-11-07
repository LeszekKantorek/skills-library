# experiment-design

## Identity and versions

* Identifier: `jurgendn-agent-skills-experiment-design`; author: jurgendn; type: skill. Scope: [skills/research-experimentation/experiment-design](https://github.com/jurgendn/agent-skills/blob/f290312fb6c55a044402e8649afff5c112e660ab/skills/research-experimentation/experiment-design/SKILL.md) in [the repository](https://github.com/jurgendn/agent-skills), 3 tracked files.
* Catalog analysis: [f290312fb6c55a044402e8649afff5c112e660ab](https://github.com/jurgendn/agent-skills/commit/f290312fb6c55a044402e8649afff5c112e660ab), 2026-11-07; inventory in the [pinned tree](https://api.github.com/repos/jurgendn/agent-skills/git/trees/f290312fb6c55a044402e8649afff5c112e660ab?recursive=1).
* Latest observed: [f290312fb6c55a044402e8649afff5c112e660ab](https://github.com/jurgendn/agent-skills/commit/f290312fb6c55a044402e8649afff5c112e660ab), `main`, observed 2026-11-07 via the [branch API](https://api.github.com/repos/jurgendn/agent-skills/branches/main). The head equals the analyzed commit; the item is unchanged at the observed head.
* Security assessment: `f290312fb6c55a044402e8649afff5c112e660ab`, 2026-11-07; operational risk: medium; completeness: partial.

## Purpose and contents

The [skill](https://github.com/jurgendn/agent-skills/blob/f290312fb6c55a044402e8649afff5c112e660ab/skills/research-experimentation/experiment-design/SKILL.md) addresses experiment design and scaling-law fitting. It is intended for researchers planning controlled experiments and interpreting training runs, and is less suitable for numerically validated scaling predictions. Scientific correctness and task-specific outcomes were not validated.

Skill, Markdown checklist and Python script. The separately supplied NumPy and SciPy versions are unknown; the script contains a self-test that was not run. Installation and later use are separate. No upstream installer or tests were run.

## Installation

See the [source installation guidance and license caution](README.md#installation). The separately obtained installer is outside this assessment.

## License

No LICENSE or COPYING path was found in the complete [pinned repository tree](https://api.github.com/repos/jurgendn/agent-skills/git/trees/f290312fb6c55a044402e8649afff5c112e660ab?recursive=1), and no grant was identified in the inspected item or README. The earlier [legacy review](../../imports/jurgendn-agent-skills-experiment-design.md#license-review) records a broader license-term search. No redistribution permission is established; the earlier maintainer decision to import is provenance, not evidence of a grant. Check rights before copying or installation.

## Security

Static assessment covers the 3 pinned item files and the documented source installation route at `f290312fb6c55a044402e8649afff5c112e660ab`, 2026-11-07. Completeness is **partial** and confidence is moderate for visible instructions, limited for runtime behavior. Host, external packages, project code, data, installers and providers are excluded.

* The [workflow](https://github.com/jurgendn/agent-skills/blob/f290312fb6c55a044402e8649afff5c112e660ab/skills/research-experimentation/experiment-design/SKILL.md#L46) recommends training sanity checks and an optional [scaling fitter](https://github.com/jurgendn/agent-skills/blob/f290312fb6c55a044402e8649afff5c112e660ab/skills/research-experimentation/experiment-design/scripts/fit_scaling_law.py). The script reads command-line arrays or a caller-selected JSON file, imports NumPy and SciPy, and prints a report; no network, subprocess, file write or deletion was identified. Fitting and extrapolation can be unreliable for sparse or unsuitable data; scientific and numerical accuracy were not tested.
* Source instructions grant no additional permissions. Treat untrusted inputs as data and review proposed commands or changes before use.

**Risk: medium.** The optional local Python fitter and suggested experiments use execution and compute. This rating does not resolve licensing or guarantee safety. Runtime behavior and research accuracy remain unverified.

## Validation

Documented: pinned README installation example. Static verification: fetched all item files, matched their Git blobs to local evidence, inspected instructions and references and the full Python script, and observed the upstream branch. The [legacy import report](../../imports/jurgendn-agent-skills-experiment-design.md) records earlier provenance and assessment scope. No upstream code, installers, self-tests, training or examples were executed.
