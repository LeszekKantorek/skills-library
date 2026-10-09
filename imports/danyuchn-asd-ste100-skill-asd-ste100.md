---
link: "https://github.com/danyuchn/asd-ste100-skill/tree/32511c6992ecb5f1971e46a2943f2e6adceedafe"
name: "danyuchn-asd-ste100-skill-asd-ste100"
sha: "32511c6992ecb5f1971e46a2943f2e6adceedafe"
commit: "https://github.com/danyuchn/asd-ste100-skill/commit/32511c6992ecb5f1971e46a2943f2e6adceedafe"
risk: "medium"
---

## Source

- Issue: https://github.com/LeszekKantorek/skills-library/issues/20
- Original name: `asd-ste100`, version `0.4.0`; repository-root skill.
- Complete tracked root package: seven files, all mode `100644`; no symlinks or submodules.

## License review

- License identifier: MIT.
- Evidence: [LICENSE](https://github.com/danyuchn/asd-ste100-skill/blob/32511c6992ecb5f1971e46a2943f2e6adceedafe/LICENSE), copyright (c) 2026 Dustin Yuchen Teng; [README license declaration](https://github.com/danyuchn/asd-ste100-skill/blob/32511c6992ecb5f1971e46a2943f2e6adceedafe/README.md).
- Scope and file-specific exceptions: repository-wide MIT terms cover the seven tracked files. No separate file license or bundled third-party dependency was found. The writing-rule reference and example introductions describe their content as paraphrases, with source links.
- Redistribution permissions: MIT permits redistribution of the unchanged package in a differently named containing directory.
- Required notices and obligations: retain the copyright and permission notice. No source-sharing or change-notice requirement applies to this unchanged import.
- Preserved files and compliance actions: original root `LICENSE` retained byte-for-byte. No extra license files were needed.
- ASD's official standard and dictionary have separate redistribution restrictions. They are not bundled. The skill explicitly excludes the official dictionary; source links do not grant permission to redistribute it. This review covers the supplied paraphrases and code, not future copies of the official standard.
- Unresolved questions or blockers: none identified in the supplied package. This is a source-license review, not a certification of STE compliance.

## Findings

- Files inspected: `LICENSE`, `README.md`, `SKILL.md`, `examples/before-after.md`, `examples/linter-edge-cases.md`, `references/writing-rules.md`, and all of `scripts/ste-lint.py`.
- Behavior and data flows: rewrite user-supplied English while retaining conditions and uncertainty. The optional linter reads stdin or explicitly supplied UTF-8 file paths and prints findings to stdout. It imports only `json`, `re`, and `sys`. No network API, subprocess execution, environment/credential lookup, file write, deletion, or remote publication appears in the script. It can read any file explicitly passed by its caller, so use only task-authorized inputs and treat stdout as containing excerpts of those inputs.
- README recommends installation through `npx skills` or Git clone; the CLI is an external executable and its telemetry statement is an upstream claim, not verified here. Neither installer was run. Use the library's direct package URL from the catalog. External documentation links are reading resources, not instructions to execute.
- Dependencies: Python 3 with standard library for optional linting; no other skill dependency or missing local resource. Python 3.14.7 was used for checks. No package installation is necessary for the linter.
- Risk: medium because the skill recommends executing a transparent local script and installer commands. Its normal rewrite workflow and linter do not require secrets, transmission, destructive actions, or broader permissions. No malicious override or bypass instruction was found.
- Limitations: regex heuristics do not verify the official ASD vocabulary, semantic equivalence, noun clusters, or complete Markdown syntax. The sentence check uses a 25-word cap and cannot distinguish the 20-word procedural cap. The intentionally invalid fixture should fail. Examples C and D illustrate additions or stronger claims than the source text; C acknowledges an added check, while D's storage claim is not established by its input. Review rewrites for factual and modality preservation regardless of lint results. No original example was repaired.
- Compatibility: preserve frontmatter name `asd-ste100`. The upstream README retains upstream installation URLs. No duplicate original name or missing package-local Markdown link was found. External link availability and `npx` installation were not tested.

## Import result

- Decision: accepted for an unchanged import through a PR to `main`; merge remains a maintainer action. No blockers identified.
- Integrity: every imported file was copied from its pinned Git blob, compared byte-for-byte in the working tree, and checked against staged and committed blob IDs and Git modes. Line endings and encodings remain upstream bytes. Git operations use `core.autocrlf=false`; committed bytes are verified rather than relying on checkout settings alone.
- Added license/attribution files: none; the original `LICENSE` is part of the source inventory.
- Checks: isolated Python invocation (`-I`), no real secrets or network inputs: upstream `--selftest` passed; the edge-case fixture returned exit 1 with exactly two `dangling-conjunction` findings on lines 7 and 8; clean stdin retained `may have failed` with zero findings and exit 0; bad stdin returned exit 1 with semicolon, phrasal-verb, and passive-voice findings. The README's `--baseline 41 SKILL.md` command returned exit 0, with 41 hard findings. These are structural checks only, not certification or proof of rewrite correctness.
- Local references, frontmatter, original-name uniqueness, catalog/review links, full inventory, and Git file modes were checked. No upstream source file was changed.

| Original path | Git mode | SHA-256 |
| --- | --- | --- |
| `LICENSE` | `100644` | `d3c674e8592076c9021a59b55177adbcba6fd7e1710082becb922522b22ec672` |
| `README.md` | `100644` | `45380a0fb7892b83bbb4fd0aa8b8ae67ea62f095da721d7893a8df4dd3a1cdb6` |
| `SKILL.md` | `100644` | `39940a0db3d185416edfd757eff4c971006d8f59ad39715295b150b552344342` |
| `examples/before-after.md` | `100644` | `d7bf2b4a390f1997a18790b243dd4c0670018d0d4d5183ec8ed44cbbf282bc52` |
| `examples/linter-edge-cases.md` | `100644` | `b6cc08af876014453b0c72d26ee4bfaeed1e9a154b5046947392752911ce1774` |
| `references/writing-rules.md` | `100644` | `4b92c86bf803f9f54e069767d34dc7356fbb95fb52a3f28476093917c608c102` |
| `scripts/ste-lint.py` | `100644` | `1b97b2d22ba50cde10654db56e1b98adf96d250dd3c8f693f8a81361b1084e85` |
