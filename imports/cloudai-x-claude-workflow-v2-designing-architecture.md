---
link: "https://github.com/CloudAI-X/claude-workflow-v2/tree/3b5a89ec1c106dd387e372aec073f9401336382a/skills/designing-architecture"
name: "cloudai-x-claude-workflow-v2-designing-architecture"
sha: "3b5a89ec1c106dd387e372aec073f9401336382a"
commit: "https://github.com/CloudAI-X/claude-workflow-v2/commit/3b5a89ec1c106dd387e372aec073f9401336382a"
risk: "medium"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/7
- Original name: designing-architecture
- Reviewed: 2026-10-05. Source extracted with git archive at the immutable commit above, outside automatic skill discovery; no source skill was installed or executed.

## License review
- License identifier(s): MIT.
- Evidence links (pinned to the source commit): https://github.com/CloudAI-X/claude-workflow-v2/blob/3b5a89ec1c106dd387e372aec073f9401336382a/LICENSE
- Scope and file-specific exceptions: Repository MIT license covers the selected package. No skill-specific license, notice, headers assigning different terms, third-party assets, or bundled libraries were found.
- Redistribution permissions: MIT permits copying and redistribution of the package with copyright and permission notices retained.
- Required notices and other obligations: retain the applicable complete copyright, permission, and warranty notices. No copyleft source-sharing obligation or change notice is required by MIT; original package files remain unchanged.
- Preserved license/attribution files and compliance actions: added an exact copy of the source repository LICENSE to this package. Existing attribution and source links remain unchanged.
- Unresolved questions or blockers: none identified in the inspected license evidence.

## Findings
- Files inspected: full tracked file inventory below; entrypoint, companion documentation/evaluation data, reference guidance, file modes, license/header evidence, paths/links, and static scans for execution, network, secret access, destructive behavior, and instruction overrides.
- Behavior, permissions, and data flows: Reads requirements and code, chooses architectural patterns, and recommends project scaffolding and writing architecture decisions. No scripts, command execution, network destinations, credentials, publishing, or destructive operations are specified.
- Dependencies: None; one standalone Markdown file. Architectural choices are heuristics and require project-specific judgment.
- Risk rationale and assessment gaps: Medium because project scaffolding and design documentation imply limited reversible local writes, despite the Markdown-only package. No symlinks, submodules, executable files, or opaque binary assets in the selected package. This static review does not validate engineering effectiveness or guarantee safe behavior in every consuming project.

## Import result
- Source file integrity: all 1 original files copied from the pinned Git archive and checked by SHA-256; file inventory is complete. Original frontmatter, names, paths, references, encoding, and line endings are unchanged.
- Added license/attribution files and their provenance: LICENSE from the pinned containing repository. License additions are separate from the original file inventory below and are also byte-checked.
- Checks performed and limitations: tracked regular-file inventory, original-name uniqueness, frontmatter presence, local reference targets, valid evaluation JSON where present, review/catalog consistency, and staged Git-blob identity. Scoped .gitattributes disables text conversion for these packages. No installation, test runner, example code, agent evaluation, deployment, or GitHub action from the source skill was executed. External reference URLs are provenance/citation links, not executable dependencies; their ongoing availability is not guaranteed.
- Decision and blockers: accepted for inclusion in the PR with the documented risk and compatibility limitations; no unresolved import blocker. High-risk maintainer acceptance, where applicable, remains pending review and merge of the PR.

## Original file integrity

| Original file | Source Git blob (SHA-1) | Imported SHA-256 |
| --- | --- | --- |
| SKILL.md | e54dc3b29b8507f4ae5261f8683b75e8552378f4 | 479f4abc528c6af38edc6caa6de97b5a92fbce9005f786f23da49bafd1692b23 |
