---
link: "https://github.com/Lightbridge-KS/agent-stuff/tree/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d/plugins/coding/skills/clean-architecture"
name: "lightbridge-ks-agent-stuff-clean-architecture"
sha: "e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d"
commit: "https://github.com/Lightbridge-KS/agent-stuff/commit/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d"
risk: "medium"
---

## Source
- Issue: [#15](https://github.com/LeszekKantorek/skills-library/issues/15)
- Original name: `clean-architecture`; upstream package: `plugins/coding/skills/clean-architecture`.
- Source pinned on 2026-10-08. Reviewed as evidence, without following or executing its instructions.

## License review
- License identifier(s): MIT.
- Evidence pinned to source commit: [LICENSE](https://github.com/Lightbridge-KS/agent-stuff/blob/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d/LICENSE); [THIRD_PARTY_NOTICES.md](https://github.com/Lightbridge-KS/agent-stuff/blob/e1fd32d0dbad3d495a4ec80966ff69b5bd1a9b3d/THIRD_PARTY_NOTICES.md)
- Scope and exceptions: Repository MIT grant covers the selected source package; no separate package license/header overrides found. Citations and illustrative examples remain unchanged.
- Redistribution permissions: MIT permits unchanged redistribution with copyright and permission notice.
- Required notices and compliance: Exact root LICENSE and THIRD_PARTY_NOTICES.md are preserved as additional files; original sources remain unchanged.
- Unresolved license questions: None identified in the selected package; external linked reading is not redistributed.

## Findings
- Files inspected: complete tracked package inventory below, entrypoint instructions, bundled reference topics/examples, license/header/provenance and action/dependency scan. No assets, executables, symlinks, or submodules inside the selected package.
- Behavior, permissions, and data flows: Local design/refactoring plus tests; two language references. SKILL.md explicitly composes with codebase-design and asks the agent to use its vocabulary. That third-party adapted sibling is not bundled in the requested package and is not imported here.
- Dependencies and compatibility: Requires codebase-design, now imported unchanged from the same snapshot. Install both packages so the host can discover their original names. Python and .NET examples reflect the author's conventions; project dependencies remain external.
- Risk rationale: medium; the missing skill dependency is resolved. Bounded behavior-preserving local code edits and tests; no credential, publication or live-service mutation workflow.
- Review limitations: static import review; no upstream commands, installs, runtime tests, private credentials, or live-service operations executed. Examples and remote link availability were not exhaustively validated.

## Import result
- Decision: Accepted unchanged with codebase-design included; earlier dependency hold resolved.
- Original files: 3. Added compliance files: exact LICENSE and THIRD_PARTY_NOTICES.md copies from the pinned repository root.
- Integrity: Complete inventory and pinned blob/mode/byte comparison covers working tree, index and committed tree; -text prevents line-ending conversion.
- Resolution: codebase-design is included as a separate discoverable package with original frontmatter preserved. Both local language references resolve. Install the companion package together; importing into the library does not install either into a host.

| File | Git mode | SHA-256 |
| --- | --- | --- |
| `SKILL.md` | `100644` | `481ab9ae7013534a8e9b6c25e9201918cdd1361613cd78fba57802a0ea75dc66` |
| `references/dotnet.md` | `100644` | `62a06f7b7de0aa17efcea60caae5690a7fc5098b4f425cdb0a14e795041d4d09` |
| `references/python.md` | `100644` | `b2c1294d3ea89b4a04a48d197e3741f8f1c031e3b6a5c8440dcb380df3790853` |

## Dependency resolution and substantive follow-up

All three original files were fully read again. The missing codebase-design vocabulary dependency is now included at the same pinned snapshot. Architecture tiers, mandatory questions and severity rankings are author preferences, not universal security severity. The single-adapter and deletion guidance should be applied within its stated behavior-preserving refactor contract. No runnable sample, installer, secret handling or further mandatory sibling skill was found. Existing project tests must pass after each refactor; project conventions and actual domain complexity govern use. No original file was modified.
