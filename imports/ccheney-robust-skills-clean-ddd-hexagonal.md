---
link: "https://github.com/ccheney/robust-skills/tree/0eea7b060d12e3520556a73b15fbfa79480987d1/skills/clean-ddd-hexagonal"
name: "ccheney-robust-skills-clean-ddd-hexagonal"
sha: "0eea7b060d12e3520556a73b15fbfa79480987d1"
commit: "https://github.com/ccheney/robust-skills/commit/0eea7b060d12e3520556a73b15fbfa79480987d1"
risk: "medium"
---

## Source
- Issue: [#15](https://github.com/LeszekKantorek/skills-library/issues/15)
- Original name: `clean-ddd-hexagonal`; upstream package: `skills/clean-ddd-hexagonal`.
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
- Behavior, permissions, and data flows: Local architecture/code edits and tests. Seven Markdown references include pseudocode and TypeScript examples for repositories, outbox, sagas, ports, layers, and tests. Persistence/deletion/publishing examples describe target application behavior; the skill does not instruct executing them against a live service.
- Dependencies and compatibility: Project language/framework and test stack. Examples mention optional architecture tools (tsarch, ArchUnit, NetArchTest, import-linter) and real-infrastructure integration tests; use isolated test services. Educational examples are not a ready-to-run application.
- Risk rationale: medium; bounded local work or documentation reads, no instructed privileged/external mutation.
- Review limitations: static import review; no upstream commands, installs, runtime tests, private credentials, or live-service operations executed. Examples and remote link availability were not exhaustively validated.

## Import result
- Decision: Accepted unchanged.
- Original files: 8. Added compliance files: LICENSE.
- Integrity: complete inventory and SHA-256 checked against pinned Git blobs; working files, staged and committed Git blob IDs/modes verified before submission. Package-specific -text attribute prevents Git line-ending conversion.
- Safeguards: use project-scoped edits, approved local destinations, no real secrets, isolated infrastructure for example tests, and verify actual runtime/support before implementing snippets.

| File | Git mode | SHA-256 |
| --- | --- | --- |
| `SKILL.md` | `100644` | `6b719ae95e3b770e4c29b88f9088081f497d51030f537434f26a0b294397cb17` |
| `references/CHEATSHEET.md` | `100644` | `e697fb5438d07742d818e615b751860bb39d201121f82c85eb46371990afa7e8` |
| `references/CQRS-EVENTS.md` | `100644` | `8733e780ef7ed4e80c04877321cf98d908021fbe187705580412a5c9627e1c33` |
| `references/DDD-STRATEGIC.md` | `100644` | `52cf8ce1d9d521f327ba74fad877e032a958bd8a74ba6137c88ee43e770414d9` |
| `references/DDD-TACTICAL.md` | `100644` | `0e566789d6797229b76a4a66a78068905f11f919e61888ffcbb24ff0531a9c60` |
| `references/HEXAGONAL.md` | `100644` | `80992d63dc56b16c1ec22ebfe637408b0e9d5840e2fa22c03707752d2b3e23df` |
| `references/LAYERS.md` | `100644` | `7dc3ade71740905ee1e14a68b2d79d6d4f1fa4c18a596d8d31f153060ce4ece5` |
| `references/TESTING.md` | `100644` | `e7cc45eb54e5cd6f77a81ee08c381d4f2ebf853788998583d7ba1f8d68eaa2df` |
| `LICENSE` | `100644` | `825d07f7ddb593f6c3a05f213a7cee5aa22bcb7f2fc549dc8d3b70d800409065` |
