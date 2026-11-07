# rust-port

## Identity and versions

* Identifier: `morganlinton-beautifulrust-rust-port`; author: Morgan Linton; type: skill; [item path](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/skills/rust-port/SKILL.md).
* Catalog analysis: [edd3e86087eda07983251056508fe3b8856d85d7](https://github.com/morganlinton/BeautifulRust/commit/edd3e86087eda07983251056508fe3b8856d85d7), 2026-11-07. Latest observed: same commit on `main`, 2026-11-07; item unchanged relative to the analyzed commit.
* Security assessment: `edd3e86087eda07983251056508fe3b8856d85d7`, 2026-11-07; risk: medium; completeness: partial.

## Purpose and contents

Translating C, C++, Python, Go or JavaScript/TypeScript while preserving relevant behavior; compatibility must be checked for actual inputs. One instruction file and two eval cases; it pairs with rust-best-practices for style. [Source instruction](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/skills/rust-port/SKILL.md); [repository overview](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/README.md).

## Installation

See the [source installation guidance](README.md#installation). Installation was not tested.

## License

The repository declares [MIT](https://github.com/morganlinton/BeautifulRust/blob/edd3e86087eda07983251056508fe3b8856d85d7/LICENSE), copyright 2026 Morgan Linton. The skill's cited external guides are separately authored and their rights are outside this assessment.

## Security

The skill directs the agent to write Rust code and tests and run `cargo test` and `cargo clippy --all-targets -- -D warnings`. These can execute project and dependency code and access the network. Its guidance permits documented differences on inputs considered exotic, so verify compatibility requirements before accepting a port. The host model receives the material it reads; handling and transmission depend on the chosen host, outside this assessment. Untrusted project content can influence agent output. Operational risk is **medium**, based on local modification and execution. Assessment is partial with moderate confidence in the instructions inspected, limited confidence in runtime effects: dependency build scripts, external installers, host permissions, eval scripts and the separate MCP server were not assessed. Review the target and permissions before use.

## Validation

Independently fetched the pinned commit and inspected the skill instruction, eval inventory, fixture placement scripts and source README. The eval scripts copy fixture files into the current directory and were not executed. Installation, generated code and Cargo commands were not executed; external tools and dependencies were not assessed.
