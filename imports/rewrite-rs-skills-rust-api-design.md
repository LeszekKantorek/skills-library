---
link: "https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/rust-api-design"
name: "rewrite-rs-skills-rust-api-design"
sha: "ae0fd62485d071437ae5e6c4036c986b0dd122a0"
commit: "https://github.com/rewrite-rs/skills/commit/ae0fd62485d071437ae5e6c4036c986b0dd122a0"
risk: "medium"
---

## Source
- Issue: [#12](https://github.com/LeszekKantorek/skills-library/issues/12).
- Original name: `rust-api-design`; complete package at `skills/rust/rust-api-design`.
- Snapshot: immutable Git commit above, obtained outside automatic skill discovery. The `skills/rust` link is a category README, not a skill; its eleven children exactly match the eleven individually requested Rust packages. No duplicate umbrella import is created. The issue's `blob/main/skills/misc/rust-supply-chain` points at a directory; its tracked package resolves unambiguously at the pinned commit.

## License review
- License identifier: BSD-3-Clause.
- Evidence: [repository LICENSE](https://github.com/rewrite-rs/skills/blob/ae0fd62485d071437ae5e6c4036c986b0dd122a0/LICENSE), copyright (c) 2026-Present, rewrite.rs.
- Scope: repository license covers all 5 package files. Package inventory contains Markdown guidance/examples and OpenAI interface YAML only; no separate skill license, copyright override, third-party vendored executable, asset or notice found.
- Redistribution: unchanged source redistribution permitted with copyright, conditions and disclaimer retained; no endorsement using holder/contributor names without permission. No source-sharing obligation or change notice applies to these unchanged copies.
- Compliance: exact repository LICENSE bytes added as LICENSE; no original file overwritten.
- Unresolved license questions: none found in this pinned snapshot.

## Findings
- Files inspected: `DEPENDENCY-INJECTION.md`, `SEMVER.md`, `SKILL.md`, `SURFACE.md`, `agents/openai.yaml`; repository LICENSE, README and Rust category README.
- Behavior: Public surface, trait design, and semver discipline. Recommended agent actions include reading target Rust source/configuration and running Cargo checks/tests; design/testing skills may make reversible project edits. Cargo may compile target dependencies/build scripts, read registries, and write local build/cache files. Run only in a trusted or restricted target project without real credentials. No bundled executable, symlink, hidden process, secret collection, publishing, service configuration, or safeguard override found.
- Dependencies: target Rust/Cargo toolchain and the tools/crates described in the original Markdown. No toolchain/dependency was installed and no source example was executed during this import review.
- Companion Markdown and agents/openai.yaml are present; interface metadata names match. Slash-name deferrals are retained: `/async-rust`, `/rust-errors`, `/rust-observability`, `/rust-testing`, `/type-driven-design`, `/unsafe-rust`. These are original harness invocations, not rewritten library slugs. Install/select companion skills explicitly; auto-routing depends on harness support. Optional port/FFI/CI skills outside #12 were not imported. `async-rust` is held in this PR, so its optional deferrals remain unavailable; core guidance in other packages can be used unchanged, but report a deferred check as not performed rather than claiming complete coverage.
- Risk rationale: medium for reversible target edits, transparent command recommendations and public network dependency/advisory reads; no private-data transmission or broad destructive permission requested.
- Assessment limits: static review of every tracked package file; examples are instructional fragments and were not compiled. This is not a correctness certification of all Rust advice or a security audit of consumers and future dependencies.

## Import result
- Accepted for unchanged import: 5 original files, original relative paths/frontmatter, plus one exact repository LICENSE copy.
- Source inventory, working files, staged blobs and committed blobs verified byte-for-byte against upstream Git blob identities and SHA-256; all file modes 100644. No executable-bit conversion or line-ending normalization allowed. Package-specific -text attribute preserves future Git checkouts.
- Original data and license are separate entries in the local verification manifest. No root plugin scripts, package manager files or unrelated skill was copied.
- Checks: complete inventory and mode comparison, source/working/staged/committed content checks, frontmatter/interface names, internal Markdown file availability, review/catalog/license consistency and whitespace checks on library-authored metadata. No Cargo build, upstream npm tests or skill behavior execution performed; these Markdown/YAML imports contain no executable package code.
- Installation limitation: original slash deferrals need companion discovery as noted above; install URLs use direct package URLs and preserve original names.
