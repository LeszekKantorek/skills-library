---
link: "https://github.com/felixgeelhaar/skills/tree/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/content-editor"
name: "felixgeelhaar-skills-content-editor"
sha: "5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447"
commit: "https://github.com/felixgeelhaar/skills/commit/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447"
risk: "medium"
---

## Source
- Issue: [#2](https://github.com/LeszekKantorek/skills-library/issues/2).
- Original name: `content-editor`.
- Source package: `content-editor/SKILL.md`, blob `688d0efe07164c7c0d13355a45c3717069b0630c`.
- Source identity: `felixgeelhaar-skills-content-editor`. The package directory and review identity use the library's namespaced name. SKILL.md frontmatter and companion references retain the original names at the maintainer's explicit instruction; only the curator's file-content renaming requirement is overridden.
- Source version: immutable commit `5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447`.

## License review
- License identifier(s): MIT.
- Evidence links: [repository LICENSE](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/LICENSE), [README license declaration](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/README.md#license), [complete skill file](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/content-editor/SKILL.md).
- Scope and file-specific exceptions: repository MIT license covers the single Markdown file; the complete source tree contains no per-skill license, COPYING file, scripts, assets or separate dependency material. No different file-level license notice was identified. Named books, frameworks and quotations remain attributed in the unchanged file; this review does not independently clear rights in every referenced third-party quotation.
- Redistribution and modification permissions: MIT expressly permits copying, modification and redistribution; no modification of the skill file is performed.
- Required notices and other obligations: retain the copyright notice (2024–2026 Felix Geelhaar), MIT permission notice and disclaimer in copies/substantial portions. No source-sharing obligation.
- Preserved license/attribution files and compliance actions: the complete, unmodified repository LICENSE is copied to `skills/felixgeelhaar-skills-content-editor/LICENSE`; source attributions inside SKILL.md are preserved.
- Unresolved questions or blockers: no conflicting license or redistribution restriction identified in the supplied package.

## Findings
- Files inspected: full source-tree inventory, `content-editor/SKILL.md`, repository LICENSE and README. Full text was scanned for command execution, secrets, external endpoints, destructive actions and instruction overrides; activation, declared tools, operating modes and companion references were reviewed. Domain claims were not independently fact-checked.
- Behavior, permissions, and data flows: The only document-editor package: explicitly declares Write and Edit for transforming supplied notes into local documents. Document templates and Markdown fences are illustrative content, not runnable scripts. Its diagnose mode asks for audience/document-type confirmation.
- Declared tools: `Read, Write, Edit, Glob, Grep`. These source declarations are preserved; availability depends on the host agent and does not override user authorization or host safeguards.
- Dependencies: no bundled executable or install-time dependency. Named external services, frameworks and tools are contextual/optional. No network or connector tool is declared by this package. Companion skills are optional and use their original names, preserved across this batch.
- Network destinations: none declared; this package lists only local read/write/edit/search tools. It supplies no upload endpoint or publishing tool.
- Risk rationale and assessment gaps: medium because the declared workflow permits reversible local document writes rather than only local reads. Static review does not establish runtime safety, factual accuracy or host-specific connector behavior. No executable code was run, secrets provided, account data accessed or external workflow enacted.

## Import result
- Changes from source: none to SKILL.md. Source name, description, allowed-tools, body, companion references and wording remain unchanged. The destination directory is namespaced; installation selects the original frontmatter name. The sole package addition is an exact copy of the source repository LICENSE.
- Checks performed and limitations: verified 32 requested directories each contain one regular SKILL.md, with no symlinks, additional resources or scripts; checked original frontmatter names, namespaced package/review/catalog identities and all original companion names against the batch; reviewed Markdown references and preserved source license. Original blob identities are checked in the prepared Git tree. No agent execution, npx installation or domain-quality tests were performed; local execution tools were unavailable.
- Decision and blockers: prepared for import through the PR; no technical or license blocker identified. Installation does not itself grant external-action permission.
