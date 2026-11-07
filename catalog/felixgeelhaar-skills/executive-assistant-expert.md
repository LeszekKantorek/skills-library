# executive-assistant-expert

## Identity and versions

* Identifier: `felixgeelhaar-skills-executive-assistant-expert`; author: Felix Geelhaar; type: skill. Scope: [executive-assistant-expert/SKILL.md](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/executive-assistant-expert/SKILL.md), a single instruction file in [the repository](https://github.com/felixgeelhaar/skills).
* Catalog analysis: [5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447](https://github.com/felixgeelhaar/skills/commit/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447), 2026-11-07. The file's Git blob is `acbce1ace27c1bec055bee599774b557264c2830`.
* Latest observed: [5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447](https://github.com/felixgeelhaar/skills/commit/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447), `main`, observed 2026-11-07 through the [branch API](https://api.github.com/repos/felixgeelhaar/skills/branches/main). The head equals the analyzed commit, so the item is unchanged at the observed head.
* Security assessment: `5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447`, 2026-11-07; operational risk: high; completeness: partial.

## Purpose and contents

The [prompt](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/executive-assistant-expert/SKILL.md#L9) addresses executive calendar, inbox, and meeting design. It is intended for executive assistants or chiefs of staff designing calendar, inbox, and decision rhythms. It is less suitable for autonomous account management without explicit authority and suitable account controls. These uses describe the source; the effectiveness and factual claims have not been tested.

The pinned [recursive tree](https://api.github.com/repos/felixgeelhaar/skills/git/trees/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447?recursive=1) contains one Markdown instruction file in the item directory. It contains the prompt and examples, with no item-local scripts, tests/evals, hooks, agent manifests, MCP configuration, or assets. It references companion skills, which are outside this assessment. The repository's installation example is separate from later prompt use; the item bundles no installer dependency.

## Installation

See the [shared upstream installation instructions and warning](README.md#installation). The documented Claude Code command installs all matching skills from a moving branch and can overwrite user-level files.

## License

The [repository MIT license](README.md#license) applies to this item. The pinned tree has no separate item license, and no different notice was identified in the skill. Rights in third-party quotations and frameworks were not independently cleared.

## Security

Assessment: static security pass of the pinned item file and tree and repository installation example, at commit `5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447`, 2026-11-07. Completeness is **partial** and confidence is moderate for visible instructions and limited for runtime effects. The host, companion skills, Git, shell utilities, providers, and separately configured integrations are outside scope and unassessed.

* The [frontmatter](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/executive-assistant-expert/SKILL.md#L1) declares `Read`, `Glob`, `Grep`, `WebSearch`, `WebFetch`, and three Scout browsing tools. Local reads can place accessible files in host context. Search queries go to the search provider, and fetched URLs go to the provider and destination. A retrieved page could contain instructions intended to redirect the agent; use public or anonymized queries and treat fetched content as data. Recipients, retention, and host enforcement are unknown. Tool declarations do not establish host enforcement.
* The [working modes](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/executive-assistant-expert/SKILL.md#L177) establish the item-specific scenario: Inbox and calendar material can contain private messages, names, and meeting details. The prompt describes deleting, delegating, and responding to messages and directs cancellation of meetings without a purpose. Those are recommendations or instructions to the agent, not proof that this file can change an account: its declared tools are read and browsing tools. A host with additional permissions could act on them; require explicit authorization and review before sends, deletion, or calendar changes.
* No fixed exfiltration endpoint, secret collection instruction, executable shell command, or automatic publication was identified in the item file. The installation example clones the whole repository from a moving branch and can overwrite user-level files; it was not run. Inspect the source and target paths before use.

**Risk: high.** The prompt calls for potentially consequential inbox and meeting actions and involves sensitive executive information, even though its declared tools do not themselves provide account changes. Review the prompt, restrict host access to the task, and review consequential outputs and actions. This rating is not a safety guarantee. Actual tool enforcement, provider behavior, companion skills, and quality of advice remain unverified.

## Validation

Documented: the pinned README's installation instructions. Static verification: fetched the complete pinned item, README, license, tree, and branch via GitHub; matched the Git blob of the existing local copy to the upstream file; inspected the prompt and installation separately. The [legacy import report](../../imports/felixgeelhaar-skills-executive-assistant-expert.md) records the earlier import and its scope. No upstream instructions, installer, declared tools, or domain-quality tests were executed; runtime behavior remains unverified.
