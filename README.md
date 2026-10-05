# skills-library

A library of AI skills installable with [`npx skills`](https://github.com/vercel-labs/skills). See [CATALOG.md](CATALOG.md) for available skills and their risk ratings.

## Installation

```sh
npx skills add LeszekKantorek/skills-library --list
npx skills add LeszekKantorek/skills-library --skill <name>
```

Replace `<name>` with a name from the catalog. The library initially contains no imported skills. The local `library-curator` skill maintains this repository and is not listed in the import catalog.

## Structure

```text
.agents/skills/library-curator/SKILL.md  # instructions for the library maintainer
skills/<name>/SKILL.md                  # imported skill and its resources
imports/<name>.md                      # technical import review
README.md
CATALOG.md
```

## Import through a GitHub Issue

1. Open an issue using the "Import skill" form and provide one or more links.
2. The maintainer resolves each link to a specific version and reviews its content, resources, dependencies, and redistribution terms. Submitting a link does not execute external code.
3. The import is submitted as a PR together with a review in `imports/` and a catalog entry. Updates to existing skills also require an issue, a new assessment, and a PR.
4. After all accepted items have been merged, label the issue `imported` and close it. Label a fully rejected request `rejected` and close it, preserving the rationale.

The repository has only two labels: `imported` and `rejected`. They are mutually exclusive. An unlabeled issue is open and pending or in progress; there is no `open` label. For multiple links, track each outcome in the issue. If some items are rejected, use `imported` once all items are resolved and identify the rejected items in the summary. Until then, keep the issue open and unlabeled.

Issues are a work queue for the maintainer; the form does not run an automatic importer. Labels describe outcomes, not risk levels.

## Risk

Every assessment must assign exactly one of `low`, `medium`, `high`, or `critical`. The rating applies to a specific version, including its instructions, bundled code, and dependencies. Assess actions the skill tells an agent to perform even when it contains no scripts. Choose the highest applicable level and explain the concrete reasons in the review.

| Risk | Criteria and examples | Import decision |
| --- | --- | --- |
| `low` | Instructions and local reads; no code execution, data transmission, or external changes. | Eligible after review. |
| `medium` | Limited, reversible local writes or transparent scripts/dependencies; network reads without transmitting private data. | Eligible after documenting scope and dependencies. |
| `high` | Access to secrets, data transmission, publishing, service changes, deletion, broad permissions, or material gaps in the assessment. | Requires documented maintainer acceptance for that version in the PR and clear safeguards. Material assessment gaps must be resolved before import. |
| `critical` | Data theft, hidden destructive actions, malicious instructions, or bypassing security safeguards. | Reject; do not add files to `skills/`. |

When important files, dependencies, or behavior cannot be inspected, assign `high`, document the missing evidence, and hold the import until the gaps are resolved. Use `critical` if the available evidence already meets its criteria. Reassess once new evidence is available; never leave the rating blank or create a fifth risk value.

A rating is not a safety guarantee. Missing redistribution permission blocks import regardless of `risk`; record it as a separate finding rather than automatically increasing the rating.

## Import review

Each import and update has an `imports/<name>.md` review. The full SHA and source commit link identify the exact version reviewed; do not put a future library commit here. Git preserves the review history.

```yaml
---
link: "https://github.com/OWNER/REPO/tree/FULL_SHA/path/to/skill"
name: "local-skill-name"
sha: "FULL_SOURCE_COMMIT_SHA"
commit: "https://github.com/OWNER/REPO/commit/FULL_SHA"
risk: "medium"
---
```

Below the frontmatter, document the issue, original name, provenance and license, inspected files, behavior and permissions, network access and data flows, dependencies, risk rationale, modifications from the original, checks performed and their limitations, and the decision. Do not claim tests that were not run.

For sources without Git, set `sha` and `commit` to `null`, provide a stable `link`, and record the downloaded artifact's SHA-256 in the review body. Hold imports without an identifiable source snapshot. Preserve reviews for rejected skills, but do not create a catalog entry or a directory in `skills/` for them.

## Library changes

The `main` protection policy requires a PR, applies to administrators, and disables force pushes and branch deletion. Requiring a PR does not require another person's approval, allowing a single maintainer to operate the library. The first commit initializes the empty repository's base branch; subsequent changes go through PRs.
