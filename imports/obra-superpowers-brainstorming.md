---
link: "https://github.com/obra/superpowers/tree/8ca22dba9a94f28898bbce59f2537ff4d87c747d/skills/brainstorming"
name: "obra-superpowers-brainstorming"
sha: "8ca22dba9a94f28898bbce59f2537ff4d87c747d"
commit: "https://github.com/obra/superpowers/commit/8ca22dba9a94f28898bbce59f2537ff4d87c747d"
risk: "high"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/9
- Original name: brainstorming
- Reviewed: 2026-10-07. Full package inventoried with git archive and restored from exact pinned Git blobs to avoid archive newline conversion, outside automatic skill discovery. Source instructions were treated as review evidence, not invoked.

## License review
- License identifier(s): MIT.
- Evidence links (pinned to the source commit): [repository LICENSE](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/LICENSE).
- Scope and file-specific exceptions: Repository license covers the selected package. All 8 package files and their headers inspected; no separate skill license, conflicting header, vendored library or local third-party asset found. External links/images are not redistributed assets. Domain-specific examples and attribution remain unchanged.
- Redistribution permissions: MIT permits copying and redistribution with its notices retained.
- Required notices and other obligations: Preserve Copyright (c) 2025 Jesse Vincent and the full permission/warranty notice; no copyleft or change-notice requirement. Original files are not modified.
- Preserved license/attribution files and compliance actions: No redistribution proposed while blocked; a future import must include the exact source LICENSE.
- Unresolved questions or blockers: None identified in license evidence. Technical dependency blockers are listed below.

## Findings
- Files inspected: Complete 8-file inventory below; instructions, companion files, all code/examples, license, Git modes and paths. No symlinks, submodules or binary assets in this selected package.
- Behavior, permissions, and data flows: Writes and commits design specs and requires staged approvals. Optional visual companion runs Node HTTP/WebSocket on loopback by default; can bind 0.0.0.0 and serves project HTML/assets, records click text/choices to state/events, persists session tokens/ports and opens a browser. Browser loads https://primeradiant.com/brand/superpowers-visual-brainstorming-logo.png?v=<version> by default, exposing client IP and version to that host; no-referrer suppresses referrer and telemetry-disable environment flags suppress this image. Generated pages can also make their own network requests. Server uses random tokens, strict cookie, WebSocket-origin checks and rejects symlink/hardlink assets; plain HTTP is not safe for untrusted remote networks. Operator BRAINSTORM_OPEN_CMD is shell-executed. stop-server.sh verifies a server instance id before signaling, but recursively deletes any supplied lexical /tmp/* session path: independently resolve/validate the exact disposable target. Windows ACLs and shell/process behavior are not validated. No hidden theft or malicious override found; absolute approval/process language remains subordinate to host/user instructions.
- Dependencies: Architectural path explicitly requires writing-plans, which is neither in issue #9 nor in this library. Bounded implementation also says TDD applies. Package-relative visual-companion.md and script assets exist, but literal skills/brainstorming/visual-companion.md assumes upstream layout; install here uses an owner-repository-skill directory. Companion requires Bash/POSIX utilities, Node built-ins and a browser. Missing repository version manifests fall back to unknown. spec-document-reviewer-prompt.md is bundled but current SKILL.md uses inline spec self-review. Optional elements-of-style skill is not a required dependency.
- Risk rationale and assessment gaps: High because it has unresolved mandatory workflow dependencies, plus sensitive diagnostics or server/network/process/deletion behavior. Static inspection is complete for the selected source package, but is not a guarantee for arbitrary consuming-project scripts, agent behavior or platform compatibility. Dependency and installation compatibility remain material unresolved gaps; import held.

## Import result
- Source file integrity: No imported files. All 8 snapshot files verified against pinned source Git blobs; SHA-256 inventory retained for a later import.
- Added license/attribution files and their provenance: None; review only.
- Checks performed and limitations: Complete file inventory, source/snapshot Git-blob identity, frontmatter and original-name uniqueness, package-local references, dependencies, catalog/review consistency and absence from skills/ and catalog. No source script, project test, pressure-test evaluation, installation, server, remote reply or publication workflow executed. External citation links were inspected as references; remote availability and host namespace registration are not guaranteed.
- Decision and blockers: Blocked; review only, no skill package or catalog entry. Required external skills and namespace/layout assumptions must be resolved in a separately authorized, pinned review or demonstrated compatible installation. Do not silently rewrite the source or import unrequested dependencies.

## Original file integrity

Hashes below identify reviewed snapshot files, not an import.

| Original file | Source Git blob (SHA-1) | SHA-256 |
| --- | --- | --- |
| scripts/frame-template.html | f540bb8a4f88107e2b37b2871a4c1a55a3b6f720 | 6a8a4e58bd6a44b904e2e3c57de774481d909204597e1498de53f1b2fecc4c4e |
| scripts/helper.js | e11d26489ce248f37af3e4dd01ddec6a4e88287f | 43c6d69954a46ec34a2a262bcc62a9a7e83e839c739f199cb72646d397c686e3 |
| scripts/server.cjs | a828b35af64d5c64ca68b9ec78473999ce698874 | 2d2961ea8d11f56c5f4c3a1a68d22709efa5d7601a2246d8c880774e7e9e8412 |
| scripts/start-server.sh | 016a8e4870142ce2adbe81a021d8b6b9073e7618 | a4e5ae84275bcaacd2f84345afeabe59cf7b00ba080e123da7cc1fb226f12847 |
| scripts/stop-server.sh | 7cacfe9440043f7a46eac555cd835fad0769c425 | 0b5ccbbd57f62d3ed88993f7940b5ee0e5c0fc9b21c550c623da4f6292e47daf |
| SKILL.md | e3f17885f8d5f87d7a92f0469141662b476e1288 | a32d2255354775aa124855aa7100cf276bea096fff4ebb3a0edf57be216e6c72 |
| spec-document-reviewer-prompt.md | 60993129de3c445efeff53987b5297dc1acf3eb1 | 95a0a195de9d984be2fffa95bab16fc8c563bc296a9cfc5e9c29cb3ece0d7457 |
| visual-companion.md | 8dca065bd9adb9d4fa82a66acbb4176ea23259c6 | 6ffcb038b53254bd31debaa15e12dcd4ff24bd63d690e0b644ac6396701cf2e2 |
