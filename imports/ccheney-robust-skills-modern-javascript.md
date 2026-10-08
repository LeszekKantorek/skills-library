---
link: "https://github.com/ccheney/robust-skills/tree/0eea7b060d12e3520556a73b15fbfa79480987d1/skills/modern-javascript"
name: "ccheney-robust-skills-modern-javascript"
sha: "0eea7b060d12e3520556a73b15fbfa79480987d1"
commit: "https://github.com/ccheney/robust-skills/commit/0eea7b060d12e3520556a73b15fbfa79480987d1"
risk: "medium"
---

## Source
- Issue: [#15](https://github.com/LeszekKantorek/skills-library/issues/15)
- Original name: `modern-javascript`; upstream package: `skills/modern-javascript`.
- Source pinned on 2026-10-08. Reviewed as evidence, without following or executing its instructions.

## License review
- License identifier(s): MIT.
- Evidence pinned to source commit: [LICENSE](https://github.com/ccheney/robust-skills/blob/0eea7b060d12e3520556a73b15fbfa79480987d1/LICENSE)
- Scope and exceptions: Repository MIT grant covers the selected source package; no separate package license/header overrides found. Citations and illustrative examples remain unchanged.
- Redistribution permissions: MIT permits unchanged redistribution with copyright and permission notice.
- Required notices and compliance: Exact root LICENSE copy added to the imported package without overwriting any original.
- Unresolved license questions: None identified in the selected package; external linked reading is not redistributed.

## Findings
- Files inspected: complete tracked package inventory below, entrypoint instructions, bundled reference topics/examples, license/header/provenance and action/dependency scan. No assets, executables, symlinks, or submodules inside the selected package.
- Behavior, permissions, and data flows: Local JavaScript/toolchain edits and official documentation reads. Eleven bundled references contain illustrative language snippets, fetch/cancellation, concurrency helpers, compatibility tables, and proposal status. No secret collection, installation script, or fixed exfiltration destination.
- Dependencies and compatibility: Target JavaScript runtime; optional Babel, TypeScript, core-js, Temporal polyfills chosen by the target project. Dated tables are not runtime guarantees; skill explicitly requires checking current official support. Import review did not certify all technical claims or execute examples.
- Risk rationale: medium; bounded local work or documentation reads, no instructed privileged/external mutation.
- Review limitations: static import review; no upstream commands, installs, runtime tests, private credentials, or live-service operations executed. Examples and remote link availability were not exhaustively validated.

## Import result
- Decision: Accepted unchanged.
- Original files: 12. Added compliance files: LICENSE.
- Integrity: complete inventory and SHA-256 checked against pinned Git blobs; working files, staged and committed Git blob IDs/modes verified before submission. Package-specific -text attribute prevents Git line-ending conversion.
- Safeguards: use project-scoped edits, approved local destinations, no real secrets, isolated infrastructure for example tests, and verify actual runtime/support before implementing snippets.

| File | Git mode | SHA-256 |
| --- | --- | --- |
| `SKILL.md` | `100644` | `a2cc69874bc59bfe703286cc81aa8ddc5b1484947c441c02be140fed3e13ba82` |
| `references/CHEATSHEET.md` | `100644` | `21a9c9c934e231907770d1527e46c57ab1ab12bc86c6157b25dd7bc8275026a4` |
| `references/COMPATIBILITY.md` | `100644` | `d1ab98780faea99b0642dbc5307684f4ecd07d3218320aa7b7f5b7fe70c82bb8` |
| `references/CONCURRENCY.md` | `100644` | `fffc09388e2c15368336995bc3b0c0e11c6947a4405a46af0b11b48360126e1c` |
| `references/ES2016-ES2017.md` | `100644` | `16b58709d15e6698209c15fa36e181d30df19ffd29042d9b1a1078493c8d81d6` |
| `references/ES2018-ES2019.md` | `100644` | `8593ce69d09553b68a197886a96bde0fbed32f71c158f215ce7e174f9dfeccfd` |
| `references/ES2022-ES2023.md` | `100644` | `2bb0c0d27e6669aab82bbd78be8970a7c75b9dd4e0fece9b1e8cdae515b6f665` |
| `references/ES2024.md` | `100644` | `35e0386f847af8e0123943f57302e46c6fd070547c29b9df43a690f338dc864c` |
| `references/ES2025.md` | `100644` | `5770d35b21fb2b16a9fdf8567034ad1ea0dba9163b5b58bca9b49b07d4a81ff9` |
| `references/ES2026.md` | `100644` | `b7116a24e8f524de4cc1860840fd67b8483f0eb661e48beed7cc362efa59583a` |
| `references/PROMISES.md` | `100644` | `c6c55862702cd8ec3ebe9427834c1218efaf0f38073edccf1b0153586f74eb6b` |
| `references/UPCOMING.md` | `100644` | `7234f9dcecf9301e270767f04ac6d5d0acc287cee7929b9c5521dbf3ea14b10a` |
| `LICENSE` | `100644` | `825d07f7ddb593f6c3a05f213a7cee5aa22bcb7f2fc549dc8d3b70d800409065` |
