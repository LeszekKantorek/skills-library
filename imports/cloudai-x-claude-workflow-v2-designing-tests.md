---
link: "https://github.com/CloudAI-X/claude-workflow-v2/tree/3b5a89ec1c106dd387e372aec073f9401336382a/skills/designing-tests"
name: "cloudai-x-claude-workflow-v2-designing-tests"
sha: "3b5a89ec1c106dd387e372aec073f9401336382a"
commit: "https://github.com/CloudAI-X/claude-workflow-v2/commit/3b5a89ec1c106dd387e372aec073f9401336382a"
risk: "medium"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/7
- Original name: designing-tests
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
- Behavior, permissions, and data flows: Recommends writing tests and configuration, running npm test and coverage/watch commands, and fixing failures. Examples create test users and initialize/tear down a test database. Commands execute the consuming project scripts; examples must use isolated test databases and synthetic data. No credentials, remote destination, telemetry, publication, or bundled executable is specified.
- Dependencies: Consuming project test runner and npm scripts. Examples mention Vitest/Jest, MSW, SuperTest, Playwright, Testing Library, faker, pytest/httpx/requests, Selenium, testify/httptest, and chromedp. These are recommendations, not bundled or installed during review; pseudocode templates require project-specific setup.
- Risk rationale and assessment gaps: Medium because the workflow writes local tests/configuration and runs project-controlled test commands. Database teardown is explicitly a test fixture; use disposable test resources, never production data. No symlinks, submodules, executable files, or opaque binary assets in the selected package. This static review does not validate engineering effectiveness or guarantee safe behavior in every consuming project.

## Import result
- Source file integrity: all 1 original files copied from the pinned Git archive and checked by SHA-256; file inventory is complete. Original frontmatter, names, paths, references, encoding, and line endings are unchanged.
- Added license/attribution files and their provenance: LICENSE from the pinned containing repository. License additions are separate from the original file inventory below and are also byte-checked.
- Checks performed and limitations: tracked regular-file inventory, original-name uniqueness, frontmatter presence, local reference targets, valid evaluation JSON where present, review/catalog consistency, and staged Git-blob identity. Scoped .gitattributes disables text conversion for these packages. No installation, test runner, example code, agent evaluation, deployment, or GitHub action from the source skill was executed. External reference URLs are provenance/citation links, not executable dependencies; their ongoing availability is not guaranteed.
- Decision and blockers: accepted for inclusion in the PR with the documented risk and compatibility limitations; no unresolved import blocker. High-risk maintainer acceptance, where applicable, remains pending review and merge of the PR.

## Original file integrity

| Original file | Source Git blob (SHA-1) | Imported SHA-256 |
| --- | --- | --- |
| SKILL.md | 83b87fdb9ebafe2ad0d0ea31024bf55f90c5beee | 049cf75af6094c92c46135f07c700fae5cc020f7bb6bb6700a25ba912f798d67 |
