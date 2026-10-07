---
link: "https://github.com/obra/superpowers/tree/8ca22dba9a94f28898bbce59f2537ff4d87c747d/skills/systematic-debugging"
name: "obra-superpowers-systematic-debugging"
sha: "8ca22dba9a94f28898bbce59f2537ff4d87c747d"
commit: "https://github.com/obra/superpowers/commit/8ca22dba9a94f28898bbce59f2537ff4d87c747d"
risk: "high"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/9
- Original name: systematic-debugging
- Reviewed: 2026-10-07. Full package inventoried with git archive and restored from exact pinned Git blobs to avoid archive newline conversion, outside automatic skill discovery. Source instructions were treated as review evidence, not invoked.

## License review
- License identifier(s): MIT.
- Evidence links (pinned to the source commit): [repository LICENSE](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/LICENSE).
- Scope and file-specific exceptions: Repository license covers the selected package. All 11 package files and their headers inspected; no separate skill license, conflicting header, vendored library or local third-party asset found. External links/images are not redistributed assets. Domain-specific examples and attribution remain unchanged.
- Redistribution permissions: MIT permits copying and redistribution with its notices retained.
- Required notices and other obligations: Preserve Copyright (c) 2025 Jesse Vincent and the full permission/warranty notice; no copyleft or change-notice requirement. Original files are not modified.
- Preserved license/attribution files and compliance actions: No redistribution proposed while blocked; a future import must include the exact source LICENSE.
- Unresolved questions or blockers: None identified in license evidence. Technical dependency blockers are listed below.

## Findings
- Files inspected: Complete 11-file inventory below; instructions, companion files, all code/examples, license, Git modes and paths. No symlinks, submodules or binary assets in this selected package.
- Behavior, permissions, and data flows: Reads logs/history, runs reproductions and tests, adds instrumentation and changes source. Diagnostic examples print environment/IDENTITY values and invoke keychain identity inspection and codesign; the shell expansion can print a nonempty identity, so redact sensitive values and avoid real signing credentials. find-polluter.sh enumerates test paths and runs npm test repeatedly; failures are suppressed and whitespace splitting makes paths containing spaces unreliable. No cleanup or external network destination is in that script. TypeScript polling example imports project-specific Lace types and is an example, not a standalone runnable library. Pressure-test documents demand scenario choices; they are evaluation fixtures, not authorization to deploy or alter production.
- Dependencies: Phase 4 requires superpowers:test-driven-development, absent from the request/library, and superpowers:verification-before-completion. The latter package is proposed here but npx preserves an unnamespaced original frontmatter name; superpowers: resolution depends on an upstream plugin/host, which this library does not bundle. Git, Bash, npm and project-controlled tests are needed for script examples. Historical CREATION-LOG/test prompts contain obsolete skills/debugging and skills/meta paths. Package-local technique references are present; Lace ~/threads imports are illustrative project-specific dependencies.
- Risk rationale and assessment gaps: High because it has unresolved mandatory workflow dependencies, plus sensitive diagnostics or server/network/process/deletion behavior. Static inspection is complete for the selected source package, but is not a guarantee for arbitrary consuming-project scripts, agent behavior or platform compatibility. Dependency and installation compatibility remain material unresolved gaps; import held.

## Import result
- Source file integrity: No imported files. All 11 snapshot files verified against pinned source Git blobs; SHA-256 inventory retained for a later import.
- Added license/attribution files and their provenance: None; review only.
- Checks performed and limitations: Complete file inventory, source/snapshot Git-blob identity, frontmatter and original-name uniqueness, package-local references, dependencies, catalog/review consistency and absence from skills/ and catalog. No source script, project test, pressure-test evaluation, installation, server, remote reply or publication workflow executed. External citation links were inspected as references; remote availability and host namespace registration are not guaranteed.
- Decision and blockers: Blocked; review only, no skill package or catalog entry. Required external skills and namespace/layout assumptions must be resolved in a separately authorized, pinned review or demonstrated compatible installation. Do not silently rewrite the source or import unrequested dependencies.

## Original file integrity

Hashes below identify reviewed snapshot files, not an import.

| Original file | Source Git blob (SHA-1) | SHA-256 |
| --- | --- | --- |
| condition-based-waiting-example.ts | 703a06b653160d060bbf46ab5c6e0cd7446bd592 | 40ae5ebe497fdf310200e43fe986552546d0a22837c0d39e855db1cfd33eb88e |
| condition-based-waiting.md | 70994f777c586f7d4c43033aac34c7cf0da6688b | e89fec8400d6cd50f43407cec9fab50976ba4d55d0ec2eb51c0bd68036b54c26 |
| CREATION-LOG.md | 9aa03092809feaf93c9bfa985252f6f1c9624692 | c24733a5b1821bd6bed1fc950261f0b9f4e90097e0bbb96459d8179713730789 |
| defense-in-depth.md | e2483354dc2b62478a2624e34ca18bc0efe887b2 | 1e175fb86fc357e58c6aebf5441e481e1b7868b4380c0456b63a17eefbd18ba7 |
| find-polluter.sh | 985f5d08ccf8a3f2d40739cfcaf4413bb24bf1cb | dd7b8f13c4cc2a24b33ff87b18da9248f3e1c80a085c3316224f69ff0fa5c43c |
| root-cause-tracing.md | 0e72e8f9566b7ef85e814633d1feacad9d0c5868 | 75b933b6a8c40bdb2031b10f21654395b56ec6ab6bc7b018c18d3fe57aeb7fb8 |
| SKILL.md | 095d194ac041502905f15b01d22d294fb94db8b2 | 808fc5717aa88ad65efff312b11c186294d3e6ee301afb584e2f86599b137787 |
| test-academic.md | 23a6ed7a2044e0c44d74c3101406140f4851aa41 | fe2ba480d78ac0d686dc025f41c2a32a43d642bf533f91b0c6053a04d35d6486 |
| test-pressure-1.md | 8d13b467e4a98abfffd12161cbc3c418021d6023 | 0b6a915db0054577819834c79be9eb614e97bddba10d73768e1fbe91cfed048a |
| test-pressure-2.md | 2d2315ec8a24ca872bc80d2f4056468ba051462a | b2030aeffba07050e8ad573ddf87486457c4a016a786bb326235bebd856f2016 |
| test-pressure-3.md | 89734b86fdc756488df315d53e5c3ac2d3752cd8 | 96b50a52e2c7989c9cf20fb752c47c1e9a3a70dc362f8f7989f8f5b64dac7708 |
