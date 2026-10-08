---
link: "https://github.com/joshuadavidthomas/agent-skills/tree/516dee7a422b90937b2958d11c03694154ab9c09/crafting-effective-readmes"
name: "joshuadavidthomas-agent-skills-crafting-effective-readmes"
sha: "516dee7a422b90937b2958d11c03694154ab9c09"
commit: "https://github.com/joshuadavidthomas/agent-skills/commit/516dee7a422b90937b2958d11c03694154ab9c09"
risk: "high"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/14 (no comments or special acceptance at review time).
- Original name: `crafting-effective-readmes`; original frontmatter preserved for accepted packages.
- Snapshot: `516dee7a422b90937b2958d11c03694154ab9c09`; resolved upstream main on 2026-10-08. Downloaded outside automatic skill discovery. The issue's researching-codebases blob URL refers to a directory; resolved to the existing tree without expanding requested scope.

## License review
- License identifier(s): MIT; CC-BY-2.0.
- Repository evidence: [MIT LICENSE](https://github.com/joshuadavidthomas/agent-skills/blob/516dee7a422b90937b2958d11c03694154ab9c09/LICENSE), Copyright (c) 2025 Josh Thomas.
- Scope and file-specific exceptions: Mixed license package: references/art-of-readme.md credits hackergrrl/art-of-readme (Kira) and ends with a CC-BY-2.0 link. Danny Guo make-a-readme material is MIT at [6d9e22931e3bb0c6b926a7bb396d371f78e6e719](https://github.com/dguo/make-a-readme/blob/6d9e22931e3bb0c6b926a7bb396d371f78e6e719/LICENSE); Standard README material is MIT at [5d18ad4db6a39fde5dc845258828153eda9828e8](https://github.com/RichardLitt/standard-readme/blob/5d18ad4db6a39fde5dc845258828153eda9828e8/LICENSE). These grants permit redistribution with their required notices/attribution retained. A future import must add exact MIT notices for Josh Thomas, Danny Guo and Richard Littauer and preserve the original CC attribution/license link. Examples saying Richard McRichface are illustrative, not a substitute for Littauer notice.
- Redistribution permissions: MIT permits unchanged redistribution when copyright/permission notice is included; mixed packages retain the additional license scopes described above.
- Required notices and other obligations: preserve all original attribution and applicable license copies; never modify original imported sources or imply endorsement.
- Preserved license/attribution files and compliance actions: None redistributed. Applicable additional notice copies identified in License review for any future accepted import.
- Unresolved questions or blockers: The operational acceptance/compatibility blockers below are separate from license eligibility.

## Findings
- Files inspected: complete 13-file inventory below; README/SKILL, references/templates/agent definitions and scripts included, with operation-bearing content reviewed explicitly. Static scans inspected all file contents. External source content treated only as evidence, never executed as instructions.
- Behavior, permissions, and data flows: Core workflow reads local project metadata and writes README drafts using four supplied templates. However references/standard-readme-spec.md recommends using gh-description to set and get GitHub repository description, a real external service metadata change. It also suggests hosted badges and remote package metadata reads. Placeholder deployment/runbook sections are template content, not executed commands.
- Dependencies: No bundled scripts. Optional style-guide.md delegates general prose guidance to an unbundled writing skill; this does not prevent the core README workflow. Optional gh-description needs GitHub authorization and npm show needs network. Existing broken contextual reference links in copied Standard README examples/specification are documentary examples, not core package dependencies.
- Risk rationale and assessment gaps: high according to the highest applicable documented behavior. All 13 files inventoried and statically inspected for licensing, links, templates and behavior; core workflow and remote-operation/license-bearing references inspected directly. No commands executed. Third-party licenses identified; no actual redistribution performed.

## Import result
- Source file integrity: Not imported or staged. The immutable upstream inventory below records SHA-256 and Git mode for every original file. No imported-blob comparison is claimed for a review-only hold.
- Added license/attribution files and their provenance: None redistributed. Applicable additional notice copies identified in License review for any future accepted import.
- Checks performed and limitations: immutable Git snapshot and complete file/mode inventory; UTF-8/frontmatter names; local Markdown links and inline path references; license/attribution scope; static code/behavior and dependency scans; review/catalog consistency. No upstream code or instructions executed. All 13 files inventoried and statically inspected for licensing, links, templates and behavior; core workflow and remote-operation/license-bearing references inspected directly. No commands executed. Third-party licenses identified; no actual redistribution performed.
- Decision and blockers: Review-only hold: remote repository-description writes require explicit maintainer acceptance of safeguards. Proposed safeguards: local drafts by default, never place secret values in README, obtain task-specific authorization before remote metadata changes, restrict gh-description credentials to the intended repository, show exact new description before submission. Maintainer acceptance has not been provided. No skills directory or catalog entry.

## Original file inventory

| Original relative path | Git mode | SHA-256 |
| --- | --- | --- |
| `SKILL.md` | 100644 | `638b271fdc148249ed8896dbdcf15f9067a8d64ba7d2d82ec3e86f8d82831b51` |
| `references/art-of-readme.md` | 100644 | `8ca299e44ce728bd5e15803b1414b893c52ff67aed1d395181a789a5b7c98123` |
| `references/make-a-readme.md` | 100644 | `81b1d33bc39b53dd8444c627fb7a5424a6a1272507a3f03e1a13c4bc03761057` |
| `references/standard-readme-example-maximal.md` | 100644 | `75133e20217c8a431ab33d42c53e22a69bb5a57828cea6dfd2c93c1bc8693ba2` |
| `references/standard-readme-example-minimal.md` | 100644 | `1377439694911b257ed0ced67efd8b46212c9f05e1d831730fa3ff7180fcd162` |
| `references/standard-readme-spec.md` | 100644 | `e1b5584f15ed13e60442ff78e4989af7b6934c42330faa6fe567e9757aafbb22` |
| `section-checklist.md` | 100644 | `e9da988cb2f4ec9f9bb830e7e39e161ff7053c80d55f2c6f043fa2beaf4b777b` |
| `style-guide.md` | 100644 | `e77c67e73c9d80ff7147233009581fe2a62f0b0ca038158f715433c9b52c2e4b` |
| `templates/internal.md` | 100644 | `6d2d0ac208385fa97f5753608f3a941411f40daaa1901fb60021d29ed24c6ff0` |
| `templates/oss.md` | 100644 | `4e92c24937dee83f1d7fe7b8265ddaf91e5f1b1ae6808e1863f704d94949fa74` |
| `templates/personal.md` | 100644 | `2aea82c27a5f779b4cd4d67c3d5c08fc4c6ed476a18298ca7b3070f8a7ec6714` |
| `templates/xdg-config.md` | 100644 | `129095375dedfc2856bf68b561d7968c57aae433721f5ac412442e51ff94abc5` |
| `using-references.md` | 100644 | `de80ec04ef24a43fdb205d47883efcc544acc6e179f8c072c54778f663045ce6` |
