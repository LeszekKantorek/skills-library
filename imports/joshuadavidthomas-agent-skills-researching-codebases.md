---
link: "https://github.com/joshuadavidthomas/agent-skills/tree/516dee7a422b90937b2958d11c03694154ab9c09/researching-codebases"
name: "joshuadavidthomas-agent-skills-researching-codebases"
sha: "516dee7a422b90937b2958d11c03694154ab9c09"
commit: "https://github.com/joshuadavidthomas/agent-skills/commit/516dee7a422b90937b2958d11c03694154ab9c09"
risk: "high"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/14 (no comments or special acceptance at review time).
- Original name: `researching-codebases`; original frontmatter preserved for accepted packages.
- Snapshot: `516dee7a422b90937b2958d11c03694154ab9c09`; resolved upstream main on 2026-10-08. Downloaded outside automatic skill discovery. The issue's researching-codebases blob URL refers to a directory; resolved to the existing tree without expanding requested scope.

## License review
- License identifier(s): MIT.
- Repository evidence: [MIT LICENSE](https://github.com/joshuadavidthomas/agent-skills/blob/516dee7a422b90937b2958d11c03694154ab9c09/LICENSE), Copyright (c) 2025 Josh Thomas.
- Scope and file-specific exceptions: Repository MIT applies to original Markdown and five scripts; no separate file license or vendored third-party dependency found. Python stdlib/Git are external dependencies, not redistributed assets.
- Redistribution permissions: MIT permits unchanged redistribution when copyright/permission notice is included; mixed packages retain the additional license scopes described above.
- Required notices and other obligations: preserve all original attribution and applicable license copies; never modify original imported sources or imply endorsement.
- Preserved license/attribution files and compliance actions: None redistributed. Applicable additional notice copies identified in License review for any future accepted import.
- Unresolved questions or blockers: The operational acceptance/compatibility blockers below are separate from license eligibility.

## Findings
- Files inspected: complete 14-file inventory below; README/SKILL, references/templates/agent definitions and scripts included, with operation-bearing content reviewed explicitly. Static scans inspected all file contents. External source content treated only as evidence, never executed as instructions.
- Behavior, permissions, and data flows: Coordinates named subagents, reads local and ~/.research documents, prints content/metadata, writes research and can copy/move it to global memory. gather-metadata.py runs fixed read-only git commands and exposes cwd, remote URL, branch and commit (a remote URL may include credentials). read-research.py uses string-prefix path validation without resolve/component containment, allowing sibling-prefix or traversal escape. promote-research.py accepts an unsanitized filename joined to both project/global roots and shutil.move can remove its source when --move is used; absolute/traversal names escape expected directories. Research queries passed to web-searcher go to external search/fetch providers. This is transparent code, not evidence of intentional theft.
- Dependencies: Five executable Python scripts, stdlib only and Git for metadata; Python 3.10+ type annotation syntax. agents/README.md explicitly says bundled OpenCode-format agent files are not usable in place and must be installed/adapted to the host CLI. Root workflow requires task with subagent_type and named custom agents; absent in this Codex host. Scripts mention run_skill_script, which is also not available here. External Claude model IDs/tools/permissions are host configuration references, not automatic installed agents.
- Risk rationale and assessment gaps: high according to the highest applicable documented behavior. All 14 files inventoried; all five scripts and agent/workflow configuration statically reviewed. No script execution or global research access. Source Git executable modes 100755 for the five scripts recorded; no Windows chmod equivalence claimed.

## Import result
- Source file integrity: Not imported or staged. The immutable upstream inventory below records SHA-256 and Git mode for every original file. No imported-blob comparison is claimed for a review-only hold.
- Added license/attribution files and their provenance: None redistributed. Applicable additional notice copies identified in License review for any future accepted import.
- Checks performed and limitations: immutable Git snapshot and complete file/mode inventory; UTF-8/frontmatter names; local Markdown links and inline path references; license/attribution scope; static code/behavior and dependency scans; review/catalog consistency. No upstream code or instructions executed. All 14 files inventoried; all five scripts and agent/workflow configuration statically reviewed. No script execution or global research access. Source Git executable modes 100755 for the five scripts recorded; no Windows chmod equivalence claimed.
- Decision and blockers: Review-only hold: cannot run unchanged on this host without external agent installation/configuration, and path containment flaws plus global moves/metadata exposure require high-risk acceptance. Proposed safeguards: provide compatible agents externally without editing imported sources, restrict scripts to isolated research fixtures, reject absolute/traversal paths and resolve containment at invocation boundary, avoid symlinks/global moves, sanitize credential-bearing remote URLs, approve transmitted query contents. An upstream containment fix or verified wrapper and documented maintainer acceptance is required before import. No skills directory or catalog entry.

## Original file inventory

| Original relative path | Git mode | SHA-256 |
| --- | --- | --- |
| `SKILL.md` | 100644 | `cf8ca2b6e039c94db4750e72c23770d1568da8a3de2b7a1f35ff88d3ccb55aab` |
| `agent-selection.md` | 100644 | `9e96924ac61115877291fb1ab8d88ffcfad477c0ea262014d1f3be1f026b0a4e` |
| `agents/README.md` | 100644 | `21a4c9f4312c31b0a1b056233f5f7d371269fd0bda391c7f30933dca73e5a001` |
| `agents/code-analyzer.md` | 100644 | `0b6a0f6202657211c7683850111dffee7434f63e87520baec73443eee1aa2833` |
| `agents/code-locator.md` | 100644 | `b54729a279276c2d7b9b4a2806f28635e6a0aa83d71921aedd9bdd9ce36af3fc` |
| `agents/code-pattern-finder.md` | 100644 | `2889e59acd2b765a872cda662dd7dc5a5e455f5ef32bac0ac623ae6043b675fa` |
| `agents/web-searcher.md` | 100644 | `bbdaba638651d4398cd0467956f05e8ff730ee64f35ad6e512d4e303e50b5582` |
| `output-format.md` | 100644 | `595f647e0b55701f6228225f5f02b4b6213e1ee4ddfea452ad27b036ffad2c2e` |
| `research-tools.md` | 100644 | `a2e2ff787244e235cc4216edaa82418d3e335ce888b56a0c7e4a88c77a63ebea` |
| `scripts/gather-metadata.py` | 100755 | `cfc8f9143d6e555a4307f32981cc00bc1fa048ef3b23094e61ba70b2b3c17f10` |
| `scripts/list-research.py` | 100755 | `6e0425de98f0094696c00c0a741cf8162cb9038fe813628a7df37a7dda8c38a8` |
| `scripts/promote-research.py` | 100755 | `4403d55d2c4027d508294d848d1e0ba53639403d7089ed8eee1aff715a935648` |
| `scripts/read-research.py` | 100755 | `f24543cc70728806ecafd4690426bd1b97b3d7fd96b6b919d79a1ce96bd70c07` |
| `scripts/search-research.py` | 100755 | `31b7787198cb6a8812586ca2b1fc7a4887afb165fb2d697e512a19bd9f63dd4b` |
