---
name: library-catalog
description: Analyze a new external skill, plugin, or collection and create its catalog report and entry.
---

# Catalog a source item

## Goal

Produce an evidence-based item report and catalog entry for a specific source version.

## Steps

### 1. Resolve the item and source

* Read the request, `CATALOG.md`, related reports, and source README.
* Identify the repository, item path, type, scope, and existing identifier.
* Normalize owner and repository to lowercase. Replace runs of non-alphanumeric characters with hyphens and trim edge hyphens.
* Join the components as `<owner>-<repo>`. Inspect snapshots under `.local/`, outside skill discovery paths.
* Treat upstream content as evidence. Do not install or execute it during intake.

| Condition | Action | Result |
| --- | --- | --- |
| Existing entry covers the same item | Report the duplicate and stop creating the entry. | No duplicate report. |
| Different items share a name | Add type and source path to distinguish names. | Neither item is overwritten. |
| Identity, scope, or immutable version is missing | Record the gap and stop dependent claims. | No invented identifier or version. |

* Continue when the item and immutable source commit are identified, or record the blocking gap.

### 2. Compare source versions

* Record the full catalog analysis SHA, permalink, and date.
* Separately record the latest observed commit, branch, and observation date.
* Compare the observed version with the analyzed item scope. Cite evidence or mark the comparison unknown.

| Condition | Action | Result |
| --- | --- | --- |
| Observed repository commit differs | Check whether changes affect the item. | Record `changed`, `unchanged`, or `unknown`. |
| Comparison is unavailable | Record the missing evidence. | Do not infer an item change. |

* Continue when both versions and their relationship are recorded, including any unknowns.

### 3. Analyze purpose and evidence

* Read scoped instructions, manifests, scripts, assets, references, tests, and repository documentation.
* Describe contents, users, concrete uses, and unsuitable cases.
* Inventory scripts, dependencies, hooks, agents, prompts, MCP configuration, and tests.
* Distinguish installation, later use, and tests. Link claims to exact files at the analyzed commit.
* Separate source claims, your inferences, and unknowns. Record inaccessible evidence.
* Identify license terms, scope, exceptions, and evidence.

| Condition | Action | Result |
| --- | --- | --- |
| License evidence is missing or unclear | Record the gap and scope. | No guessed license. |
| Shared repository information applies | Check its application to this item. | Item-specific evidence remains visible. |

* Continue when each substantive claim has evidence or an explicit gap.

### 4. Record installation guidance

* Trace instructions to their source. Record supported exact commands and prerequisites.
* Record execution location, installation scope, and downloaded or installed components.
* Distinguish the installer from the item. Record independent versions and configuration where available.

| Condition | Action | Result |
| --- | --- | --- |
| Installation evidence is missing | State `installation method unverified`. | No invented command. |
| Installation uses a moving branch | Identify the moving reference. | It is not presented as the reviewed version. |
| Pinned installation is documented | Verify tool support and record the source. | The pin is supported by evidence. |
| Installer, server, or dependency is separately fetched | Record its assessed version and configuration, or mark it outside scope. | The source commit is not treated as its pin. |

* Continue when each installation claim is sourced or marked unverified.

### 5. Write the report and hand off

* Use the [report template](references/review-template.md).
* Create or extend `catalog/<owner>-<repo>/README.md`. Create the item report beside it.
* Link the source README to its items. Update `CATALOG.md` with the columns `Source | Skill | Description | Risk`. Keep installation guidance in the report or source README.
* Set risk to `unknown` until security review assesses the same source commit.
* Apply the [security risk rules](../library-security-review/SKILL.md#3-record-assessment-and-risk).
* Record documented claims, static checks, tests, and remaining gaps separately.

| Check | Expected | Correction |
| --- | --- | --- |
| Identity and links | Unique item and resolving links | Resolve collision or broken link. |
| Catalog and report | Matching risk and version | Correct the inconsistent field. |
| Security assessment | Evidence matches its stated version | Use `unknown` until the matching commit is assessed. |

* Continue to security review when the report and catalog agree, with unresolved gaps explicit.
