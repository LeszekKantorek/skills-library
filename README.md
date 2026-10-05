# skills-library

A library of AI skills installable with [`npx skills`](https://github.com/vercel-labs/skills).

Browse [CATALOG.md](CATALOG.md) for skills, risk ratings, reviews, and installation commands. No skills have been imported yet.

## Installation

```sh
npx skills add LeszekKantorek/skills-library --list
npx skills add https://github.com/LeszekKantorek/skills-library/tree/main/skills/<name>
```

Replace `<name>` with the library name from the catalog. Imported source files, including their original skill names and references, are preserved unchanged; applicable license files are included in each package.

## Request an import

Open a [GitHub Issue](https://github.com/LeszekKantorek/skills-library/issues/new/choose) with one or more skill links. Requests are reviewed and imported through pull requests.

For requests containing multiple links, the issue records each outcome. Closing a linked pull request also closes the issue, whether or not the PR is merged. The issue form does not run an automatic importer.

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
