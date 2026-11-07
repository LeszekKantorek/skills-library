# Skills Library

Skills Library catalogs external AI skills and plugins for readers who want to understand their contents, usefulness, installation, and security risks.

Browse the [catalog](CATALOG.md) to compare sources, skills, descriptions, and risk ratings. Each entry links to a report with source evidence and an assessment at a specific commit.

## Use the catalog

1. Choose an item in [CATALOG.md](CATALOG.md).
2. Read its report for purpose, contents, prerequisites, license, and security findings.
3. Compare the assessed commit with the latest observed source commit recorded in the report.
4. Follow the report's installation guidance or its link to the shared source README.

Installation uses the upstream source. Reports identify the applicable method, such as an `npx` command or plugin installation procedure, and its scope. This repository stores descriptions and reviews rather than copies of external packages.

A command that follows a branch or downloads dependencies can install code outside the assessed snapshot. Read the installation limits before running it.

## Read the risk rating

| Risk | Meaning |
| --- | --- |
| `low` | Local reading or instructions with limited effects. |
| `medium` | Reversible local writes, limited execution, or network reads without private data. |
| `high` | Secrets, data transmission, publication, deletion, service changes, or broad permissions with material consequences. |
| `critical` | Theft, concealed destruction, or safeguard bypass with severe consequences. |
| `unknown` | Insufficient evidence to assign a rating. |

Ratings describe the assessed behavior and scope. High risk does not mean malware, and low risk is not a safety guarantee. Reports record evidence, safeguards, coverage gaps, and untested behavior separately.

## Check source versions

Each report records the full analysis and security commit SHAs, dates, and latest observed upstream commit. Use these references to identify the reviewed version and compare later changes.

The latest observed commit reflects the report's check date. It does not imply that later upstream changes have been assessed. Installation commands do not necessarily pin the reviewed commit.

## Request an assessment or update

Open a [GitHub issue](https://github.com/LeszekKantorek/skills-library/issues/new/choose) with the upstream source and item path. For an update, include the existing catalog report and the revision or changes to inspect.

## Repository structure

| Path | Contents |
| --- | --- |
| [CATALOG.md](CATALOG.md) | Source, skill, description, and risk table. |
| `catalog/<owner>-<repo>/README.md` | Source overview, item links, and shared installation and license information. |
| `catalog/<owner>-<repo>/<item>.md` | Item description, source versions, installation guidance, and security evidence. |
| `.agents/skills/` | Project workflows and supporting authoring skills. |
| `.local/` | Ignored local plans, source snapshots, and temporary analysis files. |

## Maintain the library

| Workflow | Responsibility |
| --- | --- |
| [library-catalog](.agents/skills/library-catalog/SKILL.md) | Analyze a source and create its report, source overview, and catalog entry. |
| [library-security-review](.agents/skills/library-security-review/SKILL.md) | Independently inspect the recorded source version and add security evidence and risk. |
| [library-curator](.agents/skills/library-curator/SKILL.md) | Review evidence, consistency, links, and agreement across the library. |

The skills contain the procedures and report template. Follow [AGENTS.md](AGENTS.md) for local working files and source handling.
