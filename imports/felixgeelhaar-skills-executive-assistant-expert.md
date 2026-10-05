---
link: "https://github.com/felixgeelhaar/skills/tree/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/executive-assistant-expert"
name: "executive-assistant-expert"
sha: "5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447"
commit: "https://github.com/felixgeelhaar/skills/commit/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447"
risk: "high"
---

## Source
- Issue: [#2](https://github.com/LeszekKantorek/skills-library/issues/2).
- Original name: `executive-assistant-expert`.
- Source package: `executive-assistant-expert/SKILL.md`, blob `acbce1ace27c1bec055bee599774b557264c2830`.
- Source identity: `felixgeelhaar-skills-executive-assistant-expert`. Package name, directory and frontmatter intentionally retain the original name at the maintainer's explicit instruction; this overrides the curator's normal namespacing rule.
- Source version: immutable commit `5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447`.

## License review
- License identifier(s): MIT.
- Evidence links: [repository LICENSE](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/LICENSE), [README license declaration](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/README.md#license), [complete skill file](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/executive-assistant-expert/SKILL.md).
- Scope and file-specific exceptions: repository MIT license covers the single Markdown file; the complete source tree contains no per-skill license, COPYING file, scripts, assets or separate dependency material. No different file-level license notice was identified. Named books, frameworks and quotations remain attributed in the unchanged file; this review does not independently clear rights in every referenced third-party quotation.
- Redistribution and modification permissions: MIT expressly permits copying, modification and redistribution; no modification of the skill file is performed.
- Required notices and other obligations: retain the copyright notice (2024–2026 Felix Geelhaar), MIT permission notice and disclaimer in copies/substantial portions. No source-sharing obligation.
- Preserved license/attribution files and compliance actions: the complete, unmodified repository LICENSE is copied to `skills/executive-assistant-expert/LICENSE`; source attributions inside SKILL.md are preserved.
- Unresolved questions or blockers: no conflicting license or redistribution restriction identified in the supplied package.

## Findings
- Files inspected: full source-tree inventory, `executive-assistant-expert/SKILL.md`, repository LICENSE and README. Full text was scanned for command execution, secrets, external endpoints, destructive actions and instruction overrides; activation, declared tools, operating modes and companion references were reviewed. Domain claims were not independently fact-checked.
- Behavior, permissions, and data flows: Inbox/calendar context is inherently sensitive. The text recommends deleting/delegating/responding to messages, canceling purposeless recurring meetings and proactive gatekeeping. These recommended external changes make this high even though declared tools are read/search/browser tools. The source does not implement an approval boundary.
- Declared tools: `Read, Glob, Grep, WebSearch, WebFetch, mcp__scout__navigate, mcp__scout__readable_text, mcp__scout__observe`. These source declarations are preserved; availability depends on the host agent and does not override user authorization or host safeguards.
- Dependencies: no bundled executable or install-time dependency. Named external services, frameworks and tools are contextual/optional. Scout connector tools require separately configured host integrations; no connection was established during import. Companion skills are optional and use their original names, preserved across this batch.
- Network destinations: research through WebSearch/WebFetch and Scout browsing. No hard-coded upload/exfiltration endpoint was identified. Query terms and requested URLs are disclosed to the relevant search/fetch provider. Keep credentials and private user/customer/health/business information out of public research requests; use public or anonymized inputs.
- Risk rationale and assessment gaps: high due to sensitive inbox/calendar context and recommended external deletion, response and meeting cancellation actions. Static review does not establish runtime safety, factual accuracy or host-specific connector behavior. No executable code was run, secrets provided, account data accessed or external workflow enacted.

## Import result
- Changes from source: none to SKILL.md. Source name, description, allowed-tools, body, companion references and wording remain unchanged. The sole package addition is an exact copy of the source repository LICENSE.
- Checks performed and limitations: verified 32 requested directories each contain one regular SKILL.md, with no symlinks, additional resources or scripts; checked original frontmatter names, package/review/catalog consistency and all companion names against the batch; reviewed Markdown references and preserved source license. Original blob identities are checked in the prepared Git tree. No agent execution, npx installation or domain-quality tests were performed; local execution tools were unavailable.
- Decision and blockers: prepared for import in the PR; maintainer acceptance of this high-risk package is still required before merge. Suggested safeguards: least-privilege host tooling, no secrets in research queries, scope account access to the task and review proposed inbox/calendar changes before applying them; external sends, deletions and calendar changes require explicit user authorization of the relevant action. Installation does not itself grant external-action permission.
