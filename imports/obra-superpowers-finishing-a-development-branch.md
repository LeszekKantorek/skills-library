---
link: "https://github.com/obra/superpowers/tree/8ca22dba9a94f28898bbce59f2537ff4d87c747d/skills/finishing-a-development-branch"
name: "obra-superpowers-finishing-a-development-branch"
sha: "8ca22dba9a94f28898bbce59f2537ff4d87c747d"
commit: "https://github.com/obra/superpowers/commit/8ca22dba9a94f28898bbce59f2537ff4d87c747d"
risk: "high"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/9
- Original name: finishing-a-development-branch
- Reviewed: 2026-10-07. Full package inventoried with git archive and restored from exact pinned Git blobs to avoid archive newline conversion, outside automatic skill discovery. Source instructions were treated as review evidence, not invoked.

## License review
- License identifier(s): MIT.
- Evidence links (pinned to the source commit): [repository LICENSE](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/LICENSE).
- Scope and file-specific exceptions: Repository license covers the selected package. All 1 package files and their headers inspected; no separate skill license, conflicting header, vendored library or local third-party asset found. External links/images are not redistributed assets. Domain-specific examples and attribution remain unchanged.
- Redistribution permissions: MIT permits copying and redistribution with its notices retained.
- Required notices and other obligations: Preserve Copyright (c) 2025 Jesse Vincent and the full permission/warranty notice; no copyleft or change-notice requirement. Original files are not modified.
- Preserved license/attribution files and compliance actions: Exact repository LICENSE copied into the imported package; original attribution preserved.
- Unresolved questions or blockers: None identified.

## Findings
- Files inspected: Complete 1-file inventory below; instructions, companion files, all code/examples, license, Git modes and paths. No symlinks, submodules or binary assets in this selected package.
- Behavior, permissions, and data flows: Runs full tests, inspects Git/worktree state, pulls, merges, pushes and opens PRs; may remove worktrees and delete branches. Discard requires explicit user request and the exact confirmation discard. Force-push requires explicit authorization; failed worktree removal must not be forced. Directory-name-based ownership is a heuristic, not proof: independently verify resolved cleanup targets and ownership, preserve unique files, and follow host-managed-worktree rules. Confirm repository, base, destination and publication authorization before remote changes.
- Dependencies: Git, a POSIX shell for command examples, consuming-project test runner and forge tooling. Normal repositories and externally managed detached worktrees have documented alternatives. No mandatory companion skill.
- Risk rationale and assessment gaps: High because the recommended workflow publishes/removes Git resources or sends authenticated external replies. Static inspection is complete for the selected source package, but is not a guarantee for arbitrary consuming-project scripts, agent behavior or platform compatibility. No unresolved material source assessment gap; runtime workflows were not executed.

## Import result
- Source file integrity: All 1 original files copied byte-for-byte; SHA-256 and source Git blob comparisons passed. Complete imported file list consists of the original inventory plus LICENSE only.
- Added license/attribution files and their provenance: LICENSE only, exact copy of pinned repository LICENSE, SHA-256 a37e0e9697144819e1d965176ac4ae5bc3fa02d11e7812036bbcadf6dafe2400.
- Checks performed and limitations: Complete file inventory, source/snapshot Git-blob identity, frontmatter and original-name uniqueness, package-local references, dependencies, catalog/review consistency and staged Git-blob identity with scoped -text attributes preventing newline conversion. No source script, project test, pressure-test evaluation, installation, server, remote reply or publication workflow executed. External citation links were inspected as references; remote availability and host namespace registration are not guaranteed.
- Decision and blockers: Eligible for inclusion in this draft PR. Maintainer acceptance of high risk remains pending review/merge; do not treat this review as permission to publish, delete or send replies.

## Original file integrity

Hashes below identify imported originals; LICENSE is a separate addition.

| Original file | Source Git blob (SHA-1) | SHA-256 |
| --- | --- | --- |
| SKILL.md | fa8aecaf8813f1b19d19996f7957d1b0121f2d9c | 8db5a922b242dd4e1bf824cb91c13b3e8d8e8a86d6ceaf7f0774eb9cce909d65 |
