# asd-ste100

## Identity and versions

* Identifier: `danyuchn-asd-ste100-skill-asd-ste100`; author: danyuchn; type: skill, version `0.4.0`. Assessed scope: [repository root](https://github.com/danyuchn/asd-ste100-skill/tree/32511c6992ecb5f1971e46a2943f2e6adceedafe) and its seven tracked files.
* Catalog analysis: [32511c6992ecb5f1971e46a2943f2e6adceedafe](https://github.com/danyuchn/asd-ste100-skill/commit/32511c6992ecb5f1971e46a2943f2e6adceedafe), 2026-11-07.
* Latest observed: [f38838aee0504fae07ef057667182a7c5af4ffe6](https://github.com/danyuchn/asd-ste100-skill/commit/f38838aee0504fae07ef057667182a7c5af4ffe6), `master`, observed 2026-11-07 via the [branch API](https://api.github.com/repos/danyuchn/asd-ste100-skill/branches/master). The [pinned tree](https://api.github.com/repos/danyuchn/asd-ste100-skill/git/trees/32511c6992ecb5f1971e46a2943f2e6adceedafe?recursive=1) and [observed tree](https://api.github.com/repos/danyuchn/asd-ste100-skill/git/trees/f38838aee0504fae07ef057667182a7c5af4ffe6?recursive=1) differ: the root package changed from seven to nine tracked files. The newer head was not assessed.
* Security assessment: `32511c6992ecb5f1971e46a2943f2e6adceedafe`, 2026-11-07; operational risk: medium; completeness: partial.

## Purpose and contents

The [skill](https://github.com/danyuchn/asd-ste100-skill/blob/32511c6992ecb5f1971e46a2943f2e6adceedafe/SKILL.md) rewrites English for readers who must parse instructions without clarification. It is intended for technical instructions and agent-facing text, not creative or marketing writing. Its claims and outputs do not establish formal STE compliance or preservation of meaning.

The root has one skill, README, MIT license, two example files, one writing-rule reference and one Python linter. No item-local hooks, agents, MCP configuration or bundled third-party runtime dependencies were identified. The optional linter needs Python 3 and standard-library modules; examples include linter fixtures. The separately downloaded installer is outside the item.

## Installation

See the [source installation guidance and caution](README.md#installation). Installation was not executed.

## License

The pinned [MIT license](https://github.com/danyuchn/asd-ste100-skill/blob/32511c6992ecb5f1971e46a2943f2e6adceedafe/LICENSE) covers the supplied repository material, copyright 2026 Dustin Yuchen Teng. It requires retaining the copyright and permission notices and disclaims warranties. The [skill](https://github.com/danyuchn/asd-ste100-skill/blob/32511c6992ecb5f1971e46a2943f2e6adceedafe/SKILL.md) excludes the official ASD dictionary; rights in the separately published standard and dictionary are not assessed or granted by this repository.

## Security

Static assessment covers all seven root files, including [linter source](https://github.com/danyuchn/asd-ste100-skill/blob/32511c6992ecb5f1971e46a2943f2e6adceedafe/scripts/ste-lint.py), and the source installation example at `32511c6992ecb5f1971e46a2943f2e6adceedafe`, 2026-11-07. Completeness is **partial** and confidence is moderate for visible code, limited for runtime behavior. The host, Python interpreter, separately fetched installer and official standard are outside scope.

* The linter reads stdin or explicitly supplied UTF-8 file paths and prints findings, including matched input text, to stdout. It imports `json`, `re`, and `sys`; no network, subprocess, file-write, deletion or credential lookup appears in the script. Supply only task-authorized inputs and protect captured output.
* Its structural heuristics do not compare source and rewrite or prove preserved meaning. Review conditions, numbers and modality in rewritten text. The installer is independently fetched and its telemetry claim is an upstream statement, not verified behavior.

**Risk: medium.** The optional workflow executes a local script with caller-selected file access. This is not a safety guarantee; runtime behavior and rewrite quality were not tested.

## Validation

Documented: source installation and linter usage. Static verification: fetched all seven pinned files, matched their Git blobs to local evidence, inspected the entire linter and source instructions, and compared pinned and observed trees. The [legacy import report](../../imports/danyuchn-asd-ste100-skill-asd-ste100.md) records earlier provenance and its separate tests; those tests were not repeated here. No upstream instructions, linter, installer or examples were executed in this assessment.
