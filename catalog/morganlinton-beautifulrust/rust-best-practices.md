# rust-best-practices

## Identity and versions

* Identifier: `morganlinton-beautifulrust-rust-best-practices`; author: Morgan Linton; type: skill; [item path](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/skills/rust-best-practices/SKILL.md).
* Catalog analysis: [edd3e86087eda07983251056508fe3b8856d85d7](https://github.com/morganlinton/BeautifulRust/commit/edd3e86087eda07983251056508fe3b8856d85d7), 2026-11-07. Latest observed: same commit on `main`, 2026-11-07; item unchanged relative to the analyzed commit.
* Security assessment: `edd3e86087eda07983251056508fe3b8856d85d7`, 2026-11-07; risk: medium; completeness: partial.

## Purpose and contents

Writing, refactoring and debugging Rust; it is guidance, not proof of correctness. The skill has six reference digests and four eval cases; it points to the separately maintained lint configuration. No item-local runtime script was identified. [Source instruction](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/skills/rust-best-practices/SKILL.md); [repository overview](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/README.md).

## Installation

See the [source installation guidance](README.md#installation). Installation was not tested.

## License

The repository declares [MIT](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/LICENSE), copyright 2026 Morgan Linton. The skill's cited external guides are separately authored and their rights are outside this assessment.

## Security

Requests editing Rust and running `cargo fmt`, `cargo clippy --all-targets --all-features -- -D warnings`, `cargo test` and, for libraries, `cargo doc --no-deps`. Formatting edits files, while build scripts and tests may execute project and dependency code and access the network. Use a trusted project and control execution and dependencies. The host model receives the material it reads; handling and transmission depend on the chosen host, outside this assessment. Untrusted project content can influence agent output. Operational risk is **medium**, based on local modification and execution. Assessment is partial with moderate confidence in the instructions inspected, limited confidence in runtime effects: dependency build scripts, external installers, host permissions, eval scripts and the separate MCP server were not assessed. Review the target and permissions before use.

## Validation

Statically inspected the pinned instruction, source README and file inventory. Eval content, installation, generated code and Cargo commands were not executed; external tools and dependencies were not assessed.
