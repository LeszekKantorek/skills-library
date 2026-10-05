# skills-library

A library of AI skills installable with [`npx skills`](https://github.com/vercel-labs/skills).

Browse [CATALOG.md](CATALOG.md) for skills, risk ratings, reviews, and installation commands. No skills have been imported yet.

## Installation

```sh
npx skills add LeszekKantorek/skills-library --list
npx skills add LeszekKantorek/skills-library --skill <name>
```

Replace `<name>` with a name from the catalog.

## Request an import

Open a [GitHub Issue](https://github.com/LeszekKantorek/skills-library/issues/new/choose) with one or more skill links. Requests are reviewed and imported through pull requests.

- **No label:** pending or in progress.
- **imported:** accepted skills have been merged.
- **rejected:** the request was rejected in full.

For requests containing multiple links, the issue records each outcome. The issue form does not run an automatic importer.

## Risk

| Rating | Meaning |
| --- | --- |
| `low` | Instructions and local reads. |
| `medium` | Limited local changes, scripts, or network reads. |
| `high` | Sensitive data, external changes, broad permissions, or material assessment gaps. |
| `critical` | Malicious or hidden destructive behavior; rejected. |

Read each skill's review for the reasons and limitations. A rating is not a safety guarantee. Imports with material assessment gaps remain blocked until those gaps are resolved.

## Repository

- `skills/` — imported skills and their resources.
- `imports/` — technical reviews and source metadata.
- [CATALOG.md](CATALOG.md) — available skills.
- [library-curator](.agents/skills/library-curator/SKILL.md) — maintainer workflow and templates.

Changes to `main` require a pull request.
