---
name: library-curator
description: Review catalog and security results for evidence, consistency, and library-wide integrity.
---

# Review catalog consistency

## Goal

Identify actionable defects and gaps without substituting for substantive analysis or security assessment.

## Steps

### 1. Establish review scope

* Read the request, affected reports, source READMEs, and catalog rows.
* Read the [version procedure](../library-catalog/SKILL.md#2-compare-source-versions), [assessment rules](../library-security-review/SKILL.md#3-record-assessment-and-risk), and [report template](../library-catalog/references/review-template.md).
* Identify available evidence and the requested review boundary.

| Condition | Action | Result |
| --- | --- | --- |
| A required report or catalog entry is absent | Route the gap to the responsible stage. | The review identifies missing work. |
| Evidence is inaccessible | Record the limitation and affected claims. | The review does not imply verification. |

* Continue when scope, available evidence, and limitations are explicit.

### 2. Compare records and evidence

* Compare identifiers, source paths, item types, inventories, and source README item lists.
* Check duplicates, naming collisions, local links, and material claims against cited evidence.
* Check that catalog entries use `Source | Skill | Description | Risk`. Check that reports or source READMEs retain installation guidance.
* Compare installation, license, and validation claims with their evidence and scope.
* Compare analysis, security, and observed commits, dates, and change-scope evidence.

| Check | Expected | Correction |
| --- | --- | --- |
| Assessment absent or commit differs | Risk is `unknown` | Flag the unsupported rating. |
| Assessment commit matches | Report and catalog agree; completeness and confidence are separate from risk | Flag the inconsistent rating. |
| Critical assessment | Warning remains visible without installation encouragement | Flag the missing or misleading warning. |
| Evidence does not support a claim | Claim is qualified or gap is explicit | Flag the unsupported claim. |

* Continue when each mismatch has a location and evidence, or record the review limitation.

### 3. Route findings and recheck

* Return each defect with its location, impact, and concrete correction.
* Do not silently fill substantive gaps or perform a substitute audit.

| Finding | Route | Recheck |
| --- | --- | --- |
| Source, description, installation, or license gap | library-catalog | Compare the correction with source evidence. |
| Security evidence, behavior, risk, or assessment gap | library-security-review | Compare the correction with assessment evidence. |
| Catalog and report mismatch | Responsible stage for the affected field | Compare both records again. |

* Recheck corrections against findings and affected relationships.
* If no defects remain, state the scope, checks, and limitations.
* Authorized publication may follow review through the normal PR process. Do not infer permission to publish or comment.
* Finish when each finding is resolved or remains explicit with an owner and reason.
