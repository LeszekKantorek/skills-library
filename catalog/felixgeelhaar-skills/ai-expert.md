# ai-expert

## Identity and versions

* Identifier: `felixgeelhaar-skills-ai-expert`; author: Felix Geelhaar; type: skill. Scope: [ai-expert/SKILL.md](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/ai-expert/SKILL.md), a single prompt file in [the upstream repository](https://github.com/felixgeelhaar/skills).
* Catalog analysis: [5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447](https://github.com/felixgeelhaar/skills/commit/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447), 2026-11-07. The file's Git blob is `ec723356b3ac9bf3f8a227fbd1ff6c69b6c1e5da`.
* Latest observed: [5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447](https://github.com/felixgeelhaar/skills/commit/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447), `main`, checked 2026-11-07 against the [branch API](https://api.github.com/repos/felixgeelhaar/skills/branches/main). The branch head equals the analyzed commit, so the item is unchanged at the observed head.
* Security assessment: `5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447`, 2026-11-07; operational risk: medium; completeness: partial.

## Purpose and contents

The prompt addresses AI product decisions, model choice, RAG, evaluation and AI UX. It can help a product team comparing model and architecture options or planning AI evaluations. It is less suitable for general product strategy or engineering work without an AI angle. These are the scope and uses described in the [skill](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/ai-expert/SKILL.md); effectiveness and factual claims have not been tested.

The pinned [recursive tree](https://api.github.com/repos/felixgeelhaar/skills/git/trees/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447?recursive=1) contains one Markdown instruction/prompt file in this item directory. There are no item-local scripts, tests/evals, hooks, agent manifests, MCP configuration, or assets. The prompt refers to optional companion skills; these and the separately configured Scout integration are outside this assessment. The repository README contains a shell installation example; it is distinct from later use of the prompt. The source does not bundle an installer dependency in this item.

## Installation

See the [shared upstream installation instructions and warning](README.md#installation). The documented Claude Code command installs all matching skills from a moving branch and can overwrite user-level files.

## License

The [repository MIT license](README.md#license) applies to this item. The item directory has no separate license file in the pinned tree, and no different notice was identified in the skill. Rights in third-party quotations and frameworks were not independently cleared.

## Security

Assessment: independent static security pass of the pinned item file and tree, README installation example, and the local file whose Git blob matches upstream; commit `5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447`, 2026-11-07. Completeness is **partial**, confidence moderate for the visible prompt, limited for runtime behavior. Companion skills, Git, shell utilities, host, model provider, search/fetch providers and Scout server versions, configurations and permissions are outside scope and unassessed.

* The [frontmatter](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/ai-expert/SKILL.md#L1) declares `Read`, `Glob`, `Grep`, `WebSearch`, `WebFetch`, and three Scout browsing tools. Local reads can expose accessible files to the host context; web searches disclose query terms to the search provider and fetches disclose requested URLs to the provider and destination. Actual recipients, retention and permissions depend on the host. No fixed exfiltration endpoint, secret collection instruction, shell execution, deletion or publication instruction was identified in the item file. Tool declarations are not proof the host enforces them.
* The [prompt](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/ai-expert/SKILL.md#L9) directs research before model, trend, and landscape answers, making network use an expected step for those questions. A query containing a proprietary product plan could disclose it to a search provider; a malicious retrieved page could steer the agent. Use public or anonymized queries and treat retrieved text as data. The prompt discusses privacy, least privilege, prompt injection and approval for consequential actions, but those are design recommendations, not enforced controls.
* The README's optional clone-and-copy installation accesses GitHub, downloads the whole repository and writes to user skill directories; it may overwrite files. It uses a moving branch and is not a pinned installation. Inspect the source and target paths before using it. This static review did not execute the commands.
* Untrusted fetched content can contain instructions that redirect an agent or induce disclosure if the host treats content as authority. Keep host permissions narrow, separate external content from instructions, and review consequential actions. Optional companion skills can introduce additional behavior; they are not covered here.

**Risk: medium.** The visible prompt permits local reads and network research, with no observed instruction to transmit secrets or make service changes. Sensitive-data disclosure remains possible through host-selected query content; runtime tool behavior and integrations are unknown. Recommendation: review the prompt and constrain data and tools before use. This rating is not a safety guarantee or an assessment of the moving branch after the observation date.

Unresolved: actual host enforcement, Scout implementation and data recipients, installation behavior, behavior of companion skills, and performance or safety of generated advice.

## Validation

Documented: installation instructions in the pinned README. Static checks: fetched the pinned README, license, item file and recursive tree via the GitHub connector; compared the local item's Git blob to the upstream tree blob. Branch head checked via GitHub branch API. No upstream instructions, installation, agents, declared network tools or domain-quality tests were executed. Host behavior, external dependencies and runtime effects remain unverified.
