---
link: "https://github.com/joshuadavidthomas/agent-skills/tree/516dee7a422b90937b2958d11c03694154ab9c09/rust"
name: "joshuadavidthomas-agent-skills-rust"
sha: "516dee7a422b90937b2958d11c03694154ab9c09"
commit: "https://github.com/joshuadavidthomas/agent-skills/commit/516dee7a422b90937b2958d11c03694154ab9c09"
risk: "medium"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/14 (no comments or special acceptance at review time).
- Original name: `rust`; original frontmatter preserved for accepted packages.
- Snapshot: `516dee7a422b90937b2958d11c03694154ab9c09`; resolved upstream main on 2026-10-08. Downloaded outside automatic skill discovery. The issue's researching-codebases blob URL refers to a directory; resolved to the existing tree without expanding requested scope.

## License review
- License identifier(s): MIT.
- Repository evidence: [MIT LICENSE](https://github.com/joshuadavidthomas/agent-skills/blob/516dee7a422b90937b2958d11c03694154ab9c09/LICENSE), Copyright (c) 2025 Josh Thomas.
- Scope and file-specific exceptions: Source references cite authority, books, articles and documentation and contain explanatory summaries and illustrative code; no separately licensed vendored program, book text snapshot, or file-specific copyright grant was found. SPDX-like values inside Cargo.toml examples are example project metadata, not package relicensing. Repository MIT covers the authored skill. Original citations/quotations are preserved.
- Redistribution permissions: MIT permits unchanged redistribution when copyright/permission notice is included; mixed packages retain the additional license scopes described above.
- Required notices and other obligations: preserve all original attribution and applicable license copies; never modify original imported sources or imply endorsement.
- Preserved license/attribution files and compliance actions: Exact upstream repository LICENSE (Josh Thomas) copied to package LICENSE.
- Unresolved questions or blockers: None preventing this import; usage limitations below.

## Findings
- Files inspected: complete 73-file inventory below; SKILL.md, thirteen topic guides and 59 references/ Markdown files included, with operation-bearing content reviewed explicitly. Static scans inspected all file contents. External source content treated only as evidence, never executed as instructions.
- Behavior, permissions, and data flows: Guides local Rust source edits and review, Cargo configuration, dependency/tool installation, tests, snapshots, fuzzing, profiling, and binding generation. Examples include filesystem reads, threading and native-memory APIs. These are visible illustrative project operations, not a bundled executable or automatic transmission workflow. Distinguish atomic memory publication from external publishing. napi pre-publish is packaging preparation; no registry upload command is instructed.
- Dependencies: Markdown only; 73 original files with Rust/TOML/CLI examples. Suggested tools/libraries include Rust/Cargo, rustup/nightly/Miri, Clippy, Tokio, rayon, serde, thiserror/anyhow, proptest, insta/cargo-insta, criterion/divan, cargo-fuzz/nextest, syn/quote/trybuild, cxx, PyO3/maturin, napi-rs, UniFFI and wasm-bindgen. They are task-specific suggestions, not bundled runtime requirements. Local supplementary paths reference/rust-atomics-and-locks, reference/rust-reference, and reference/rust-nomicon are absent; core guide and all directly linked package Markdown remain usable unchanged.
- Risk rationale and assessment gaps: medium according to the highest applicable documented behavior. Every original file was inventoried and statically scanned for behavior, code fences, dependencies, licensing, paths and network destinations; root and operation-bearing references were read in detail. Examples were not compiled or executed. Unsafe/FFI claims and third-party tool versions must be verified for the target project; absence of exhaustive example execution is a stated validation limitation, not a missing dependency blocker.

## Import result
- Source file integrity: All 73 original files copied from pinned Git blobs; all original relative paths and byte sequences preserved. Working-tree, staged and committed blob/mode comparisons are performed against the machine-readable inventory. Additional exact license copies are verified separately. Package-specific -text attributes and core.autocrlf=false prevent conversion.
- Added license/attribution files and their provenance: Exact upstream repository LICENSE (Josh Thomas) copied to package LICENSE.
- Checks performed and limitations: immutable Git snapshot and complete file/mode inventory; UTF-8/frontmatter names; local Markdown links and inline path references; license/attribution scope; static code/behavior and dependency scans; review/catalog consistency. No upstream code or instructions executed. Every original file was inventoried and statically scanned for behavior, code fences, dependencies, licensing, paths and network destinations; root and operation-bearing references were read in detail. Examples were not compiled or executed. Unsafe/FFI claims and third-party tool versions must be verified for the target project; absence of exhaustive example execution is a stated validation limitation, not a missing dependency blocker.
- Decision and blockers: Imported unchanged with optional reference-corpus limitation recorded. Medium risk: transparent local edits and tools; no remote publishing/secret handling capability is bundled. No high-risk acceptance is claimed.

## Original file inventory

| Original relative path | Git mode | SHA-256 |
| --- | --- | --- |
| `SKILL.md` | 100644 | `c1f6492cfb19fd63ceaa973b3c01054977a665026cc1536a41cb19877379e982` |
| `async.md` | 100644 | `a113a17117aaf2e859c969dfb0ddfc20543dcf8384f80a59133c7597e05da6e0` |
| `atomics.md` | 100644 | `2afd898e2c8e8f3626e97b93322a1edcbf9b0874bf262ac991385d47e9114c9e` |
| `error-handling.md` | 100644 | `9a013fd63bf32b7d1dad4ed5fe3fed4e7c0cec8da14622496d005a4223e41a19` |
| `interop.md` | 100644 | `6e0226882802b56fe4e7ccdbb2043452506d48396eeba1b96e1091a0ca753583` |
| `macros.md` | 100644 | `6a039068537b9b902682461fbf55e67d1d712551e3c53899211a2fced75b8059` |
| `ownership.md` | 100644 | `684324a590e44b3a0e24f68bb5a9367965772388265b1db4c91f2764bd516fdd` |
| `performance.md` | 100644 | `dcf22527e189e29a9ca92b69d461de42dc72997fd0a6d23fc309c35864bffb13` |
| `project-structure.md` | 100644 | `757355fddf48016f2c84ba8451fa5f651cf86068db1a5479e7e72638c911dc90` |
| `references/adapters-and-custom-impls.md` | 100644 | `4103e0dbef3bb051632e023cc9c2590d691159cba24b248d055b3ac38a02cf19` |
| `references/allocation-and-data-structures.md` | 100644 | `db49db641d0843d3216eee17a4cf90d0b321c923e1c1231389be521373306121` |
| `references/anyhow-patterns.md` | 100644 | `15e728d2b802d4f466b9ef8d395a0828cab293e2d1dff395a91af1a9846b8969` |
| `references/attributes-cheatsheet.md` | 100644 | `313214b271baef34abcc2d4a3ae8e9e7ee3a30b861ab830f1c83711ab7dab0ef` |
| `references/benchmarking-and-fuzzing.md` | 100644 | `5842d20dc959a43638295f67b4a425aff9a5cbf0436c20ae68d682f640e5c808` |
| `references/blocking-and-bridging.md` | 100644 | `27e2d6299e90cb92f6cc7de93450268da2730f28a988a0cf076fb29501c62c0d` |
| `references/bool-to-enum.md` | 100644 | `2ec502e9f07aef08f0fc4be8fb1c62c35dfe82db7c9590f3069e3da4f5007f83` |
| `references/borrow-by-default.md` | 100644 | `dc031271f8db7d9d8db2ddf18eb3a904a7dcd3b8aa2ea75bf9c5e7abfe994d9c` |
| `references/builder-patterns.md` | 100644 | `ca11adb940d539b6b29b559b747ec022d43d055589b13ab0f04386708c07b8d4` |
| `references/c-ffi.md` | 100644 | `8027a6469765c7c16ad98344057d15462b66a9cf69f74255aa86942b5f6f78c5` |
| `references/channels-and-select.md` | 100644 | `30981aec114d7c15fb50d5126b9649aa4159c7f447d5a32b78e3c1b9f8103571` |
| `references/combinators.md` | 100644 | `c1255cde99da1a8765532995b57f4892724de965160412686e3bb610c779d6d0` |
| `references/cxx.md` | 100644 | `02464db97b461cfd209bdb16e74eb8e5fd0db172d638c1512b8fd0693903f867` |
| `references/designing-error-types.md` | 100644 | `50a4158c6a558e86b0c2a926cf1bf5ee0a759eefc33d7cbbb5f059d13ba08908` |
| `references/dispatch-patterns.md` | 100644 | `2aae48db819a28e0e5c455eac616204708a925cb95d3acee967955cee2343485` |
| `references/enums-as-modeling-tool.md` | 100644 | `83e55aad38608f74e9ddc2b40d1123e989db1f44e045732ee59a24f5d2d0a2bf` |
| `references/exhaustive-matching.md` | 100644 | `c76928eec623252a3c30d274fb11ec44534614c21706e95ac5c0ce1d7ec74e9f` |
| `references/extension-traits.md` | 100644 | `800411f7f2c00e33e26157da5b6908fbb7084f74de954257244b76a6cda4bde4` |
| `references/features-and-unification.md` | 100644 | `bc390bc12f1345e8564648a5c4d1e76f7ed96b3480d79f3e0121c7edaa23fd20` |
| `references/function-signatures.md` | 100644 | `d6f2a0799d45b8d541fc422eb252b504e862ff71f4d944ea2ae13a99b22024c9` |
| `references/getter-setter.md` | 100644 | `381a20e47925f0b4ad9bb0a841e6ac6bff5c95e7c5e31c4f4a51dbb951c83101` |
| `references/impl-namespace.md` | 100644 | `5c187870cb5fdd127691355ceea0914b18971a76fcd4eab078c5e224d4759a29` |
| `references/iterators-over-indexing.md` | 100644 | `4f8b1584a39688c4107c14732341cf6588debe2b1a744172ca56e532e159608f` |
| `references/lifetime-patterns.md` | 100644 | `ac5fc1c86eeaeccc63ee8dc76ddc00486fd9542246863d9746d6f0eb7552cb98` |
| `references/macro_rules-patterns.md` | 100644 | `8269ec87345f1799b7ed01b670e21006054adef8e41e0750058b9c56d1b58f87` |
| `references/miri-and-unsafe-testing.md` | 100644 | `574d989dd2545d4aca287fe6050b4ad8760f7d6ee143b3c0a87fb70f3ddd7683` |
| `references/napi-rs.md` | 100644 | `524f8966ffa26301893c33cecdd1122ae84e87644cb62ae9c26febff455c961d` |
| `references/newtype-patterns.md` | 100644 | `7fa12d0d80944990d7cabb38f743f9b4f4795b95ef4d071edd674ef486a41d06` |
| `references/newtypes-and-domain-types.md` | 100644 | `e922d644b851f2da8d40700990449fda93f7a449e120efe4905dbe4c4fc83ac1` |
| `references/option-bool-to-enum.md` | 100644 | `43add25c8a3eeeca19834e8c7106a1e97e892491ee7c3be2d2687e0647693461` |
| `references/option-over-sentinels.md` | 100644 | `50bc9d91043332b8a12fc07954e589c5c9d07c4c77150c0a4f8e38696fd14850` |
| `references/ordering-cheatsheet.md` | 100644 | `483eda75ddae1dbc0c2c71b312498bc8ab5d0d6be653abc2845a51ceda7997c7` |
| `references/ownership-before-refcell.md` | 100644 | `190776bf0d1e07df3b745b06b574c1c7678e9014d397fbe95d081f7a5ea62040` |
| `references/ownership-handoff-deadlocks.md` | 100644 | `911bec88fee7e3c547d38ada7ef222e6f9b348b2d5445bce725148361cdbbd61` |
| `references/parse-dont-validate.md` | 100644 | `4b8a5f3c92367b18ec0fd6998b6033005d890e5b1a330bd51e12cacc5a80d3fe` |
| `references/pattern-matching-tools.md` | 100644 | `f149b892462cc823afd966740e0a94ede4d00e4975659bfbda8c81856c75caf1` |
| `references/patterns-from-rust-atomics-and-locks.md` | 100644 | `cd4ef12c723b9ab14c8ca54fbc04a9c79679fd523c47cc7f11e34373db9208b1` |
| `references/proc-macro-patterns.md` | 100644 | `0994b1479ef8e0d89e8427e4fc6adedef81cf2c78a09875d366fa5b9f78a42e5` |
| `references/production-patterns.md` | 100644 | `7c8caa977d01f3753a4ac1f69afe12f0ea54b3e07592b286357f5eb60c6c4428` |
| `references/profiling-and-benchmarking.md` | 100644 | `6d57a70743007e53610cadff6056a4514e252d5a28ba42c1ced03ca5dd367ba0` |
| `references/property-testing.md` | 100644 | `77ca93e8c85be5a0a5d488274e76f555a0fae697c8b1ac7c442b9531b3602157` |
| `references/public-api-surface.md` | 100644 | `2225dca4d3f514433c485444757f14d7125b2c4a3f586e2f5d3e6d59c7cc59be` |
| `references/pyo3.md` | 100644 | `20fc72c078624d816ee1962ac99ac8a151e16352d0335e5ad60d53c616b99ca1` |
| `references/safety-comments-and-unsafe-contracts.md` | 100644 | `ecc6769f93528692c1e0be303e068f3da5b7b32fddcea12be5fe4b72cd021fda` |
| `references/smart-pointers.md` | 100644 | `1a8c3e337b8c033e9352a9517dae19c2b59366d75c2d2212b6b024f8f92c04bd` |
| `references/snapshot-testing.md` | 100644 | `5cd8c1598d953a20da07531e5cbf499cb33b61030841c957140682b708b6262b` |
| `references/standard-traits.md` | 100644 | `0f01714f0531626ac7133166b2f0341a3c97276ad323582fe82ace2526106bb4` |
| `references/struct-collections.md` | 100644 | `54be49b7786188527374c8674f64fcca310a79f99b769d3e12da371cbe1b7d3d` |
| `references/testing-and-debugging-macros.md` | 100644 | `02909b12654bba10091e731efd536d92b528ce8bcabe909051726a702ae443cb` |
| `references/thiserror-patterns.md` | 100644 | `acb23df2b3f5851902eda3d0a0c8cf0fb19e7070a313b18940d1c96e321d31eb` |
| `references/trait-patterns.md` | 100644 | `938f028ae5f60a9b5f6843d38a356f6e281c485c84fe9d450aa0bc71cf591294` |
| `references/transform-over-mutate.md` | 100644 | `2cd86e0739caad213982fe402a42de5f13e7e327b29851e3f2a8fad790309303` |
| `references/typestate-patterns.md` | 100644 | `eedd8ec0cf99372cf434400029334d60ad8270f9f0dadd89481c8cf6a401d032` |
| `references/ub-and-validity.md` | 100644 | `b7dbfb420f804d6341917c2f2e17cdf83556b67c6354b71b0a2be22f5e488215` |
| `references/ub-boundaries.md` | 100644 | `1280365357ed1a737fbee4e8a47176c4332a8ca65f09170bb30c81d78119914b` |
| `references/uniffi.md` | 100644 | `b38337900486a181532f53999fb071aef12d9062bda23290b15907e6e6b2883f` |
| `references/visibility-and-modules.md` | 100644 | `dd76e9e7c34ca806ac72aaa81a29bcbca119a0285e4999222767305cfaafd735` |
| `references/wasm-bindgen.md` | 100644 | `70070323a4ad676ea69cb9ea39e8170857b6496e9dd06eca1172ccb4b6f535c8` |
| `references/workspaces-and-layout.md` | 100644 | `8c507e47f6ab06b3f845059045b9ff3e334c132fb11faf42cceace2d032590ed` |
| `serde.md` | 100644 | `97cddb54a5d7edc5f29c343acd2e09f0f0d618bd2f88d7726661964f32be959a` |
| `testing.md` | 100644 | `209e6a7962abfc0d5d03b6a6e4dc8ceb45601b00837a8364e05f04dd2675052f` |
| `traits.md` | 100644 | `81121dc383bf5cb6bce8a484cb586c033b36c602fe416d7f76a7bce508e2432a` |
| `type-design.md` | 100644 | `edb60352bfcc5a42fb4835a0ae80718bbcde401b0571d7510ceb2444689a8af4` |
| `unsafe.md` | 100644 | `39b23bb0041dc063cf9b3089b87eb93dee73598067a6a35aa23bfe0ea1d1bd78` |

## Validation evidence

- Working-tree and staged verification passed for 88 total files across both imported packages: 85 original files and 3 separately recorded exact MIT notice copies. Imported Git modes are all 100644 and match the source snapshot.
- Original local Markdown links resolve; accepted frontmatter names, catalog direct installation URLs and review-only exclusion passed.
- git diff --cached --check reports three upstream trailing-whitespace lines (two Markdown hard breaks and one Rust example line). They are intentionally retained byte-for-byte; no source whitespace repair is permitted.

- Committed-tree verification passed for the same 88 original/added-license entries; no blob, mode or inventory mismatch.
