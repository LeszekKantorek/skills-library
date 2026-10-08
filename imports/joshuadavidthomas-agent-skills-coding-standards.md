---
link: "https://github.com/joshuadavidthomas/agent-skills/tree/516dee7a422b90937b2958d11c03694154ab9c09/coding-standards"
name: "joshuadavidthomas-agent-skills-coding-standards"
sha: "516dee7a422b90937b2958d11c03694154ab9c09"
commit: "https://github.com/joshuadavidthomas/agent-skills/commit/516dee7a422b90937b2958d11c03694154ab9c09"
risk: "medium"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/14 (no comments or special acceptance at review time).
- Original name: `coding-standards`; original frontmatter preserved for accepted packages.
- Snapshot: `516dee7a422b90937b2958d11c03694154ab9c09`; resolved upstream main on 2026-10-08. Downloaded outside automatic skill discovery. The issue's researching-codebases blob URL refers to a directory; resolved to the existing tree without expanding requested scope.

## License review
- License identifier(s): MIT.
- Repository evidence: [MIT LICENSE](https://github.com/joshuadavidthomas/agent-skills/blob/516dee7a422b90937b2958d11c03694154ab9c09/LICENSE), Copyright (c) 2025 Josh Thomas.
- Scope and file-specific exceptions: The package README attributes adapted ideas from dmmulroy/skills. Its repository LICENSE is MIT at [8603380821fee6a77c82639f364ce8fe4f5a92be](https://github.com/dmmulroy/skills/blob/8603380821fee6a77c82639f364ce8fe4f5a92be/LICENSE). The exact source LICENSE is additionally preserved as LICENSE-dmmulroy; its notice says Copyright (c) 2026 Matt Pocock and is not corrected or reassigned. Short attributed quotations and cited concepts do not establish a separate package license.
- Redistribution permissions: MIT permits unchanged redistribution when copyright/permission notice is included; mixed packages retain the additional license scopes described above.
- Required notices and other obligations: preserve all original attribution and applicable license copies; never modify original imported sources or imply endorsement.
- Preserved license/attribution files and compliance actions: Exact upstream repository LICENSE (Josh Thomas) copied to package LICENSE. Exact dmmulroy/skills LICENSE copied to LICENSE-dmmulroy at 8603380821fee6a77c82639f364ce8fe4f5a92be.
- Unresolved questions or blockers: None preventing this import; usage limitations below.

## Findings
- Files inspected: complete 12-file inventory below; README/SKILL, references/templates/agent definitions and scripts included, with operation-bearing content reviewed explicitly. Static scans inspected all file contents. External source content treated only as evidence, never executed as instructions.
- Behavior, permissions, and data flows: Read project code, identify design-level concerns, propose or perform scoped local source refactors, and use project-native tests to verify behavior. The instruction to remove obsolete scaffolding follows understanding the real obligation and preserves contracts. This is limited reversible code editing; there is no arbitrary file-tree deletion command, secret access, data transmission, publishing, or remote service mutation workflow.
- Dependencies: No bundled scripts or executable assets; host language/project-native tests only. All ten local reference files are present. README attributes conceptual adaptation to dmmulroy/skills and a historical gist. Ideas and short attributed quotations are distinguished from wholesale bundled third-party sources.
- Risk rationale and assessment gaps: medium according to the highest applicable documented behavior. Static review covers the original Markdown package, examples, links, and attribution. No example programs or project tests executed; correctness of language-translated examples is not certified.

## Import result
- Source file integrity: All 12 original files copied from pinned Git blobs; all original relative paths and byte sequences preserved. Working-tree, staged and committed blob/mode comparisons are performed against the machine-readable inventory. Additional exact license copies are verified separately. Package-specific -text attributes and core.autocrlf=false prevent conversion.
- Added license/attribution files and their provenance: Exact upstream repository LICENSE (Josh Thomas) copied to package LICENSE. Exact dmmulroy/skills LICENSE copied to LICENSE-dmmulroy at 8603380821fee6a77c82639f364ce8fe4f5a92be.
- Checks performed and limitations: immutable Git snapshot and complete file/mode inventory; UTF-8/frontmatter names; local Markdown links and inline path references; license/attribution scope; static code/behavior and dependency scans; review/catalog consistency. No upstream code or instructions executed. Static review covers the original Markdown package, examples, links, and attribution. No example programs or project tests executed; correctness of language-translated examples is not certified.
- Decision and blockers: Imported unchanged. Medium risk reflects local code edits and project-native validation. No high-risk maintainer acceptance is claimed.

## Original file inventory

| Original relative path | Git mode | SHA-256 |
| --- | --- | --- |
| `README.md` | 100644 | `865af5d9c74e413139e031ee52f925900fc0ad2fe7a5c876de25c2ea0672eed7` |
| `SKILL.md` | 100644 | `5988235deb58e83fb5e8e96ce84bf6b0d36d9eb8276da37901f7ea5b53c21fb6` |
| `references/boundaries.md` | 100644 | `0081d0345d5c768a4a675bfb3f5c7ebbc4a7f15dad4fc54f1cf5b44340a3e49a` |
| `references/complexity.md` | 100644 | `175cd27e37d1c9778b273f13059a34f6dfc94e9fd59a192684daaa678baa2496` |
| `references/domain-modeling.md` | 100644 | `e94fe3ddfc1f310c7bad03c4ce0d01cbbefd9a3ee0db410271379337ac947612` |
| `references/effects.md` | 100644 | `45914d104b082e7cf67d9f859893e136d8e6fb636b7556212c3d64be0e44da42` |
| `references/error-handling.md` | 100644 | `8c76831d2228e3b96c1255da2fa2b9299aa9b1efb14766d3c2b12e4b2eac2c15` |
| `references/maintainability.md` | 100644 | `500e8b6970329d1439a132bb7a4205afb11f93ecbbead2b16b8111425cc25940` |
| `references/modules.md` | 100644 | `d83a4e20e4bdf7a1b7345ab08ccec1aa872294bfd1f7a26e1fb63350141da50b` |
| `references/state.md` | 100644 | `ed91788766886c34a2e7dc71f23f9bc9272ac5bf2d74b16eadd5662bb94b6e19` |
| `references/verification.md` | 100644 | `0597ecdf0178b2d4e74681e4be0c8f252f98e8c8eda45195a0f472ef468c82cd` |
| `references/vocabulary.md` | 100644 | `5562155162be17ad524be5f7803d0a63d17d8be59b542754eae8ecb52a440a5b` |

## Validation evidence

- Working-tree and staged verification passed for 88 total files across both imported packages: 85 original files and 3 separately recorded exact MIT notice copies. Imported Git modes are all 100644 and match the source snapshot.
- Original local Markdown links resolve; accepted frontmatter names, catalog direct installation URLs and review-only exclusion passed.
- git diff --cached --check reports three upstream trailing-whitespace lines (two Markdown hard breaks and one Rust example line). They are intentionally retained byte-for-byte; no source whitespace repair is permitted.
