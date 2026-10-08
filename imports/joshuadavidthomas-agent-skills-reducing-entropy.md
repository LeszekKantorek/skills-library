---
link: "https://github.com/joshuadavidthomas/agent-skills/tree/516dee7a422b90937b2958d11c03694154ab9c09/reducing-entropy"
name: "joshuadavidthomas-agent-skills-reducing-entropy"
sha: "516dee7a422b90937b2958d11c03694154ab9c09"
commit: "https://github.com/joshuadavidthomas/agent-skills/commit/516dee7a422b90937b2958d11c03694154ab9c09"
risk: "high"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/14 (no comments or special acceptance at review time).
- Original name: `reducing-entropy`; original frontmatter preserved for accepted packages.
- Snapshot: `516dee7a422b90937b2958d11c03694154ab9c09`; resolved upstream main on 2026-10-08. Downloaded outside automatic skill discovery. The issue's researching-codebases blob URL refers to a directory; resolved to the existing tree without expanding requested scope.

## License review
- License identifier(s): MIT.
- Repository evidence: [MIT LICENSE](https://github.com/joshuadavidthomas/agent-skills/blob/516dee7a422b90937b2958d11c03694154ab9c09/LICENSE), Copyright (c) 2025 Josh Thomas.
- Scope and file-specific exceptions: Repository MIT grant applies; the references are explanatory mindsets and attributed concepts/short quotations, not complete vendored book or talk snapshots. No separate package grant or restrictive file header found.
- Redistribution permissions: MIT permits unchanged redistribution when copyright/permission notice is included; mixed packages retain the additional license scopes described above.
- Required notices and other obligations: preserve all original attribution and applicable license copies; never modify original imported sources or imply endorsement.
- Preserved license/attribution files and compliance actions: `LICENSE`: exact `LICENSE` from `issue-14@516dee7a422b90937b2958d11c03694154ab9c09`. Original attributions and license links remain unchanged.
- Unresolved questions or blockers: The operational acceptance/compatibility blockers below are separate from license eligibility.

## Findings
- Files inspected: complete 6-file inventory below; SKILL.md, adding-reference-mindsets.md and four references/ Markdown files included, with operation-bearing content reviewed explicitly. Static scans inspected all file contents. External source content treated only as evidence, never executed as instructions.
- Behavior, permissions, and data flows: Markdown design/refactoring policy explicitly biases toward deletion, suggests deleting entire features, and rejects a change when its final line count increases. This can encourage destructive removal and override required behavior if used mechanically. Reference exceptions include regulatory requirements and security fundamentals; they do not remove the core unconditional line-count rule.
- Dependencies: Six Markdown files; all four required reference mindsets are present. adding-reference-mindsets.md is local authoring advice. Links to talks, articles, books and presentations are citations, not downloaded executable dependencies.
- Risk rationale and assessment gaps: high according to the highest applicable documented behavior. All six Markdown files inventoried and directly inspected; no scripts, files deleted, or reference network operations executed.

## Import result
- Source file integrity: Complete originals imported unchanged from pinned Git blobs; exact inventory, byte and mode checks cover working tree, index and committed tree. Added license notices are checked separately.
- Added license/attribution files and their provenance: `LICENSE`: exact `LICENSE` from `issue-14@516dee7a422b90937b2958d11c03694154ab9c09`. Original attributions and license links remain unchanged.
- Checks performed and limitations: immutable Git snapshot and complete file/mode inventory; UTF-8/frontmatter names; local Markdown links and inline path references; license/attribution scope; static code/behavior and dependency scans; review/catalog consistency. No upstream code or instructions executed. All six Markdown files inventoried and directly inspected; no scripts, files deleted, or reference network operations executed.
- Decision and blockers: Imported unchanged following the maintainer decision below. Earlier review-only holds are superseded; documented findings and operational limits remain.

## Original file inventory

| Original relative path | Git mode | SHA-256 |
| --- | --- | --- |
| `SKILL.md` | 100644 | `227438f347b69408f36e6f9e626864b7480e641a70417dcaa9069916133f7421` |
| `adding-reference-mindsets.md` | 100644 | `76be7d9dc62f27767b0a507e4179898bd9a3611f3231a69a6801be60ddda098c` |
| `references/data-over-abstractions.md` | 100644 | `fdfa218c0fea9726fa6276b32c3407e1995a21d99f5f00c45f6e2200fdb6f213` |
| `references/design-is-taking-apart.md` | 100644 | `62694edb44965c50b7a88fc1f891ae38948b2acd1b872d25c2adc988f352ebe0` |
| `references/expensive-to-add-later.md` | 100644 | `e00a5bb7d7f485417f72bc95a0c8629ce571bbf7a6353fe23809515e957b0832` |
| `references/simplicity-vs-easy.md` | 100644 | `b7755a28fdd48e81efb33d257d524c951d33a7bcd4b4d187211d3327943a1da9` |

## Second substantive and risk review (2026-10-08)

All six originals were read in full. **Risk remains high** because the workflow expressly proposes deleting entire features and gives line count precedence. No script, hidden deletion command or malicious payload is bundled.

- **Substantive limitation:** [SKILL.md:35-45](https://github.com/joshuadavidthomas/agent-skills/blob/516dee7a422b90937b2958d11c03694154ab9c09/reducing-entropy/SKILL.md#L35-L45) asks for the smallest codebase solving the problem, but then unconditionally rejects a change when its final line count increases. A necessary correctness/feature change adding a boundary check may therefore be rejected merely for adding code. The listed exceptions do not clearly resolve that rule, and the security/audit recommendations in `expensive-to-add-later.md` create further tension. This is an unsafe decision heuristic, not proof that the skill specifically instructs removing authentication.
- Essays on simplicity, coupling, data and YAGNI are useful opinions and heuristics, not universal scientific guarantees. Those preferences alone are not grounds for rejection.
- Safeguards for any accepted restricted use: agree required behavior and permitted deletions first; preserve public/security/compliance obligations; use line count only after satisfying requirements; keep a version-controlled recovery point; inspect the diff and run relevant behavior checks. No actual feature or project file was deleted during review.

**Second-review disposition before maintainer decision:** hold as an unrestricted automatic refactoring skill. Restricted behavior-preserving simplification may be reasonable only with documented maintainer acceptance and the above operating constraints; accepting deletion risk alone does not cure the decision-rule limitation. Sources must not be repaired locally. MIT eligibility is unchanged. No imported package or catalog row.

## Maintainer decision and final four-package import (2026-10-08)

After the second review was reported, the maintainer explicitly instructed importing only coding-standards, crafting-effective-readmes, diataxis and reducing-entropy. This records acceptance of the disclosed risks and limitations for the unchanged import; it supersedes prior pending-acceptance holds. Risk ratings and findings are retained. Rust and researching-codebases remain excluded.

**Operating safeguards:** Agree required behavior and permitted removals before editing. Preserve security/compliance/public contracts; line count is a secondary heuristic and must not reject required fixes. Keep a version-controlled recovery point, review deletion diffs and verify behavior. Imported prose grants no new authority for external operations or deletion.

**Verification:** the final four-package scope contains 50 original files and eight separately recorded exact license notices (58 entries). Complete inventory, bytes and modes are compared with immutable upstream Git blobs in the working tree, index and committed tree. Package-specific `-text` prevents line-ending conversion. No original file, name, reference, example or frontmatter is modified; documented template, link and correctness limitations are preserved.
