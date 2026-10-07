---
link: "https://github.com/obra/superpowers/tree/8ca22dba9a94f28898bbce59f2537ff4d87c747d/skills/requesting-code-review"
name: "obra-superpowers-requesting-code-review"
sha: "8ca22dba9a94f28898bbce59f2537ff4d87c747d"
commit: "https://github.com/obra/superpowers/commit/8ca22dba9a94f28898bbce59f2537ff4d87c747d"
risk: "medium"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/9
- Original name: requesting-code-review
- Reviewed: 2026-10-07. Full package inventoried with git archive and restored from exact pinned Git blobs to avoid archive newline conversion, outside automatic skill discovery. Source instructions were treated as review evidence, not invoked.

## License review
- License identifier(s): MIT.
- Evidence links (pinned to the source commit): [repository LICENSE](https://github.com/obra/superpowers/blob/8ca22dba9a94f28898bbce59f2537ff4d87c747d/LICENSE).
- Scope and file-specific exceptions: Repository license covers the selected package. All 2 package files and their headers inspected; no separate skill license, conflicting header, vendored library or local third-party asset found. External links/images are not redistributed assets. Domain-specific examples and attribution remain unchanged.
- Redistribution permissions: MIT permits copying and redistribution with its notices retained.
- Required notices and other obligations: Preserve Copyright (c) 2025 Jesse Vincent and the full permission/warranty notice; no copyleft or change-notice requirement. Original files are not modified.
- Preserved license/attribution files and compliance actions: Exact repository LICENSE copied into the imported package; original attribution preserved.
- Unresolved questions or blockers: None identified.

## Findings
- Files inspected: Complete 2-file inventory below; instructions, companion files, all code/examples, license, Git modes and paths. No symlinks, submodules or binary assets in this selected package.
- Behavior, permissions, and data flows: Reads Git history/diffs and provides a narrowly crafted task and code context to a general-purpose reviewer subagent. The bundled template requires a read-only review and forbids nested reviewers, but allows creating a separate temporary checkout if needed. Feedback can lead to reversible local code changes and project tests. No automatic GitHub posting, remote publication or secret lookup. Use a trusted agent environment, minimize supplied context and inspect project tests.
- Dependencies: Git and a host supporting general-purpose subagents. code-reviewer.md is present. References to subagent-driven development describe a use case, not a required dispatch mechanism. Hosts without subagents cannot use this workflow unchanged.
- Risk rationale and assessment gaps: Medium because it executes project-controlled checks or delegates code context within a trusted host. Static inspection is complete for the selected source package, but is not a guarantee for arbitrary consuming-project scripts, agent behavior or platform compatibility. No unresolved material source assessment gap; runtime workflows were not executed.

## Import result
- Source file integrity: All 2 original files copied byte-for-byte; SHA-256 and source Git blob comparisons passed. Complete imported file list consists of the original inventory plus LICENSE only.
- Added license/attribution files and their provenance: LICENSE only, exact copy of pinned repository LICENSE, SHA-256 a37e0e9697144819e1d965176ac4ae5bc3fa02d11e7812036bbcadf6dafe2400.
- Checks performed and limitations: Complete file inventory, source/snapshot Git-blob identity, frontmatter and original-name uniqueness, package-local references, dependencies, catalog/review consistency and staged Git-blob identity with scoped -text attributes preventing newline conversion. No source script, project test, pressure-test evaluation, installation, server, remote reply or publication workflow executed. External citation links were inspected as references; remote availability and host namespace registration are not guaranteed.
- Decision and blockers: Eligible for inclusion in this draft PR. No unresolved import blocker on a compatible host.

## Original file integrity

Hashes below identify imported originals; LICENSE is a separate addition.

| Original file | Source Git blob (SHA-1) | SHA-256 |
| --- | --- | --- |
| code-reviewer.md | 6d358b5d7d450c83cacbe450b7dbd4e673b694ad | 82e370be6b3447523816286195571e4216ba56ba1ad6ad0e87862294c4c78dcb |
| SKILL.md | 6d995da5c7d8d6c5a3cc63ddb701427f88ec2021 | cfcee1b06774e7c0517f1e09be1a11f2d5680257072723e709ddbcf7e08b795a |
