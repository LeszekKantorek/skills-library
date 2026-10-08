# Issue #12 source mapping

The 15 submitted URLs resolve to 14 unique packages at commit `ae0fd62485d071437ae5e6c4036c986b0dd122a0`. The broad Rust category is not a fifteenth skill.

| Requested source path | Result | Review |
| --- | --- | --- |
| [skills/workflow/rust-code-review](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/workflow/rust-code-review) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-rust-code-review](rewrite-rs-skills-rust-code-review.md) |
| [skills/workflow/rust-testing](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/workflow/rust-testing) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-rust-testing](rewrite-rs-skills-rust-testing.md) |
| [skills/rust](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust) | Category README; eleven child packages listed separately below; deduplicated | Individual child reviews below |
| [skills/rust/async-rust](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/async-rust) | Held: cancellation correctness | [rewrite-rs-skills-async-rust](rewrite-rs-skills-async-rust.md) |
| [skills/rust/idiomatic-rust](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/idiomatic-rust) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-idiomatic-rust](rewrite-rs-skills-idiomatic-rust.md) |
| [skills/rust/ownership-not-clone](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/ownership-not-clone) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-ownership-not-clone](rewrite-rs-skills-ownership-not-clone.md) |
| [skills/rust/rust-api-design](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/rust-api-design) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-rust-api-design](rewrite-rs-skills-rust-api-design.md) |
| [skills/rust/rust-concurrency](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/rust-concurrency) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-rust-concurrency](rewrite-rs-skills-rust-concurrency.md) |
| [skills/rust/rust-docs](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/rust-docs) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-rust-docs](rewrite-rs-skills-rust-docs.md) |
| [skills/rust/rust-errors](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/rust-errors) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-rust-errors](rewrite-rs-skills-rust-errors.md) |
| [skills/rust/rust-observability](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/rust-observability) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-rust-observability](rewrite-rs-skills-rust-observability.md) |
| [skills/rust/rust-performance](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/rust-performance) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-rust-performance](rewrite-rs-skills-rust-performance.md) |
| [skills/rust/type-driven-design](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/type-driven-design) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-type-driven-design](rewrite-rs-skills-type-driven-design.md) |
| [skills/rust/unsafe-rust](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/rust/unsafe-rust) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-unsafe-rust](rewrite-rs-skills-unsafe-rust.md) |
| [skills/misc/rust-supply-chain](https://github.com/rewrite-rs/skills/tree/ae0fd62485d071437ae5e6c4036c986b0dd122a0/skills/misc/rust-supply-chain) | Imported unchanged, medium, BSD-3-Clause | [rewrite-rs-skills-rust-supply-chain](rewrite-rs-skills-rust-supply-chain.md) |

The supply-chain URL was supplied with `/blob/main/` but names a directory. The pinned Git tree contains its SKILL.md, DENY.md and agents/openai.yaml, making the package identity unambiguous.

No umbrella `skills/rewrite-rs-skills-rust/` package is created. All eleven children were assessed individually; ten are imported and async-rust remains outside skills/ and the catalog.

13 imports: 43 original files + 13 exact root LICENSE copies. Complete byte comparison, upstream/staged/committed Git blob identity and mode 100644 inventory verification passed. No skill was installed or executed.

The held result is recorded independently of license permission. Review acceptance or corrected upstream sources is required for async-rust; merging this PR preserves the recorded hold rather than importing that package.
