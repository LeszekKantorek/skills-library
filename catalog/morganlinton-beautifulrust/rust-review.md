# rust-review

## Identity and versions

* Identifier: `morganlinton-beautifulrust-rust-review`; author: Morgan Linton; type: skill; [item path](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/skills/rust-review/SKILL.md).
* Catalog analysis: [edd3e86087eda07983251056508fe3b8856d85d7](https://github.com/morganlinton/BeautifulRust/commit/edd3e86087eda07983251056508fe3b8856d85d7), 2026-11-07. Latest observed: same commit on `main`, 2026-11-07; item unchanged relative to the analyzed commit.
* Security assessment: `edd3e86087eda07983251056508fe3b8856d85d7`, 2026-11-07; risk: medium; completeness: partial.

## Purpose and contents

Reviewing a file, crate or diff and producing prioritized, cited findings; its advice is not a substitute for testing or an independent security audit. One instruction file and two eval cases; it optionally consults the best-practices references and recommends the repository lint configuration. [Source instruction](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/skills/rust-review/SKILL.md); [repository overview](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/README.md).

## Installation

See the [source installation guidance](README.md#installation). Installation was not tested.

## License

The repository declares [MIT](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/LICENSE), copyright 2026 Morgan Linton. The skill's cited external guides are separately authored and their rights are outside this assessment.

## Security

The instructions say not to rewrite code without a request, but recommend `cargo fmt --check`, `cargo clippy --all-targets --all-features -- -W clippy::pedantic`, and `cargo test`. Builds and tests can execute project and dependency code and access the network. Restrict execution to trusted projects. The host model receives the material it reads; handling and transmission depend on the chosen host, outside this assessment. Untrusted project content can influence agent output. Operational risk is **medium**, based on local modification and execution. Assessment is partial with moderate confidence in the instructions inspected, limited confidence in runtime effects: dependency build scripts, external installers, host permissions, eval scripts and the separate MCP server were not assessed. Review the target and permissions before use.

## Validation

Independently fetched the pinned commit and inspected the skill instruction, eval inventory, fixture placement scripts and source README. The eval scripts copy fixture files into the current directory and were not executed. Installation, generated code and Cargo commands were not executed; external tools and dependencies were not assessed.
