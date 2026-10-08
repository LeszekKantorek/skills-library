---
link: "https://github.com/Lightbridge-KS/agent-stuff/tree/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d/plugins/coding/skills/codebase-design"
name: "lightbridge-ks-agent-stuff-codebase-design"
sha: "e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d"
commit: "https://github.com/Lightbridge-KS/agent-stuff/commit/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d"
risk: "medium"
---

## Source
- Issue: [#15](https://github.com/LeszekKantorek/skills-library/issues/15); added to PR #17 to resolve the requested clean-architecture dependency.
- Original name: codebase-design. All three original files fully read at the same immutable snapshot as clean-architecture.

## License review
- License identifier: MIT.
- Evidence: [root LICENSE](https://github.com/Lightbridge-KS/agent-stuff/blob/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d/LICENSE) and [THIRD_PARTY_NOTICES.md](https://github.com/Lightbridge-KS/agent-stuff/blob/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d/THIRD_PARTY_NOTICES.md).
- Root notice identifies Kittipos S.; codebase-design is explicitly listed as adapted from mattpocock/skills. The notice reproduces Matt Pocock's MIT grant. Original attribution footer is retained.
- Unchanged redistribution is allowed with applicable copyright and permission notices; exact root LICENSE and THIRD_PARTY_NOTICES.md are added without overwriting originals. No license blocker remains.

## Findings
- Files inspected: SKILL.md, DEEPENING.md and DESIGN-IT-TWICE.md, plus both license/notice files; no bundled script, binary, symlink, installer, credential access, network upload or service mutation.
- Behavior: local interface design/refactoring and behavior-oriented testing. DEEPENING recommends deleting old unit tests only after replacement interface tests exist. This is scoped reversible source editing, not arbitrary file/data/feature deletion; preserve required regression coverage before removing tests.
- Dependencies: the core shared vocabulary and both local reference links work unchanged. codebase-blueprint is an alternate task route, not a mandatory dependency. CONTEXT.md is project-provided domain vocabulary for the optional design exercise, not a missing bundled asset.
- Optional alternative-interface exploration requests 3+ parallel agents and an Agent tool. The exact tool spelling is host-specific; use a compatible authorized host agent interface. This does not require further imported skill packages, and is not executed by importing the Markdown.
- Risk: medium for bounded reversible project refactors and tests. The terms and one/two-adapter rules are design heuristics, not universal necessity; a useful indirection may serve compatibility, policy or ownership even with one implementation. Private tests and local substitutes do not by themselves prove production-adapter equivalence.
- Review limits: static review of all files and original examples; no host multi-agent exercise, project refactoring or dependency installation performed. No claim of universal applicability or exhaustive correctness certification.

## Import result
- Decision: accepted unchanged as the dependency requested by the maintainer; no high-risk acceptance requirement is invented.
- Source integrity: complete upstream inventory, bytes and Git modes verified in working tree, staged and committed contents. Three originals plus two exact notice additions. Package-specific -text prevents conversion.
- Safeguards: preserve required public/persisted behavior and regression coverage; only remove old tests after adequate replacement; review local diffs and validate actual runtime behavior; follow existing user authorization for agent delegation and external operations.

## Original inventory

| File | Mode | SHA-256 |
| --- | --- | --- |
| `DEEPENING.md` | 100644 | `125e6b77413ad2bc7cf7a772bc74336d580a50f9e797db2178ed133d62333d06` |
| `DESIGN-IT-TWICE.md` | 100644 | `21c3264953bd30ee87b181a3ccaf0e70649f461e5ffd7dc654acee4ba1788b31` |
| `SKILL.md` | 100644 | `8fe698cbad8a6afe1777286eea99a02c413e497009bc96a798ffc9920a1354dd` |
