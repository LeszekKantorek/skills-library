---
link: "https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/async-rust"
name: "rewrite-rs-skills-async-rust"
sha: "ae0fd62485d071437ae5e6c4036c986b0dd122a0"
commit: "https://github.com/rewrite-rs/skills/commit/ae0fd62485d071437ae5e6c4036c986b0dd122a0"
risk: "high"
---

## Source
- Issue: [#12](https://github.com/LeszekKantorek/skills-library/issues/12).
- Original name: `async-rust`; complete package at `skills/rust/async-rust`.
- Snapshot: immutable Git commit above, obtained outside automatic skill discovery. The `skills/rust` link is a category README, not a skill; its eleven children exactly match the eleven individually requested Rust packages. No duplicate umbrella import is created. The issue's `blob/main/skills/misc/rust-supply-chain` points at a directory; its tracked package resolves unambiguously at the pinned commit.

## License review
- License identifier: BSD-3-Clause.
- Evidence: [repository LICENSE](https://github.com/rewrite-rs/skills/blob/ae0fd62485d071437ae5e6c4036c986b0dd122a0/LICENSE), copyright (c) 2026-Present, rewrite.rs.
- Scope: repository license covers all 3 package files. Package inventory contains Markdown guidance/examples and OpenAI interface YAML only; no separate skill license, copyright override, third-party vendored executable, asset or notice found.
- Redistribution: unchanged source redistribution permitted with copyright, conditions and disclaimer retained; no endorsement using holder/contributor names without permission. No source-sharing obligation or change notice applies to these unchanged copies.
- Compliance: no source copied because import is held; the BSD permission is verified independently of the technical blocker.
- Unresolved license questions: none found in this pinned snapshot.

## Findings
- Files inspected: `CANCELLATION.md`, `SKILL.md`, `agents/openai.yaml`; repository LICENSE, README and Rust category README.
- Behavior: Runtimes, Send bounds, cancellation safety, and blocking work. Recommended agent actions include reading target Rust source/configuration and running Cargo checks/tests; design/testing skills may make reversible project edits. Cargo may compile target dependencies/build scripts, read registries, and write local build/cache files. Run only in a trusted or restricted target project without real credentials. No bundled executable, symlink, hidden process, secret collection, publishing, service configuration, or safeguard override found.
- Dependencies: target Rust/Cargo toolchain and the tools/crates described in the original Markdown. No toolchain/dependency was installed and no source example was executed during this import review.
- Companion Markdown and agents/openai.yaml are present; interface metadata names match. Slash-name deferrals are retained: `/ownership-not-clone`, `/rust-api-design`, `/rust-errors`, `/unsafe-rust`. These are original harness invocations, not rewritten library slugs. Install/select companion skills explicitly; auto-routing depends on harness support. Optional port/FFI/CI skills outside #12 were not imported. `async-rust` is held in this PR, so its optional deferrals remain unavailable; core guidance in other packages can be used unchanged, but report a deferred check as not performed rather than claiming complete coverage.
- Risk rationale: high because central cancellation guidance conflicts with documented runtime semantics and may lead to uncontrolled background effects/data loss; material technical concern is documented below.
- Assessment limits: static review of every tracked package file; examples are instructional fragments and were not compiled. This is not a correctness certification of all Rust advice or a security audit of consumers and future dependencies.

## Import result
- Decision: held; no skills directory or catalog row added. License eligible, technical correctness unresolved.
- `CANCELLATION.md` says dropping JoinHandle aborts its task. [Tokio 1.48.0 primary documentation](https://docs.rs/tokio/1.48.0/tokio/task/struct.JoinHandle.html) says dropping it detaches the task and it continues in the background. This directly compromises the skill's core cancellation/shutdown advice.
- The purported safe queue example sends `item` into `process(item)` and then reuses it in the shutdown arm. For an owning non-Copy argument it does not preserve the item; [Rust E0382 documentation](https://doc.rust-lang.org/error_codes/E0382.html) explains use-after-move rejection. The fragment omits signatures, so borrow/Copy alternatives could compile, but its claimed generic ownership repair is unsupported as written.
- Safeguards needed: corrected immutable upstream cancellation guidance, then fresh review; alternatively explicit maintainer acceptance of the exact unchanged defects with use restrictions. No acceptance is inferred from the general import request, and no local repair is permitted.
- Integrity/permissions: all three source files inspected as mode 100644; no source import staged or committed.
