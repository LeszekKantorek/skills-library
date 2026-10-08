---
link: "https://github.com/magnus919/agent-skills/tree/3c946d99ce4e17d8e430eaa37f554d96f65f575a/qa-methodology"
name: "magnus919-agent-skills-qa-methodology"
sha: "3c946d99ce4e17d8e430eaa37f554d96f65f575a"
commit: "https://github.com/magnus919/agent-skills/commit/3c946d99ce4e17d8e430eaa37f554d96f65f575a"
risk: "high"
---

## Source

- Issue: [#13 — Import: qa-methodology](https://github.com/LeszekKantorek/skills-library/issues/13), one requested package and no issue comments at review time.
- Original name: `qa-methodology`; original metadata identifies skill version `2.0.0` and `source_repo: hermes-profiles`. These upstream values will remain unchanged; the source actually reviewed is the pinned `magnus919/agent-skills` snapshot above.
- Reviewed on 2026-10-08. The immutable snapshot contains 37 package files, all regular Git blobs with mode `100644`; no symlinks, submodules, binary assets, or executable-mode files occur in this package.

## License review

- License identifier: **MIT**.
- Evidence: pinned [repository LICENSE.md](https://github.com/magnus919/agent-skills/blob/3c946d99ce4e17d8e430eaa37f554d96f65f575a/LICENSE.md) and [SKILL.md license declaration](https://github.com/magnus919/agent-skills/blob/3c946d99ce4e17d8e430eaa37f554d96f65f575a/qa-methodology/SKILL.md).
- Scope and file-specific exceptions: root MIT license applies to the package; copyright is `Copyright (c) 2026 Magnus Hedemark`. No package-specific LICENSE/COPYING, conflicting headers, separate third-party license files, vendored implementations, or separately licensed binary assets were found among all 37 inspected files. References include attributed sources and illustrative snippets, rather than bundled copies of the cited tools or papers.
- Redistribution permissions: MIT permits redistribution of the unchanged package under the library directory name.
- Required notices and obligations: retain the copyright, permission notice, and disclaimer in copies/substantial portions. No copyleft source-sharing requirement or change notice applies to this unchanged import.
- Compliance action prepared: exact source `LICENSE.md` copy, added separately from the 37 originals in the local review snapshot. On acceptance it will be included as `skills/magnus919-agent-skills-qa-methodology/LICENSE.md`, without overwriting any original.
- Unresolved license questions or blockers: none identified. The import hold below is a risk-acceptance decision, separate from redistribution eligibility.

## Findings

### Files inspected

The complete package was inspected as external evidence, without treating its instructions as authorization:

- `SKILL.md`, `README.md`, `pytest.ini`, `evals/evals.json`.
- `assets/`: `qa-definition-of-done.md`, `risk-matrix-grid.md`, `test-design-techniques-checklist.md`.
- `references/`: `agent-ui-navigation.md`, `agentic-eval-design.md`, `ai-code-quality-gates.md`, `ai-test-artifact-evidence.md`, `ci-failure-triage.md`, `exploratory-testing.md`, `performance-testing.md`, `qa-career-levels.md`, `quality-gates-and-metrics.md`, `regression-testing.md`, `risk-based-testing.md`, `sdet-engineering.md`, `security-testing.md`, `test-automation.md`, `test-data-management.md`, `test-debugging.md`, `test-design-techniques.md`, `test-strategy.md`.
- `scripts/`: `check-ac-testability.py`, `risk-prioritize.py`.
- `templates/`: `agent-ui-run-record.md`, `ai-assisted-verification-note.md`, `bug-report.md`, `exploratory-charter.md`, `mutation-review.md`, `risk-register.md`, `test-strategy.md`, `verification-plan.md`.
- `tests/`: `test_check_ac_testability.py`, `test_risk_prioritize.py`.

### Behavior, permissions, and data flows

- The two bundled CLIs use Python's standard library only. They read a user-selected UTF-8 local file or stdin and emit rankings/testability findings to stdout/stderr with documented exit codes. They contain no network requests, process spawning, environment/credential reads, writes, deletion, or dynamic evaluation. The AC scanner prints criterion text, so sensitive input could appear in terminal logs; it is a linguistic heuristic, not proof of functional correctness.
- Bundled tests spawn those two known scripts using the current Python interpreter, supply synthetic inputs, create temporary `.md`/`.json` files, read them back, and unlink only the files they created. They also list the temporary directory to check artifacts. No real services or credentials are needed for these tests.
- Recommended agent actions go beyond those CLIs. [Test data management](https://github.com/magnus919/agent-skills/blob/3c946d99ce4e17d8e430eaa37f554d96f65f575a/qa-methodology/references/test-data-management.md) includes create/drop test schemas, `TRUNCATE ... CASCADE`, migrations and rollback. [Security testing](https://github.com/magnus919/agent-skills/blob/3c946d99ce4e17d8e430eaa37f554d96f65f575a/qa-methodology/references/security-testing.md) includes DAST, fuzzing, credential/access-control tests, and secret/history scanning. [Performance testing](https://github.com/magnus919/agent-skills/blob/3c946d99ce4e17d8e430eaa37f554d96f65f575a/qa-methodology/references/performance-testing.md) includes load/stress/soak traffic and an illustrative `https://staging.example.com/api/items` target.
- CI and SDET references recommend installing third-party tools, modifying CI configuration, quarantining/deleting tests, publishing Pact contracts, and canary/rollback workflows. UI navigation scenarios can create synthetic orders or other persistent effects. Agent-eval references discuss transmitting inputs to LLM graders and capturing production transcripts with consent and anonymization. These require project-specific permissions and can affect external systems; importing the skill must not silently authorize them.
- Existing safeguards are meaningful: synthetic/masked data and **no production PII**, fake credentials, mocked external services rather than real buckets, independent verification, immutable oracles, finite mutation/repair budgets, identity checks, reconciliation before uncertain UI retries, redaction, and stopping on real vulnerabilities. No hidden exfiltration endpoint, instruction override to bypass host safeguards, or concealed destructive payload was found.

### Dependencies and portability

- Core QA guidance, templates, assets, and both CLIs are usable unchanged without a named CI platform, test framework, or model. Scripts declare Python 3.8+; tests use `unittest` and standard-library subprocess/tempfile helpers. Python 3.8 itself was not available for a runtime test; the actual checked runtime was Python 3.14.
- Cross-skill routing names are preserved: `systematic-debugging`, `secure-software-engineering`, `playwright`, `spec-driven-development`, `agent-evals-and-observability`, `verification-methodology`, `release-engineering`, `web-accessibility`, and `system-one`. Their original sibling relative paths do not resolve in an isolated package or under this library's owner-repository-skill naming scheme. Existing differently named imports do not satisfy those literal filesystem links. The link check identified 38 such routing/composition occurrences and no missing package-internal Markdown targets.
- The siblings cover excluded domains and optional compositions rather than mandatory startup/runtime dependencies for the core skill. Formal SDD gate ownership, external verification verdicts, accessibility mechanics, and optional System One model integration need separately reviewed compatible capabilities; these workflows must stop at unavailable routing/access boundaries. No sibling was installed, copied, or patched into this request.
- README quick-start commands contain the original `qa-methodology/` directory prefix. They assume the original upstream layout; callers of a future renamed library package must invoke its actual path. Original text and frontmatter will not be adapted.
- Illustrative pytest/Playwright/Pact/k6/security-tool configurations require the target project's installed tools and policies. They were statically inspected, not executed against services. External citations/tool/version claims were not individually revalidated; this review assesses source behavior and redistribution, not empirical correctness of every methodology claim.
- Preserved upstream inconsistency: the risk matrix grid labels score `16` as `P0`, whereas its zone thresholds and risk tier definitions classify `12–19` as `P1`. The CLI computes raw P×I ranks without tiers; consumers should independently qualify their tier policy. No source correction is proposed.

### Risk rationale and proposed safeguards

**High** is assigned because the recommended workflow includes database deletion/reset, active network/security testing, CI/service changes, external contract publication, and model/transcript transmission. This is based on concrete source actions, not missing example-framework executions. The bundled CLIs alone have a narrower read-only behavior.

Proposed acceptance boundaries, maintained outside imported sources:

1. Start with local QA design and the two reviewed CLIs; use synthetic, non-sensitive input and redact retained reports. Never feed real credentials or production PII to tools/models.
2. Execute tests only in explicitly authorized, isolated test environments/accounts with named targets and finite load/fuzz/mutation/repair budgets. No production load/security probing or real payments/email/object-storage effects under generic skill invocation.
3. Allow schema drop/truncate/reset only for verified disposable test data with rollback/recreation arrangements. Resolve the exact account/database/path before mutation and stop on identity ambiguity or uncertain commit state.
4. Require separate explicit task authorization for CI/policy changes, contract publishing, production capture/transmission, canary/deployment/rollback, and deletions beyond disposable test fixtures. Preserve project approval and branch-protection requirements.
5. Qualify third-party tools and model providers against the target project's manifests/policies; do not auto-install missing siblings or bypass unavailable verification/routing capabilities. Protect independent oracles and require human/independent evidence for high-impact decisions.

Maintainer acceptance of this high-risk package and these boundaries is **pending**. General authorization to prepare import PRs is not recorded as acceptance of these consequential workflows or compatibility limitations.

## Import result

- **Decision: held pending explicit maintainer risk acceptance; review-only draft PR.** No `skills/` package, catalog entry, or package `.gitattributes` rule is submitted while held. No existing imports or catalog rows are modified.
- Integrity preparation: the complete 37-file package was reconstructed outside automatic skill discovery from pinned Git blobs using binary writes and compared byte-for-byte with those blobs. Git modes were inventoried as `100644` for every original; the exact root MIT license is the only additional prepared package file. Source files were not modified, including frontmatter, paths, line endings, metadata, or cross-skill references.
- Tests actually performed after inspection: `python -I -B -m unittest discover -s <prepared-package>/tests -v` on Python 3.14, with a minimal allowlisted environment, no injected credentials, synthetic test data, temporary files confined to a separate local test directory, and bytecode disabled for the process/children. **46 tests passed**, exit 0. A post-test exact inventory/byte comparison passed again: 37 originals + one license, no generated package files.
- Additional checks: JSON parse/schema/required fields and unique IDs for all 21 output-quality eval cases; package-internal Markdown targets; external sibling routing; license scope; complete inventory/path containment and Git modes. Model output-quality evals, live UI tests, load/DAST tests, deployment, and third-party example toolchains were not run.
- Staged/committed original-file integrity is **not applicable yet** because no original package is submitted in this held review. Before accepting an import, add scoped `/skills/magnus919-agent-skills-qa-methodology/** -text` protection against `core.autocrlf`, then verify worktree, staged and committed blobs, complete inventory, and modes against this snapshot, including the added license. Only then add the direct package installation URL and catalog summary.
- Required next decision: maintainer accepts or declines the high-risk behavior and proposed safeguards, with acknowledged unchanged optional-routing and tier-policy limitations. Acceptance would permit completion on this same branch; it would not itself authorize merge or live service actions. Until then, keep the issue/PR open with only the `blocked` label and do not merge.
