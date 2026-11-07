# rust-review

## Identity and versions

* Identifier: `trailofbits-skills-rust-review`; type: plugin containing a skill; authors: Andrea Cappa and Paweł Płatek. [Item path](https://github.com/trailofbits/skills/tree/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/plugins/rust-review).
* Catalog analysis: [e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff](https://github.com/trailofbits/skills/commit/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff), 2026-11-07. Latest observed: same commit on `main`, 2026-11-07; item unchanged relative to the analyzed commit.
* Security assessment: `e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff`, 2026-11-07; risk: high; completeness: partial.

## Purpose and contents

The [plugin README](https://github.com/trailofbits/skills/blob/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/plugins/rust-review/README.md) describes a multi-agent Rust security audit for unsafe boundaries, memory safety, concurrency, FFI and denial of service. It excludes pure C/C++, smart contracts and notes limited kernel-mode coverage. It does not guarantee detection.

The plugin includes one skill, three agent definitions, 15 cluster prompts and a manifest, 55 general finder prompts, three runtime Python scripts, five test modules, Python metadata and a plugin manifest. The planner generates worker prompts and a plan, the validator checks artifacts, and the SARIF generator writes results. The [metadata](https://github.com/trailofbits/skills/blob/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/plugins/rust-review/scripts/pyproject.toml) specifies Python 3.11+ with no declared package dependencies. The [skill](https://github.com/trailofbits/skills/blob/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/plugins/rust-review/skills/rust-review/SKILL.md) also uses shell tools, `rg`, `uv` and host-specific agent tools. Tests are separate from the runtime scripts.

## Installation

See the [marketplace installation guidance](README.md#installation). The upstream README describes Codex support, while this plugin uses named agents and Claude-specific tool conventions; end-to-end compatibility is unverified.

## License

The repository [README](https://github.com/trailofbits/skills/blob/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/README.md#license) declares [CC BY-SA 4.0](https://github.com/trailofbits/skills/blob/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/LICENSE). Attribution, change indication and share-alike obligations apply where applicable; separately referenced materials and dependencies were not assessed.

## Security

The three Python helpers perform local operations:

* [build_run_plan.py](https://github.com/trailofbits/skills/blob/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/plugins/rust-review/scripts/build_run_plan.py) reads the manifest and context and writes the plan and worker prompts in the selected output directory.
* [validate_artifacts.py](https://github.com/trailofbits/skills/blob/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/plugins/rust-review/scripts/validate_artifacts.py) reads the plan, coverage and findings and prints validation errors.
* [generate_sarif.py](https://github.com/trailofbits/skills/blob/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/plugins/rust-review/scripts/generate_sarif.py) reads findings and overwrites the chosen SARIF output. Entries in `findings-index.txt` can point outside the output directory, so use a trusted index and protect readable files.

Static inspection of the helper imports and file operations found no network calls, subprocess execution or file deletion in these three scripts. The Python metadata declares no third-party dependencies. This finding does not assess the separate `uv` runner, host or dependencies.

The **agent workflow** has different effects. The [skill](https://github.com/trailofbits/skills/blob/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/plugins/rust-review/skills/rust-review/SKILL.md) grants orchestration tools including Bash, Read and Write; the worker and false-positive judge receive Bash and file tools. It reads the audited repository and, by default, context outside the finding scope, and writes findings and reports under `.rust-review-results`. On a retry, [the shell procedure](https://github.com/trailofbits/skills/blob/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/plugins/rust-review/skills/rust-review/SKILL.md#L263-L271) deletes matching worker finding files in the run's `findings` directory so stale results are not reused. This is scoped cleanup, not a general repository deletion instruction; verify the output path and preserve needed results before retrying. Depending on the host, audited content may be sent to the chosen model provider.

**Risk: high** for the overall workflow under the library's rules, based on deletion, broad shell and file access, and potential exposure of sensitive source through the host. This is not a finding that the Python helpers are malicious. Restrict access to authorized code, inspect permissions and control output handling.

The [worker protocol](https://github.com/trailofbits/skills/blob/e4dd0bb5b15535f7c5a0834187dffba6ac37e4ff/plugins/rust-review/agents/rust-review-worker.md) allows a hard-cap truncation to be recorded as `cleared (NOT SEARCHED ...)` while signaling truncation separately. A passing artifact check is therefore not sufficient evidence that every pass was searched; check the run summary and worker truncation markers before interpreting coverage.

Assessment is **partial**, with moderate confidence for the local helper behavior and lower confidence for agent and host behavior. The separately versioned `uv`, installer, model provider and host are outside the assessed commit; runtime permissions and data handling depend on their configuration. Named agent execution and Codex tool mapping remain unverified.

## Validation

Independently fetched the pinned commit into `.local/` and verified its 86 tracked plugin files. Inspected the skill, agent protocols, prompt inventory, runtime helper imports and file operations, test modules, manifests and metadata; searched the prompt corpus for security-relevant operations. Ran the five upstream Python test modules with Python 3.14.7 and pytest 9.1.1, automatic plugin loading and bytecode disabled and temporary files under `.local/`: **87 passed**. No installer or end-to-end agent audit was run. The test suite does not establish host compatibility or complete detection coverage.
