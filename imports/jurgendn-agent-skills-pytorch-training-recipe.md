---
link: "https://github.com/jurgendn/agent-skills/tree/f290312fb6c55a044402e8649afff5c112e660ab/skills/research-engineering/pytorch-training-recipe"
name: "jurgendn-agent-skills-pytorch-training-recipe"
sha: "f290312fb6c55a044402e8649afff5c112e660ab"
commit: "https://github.com/jurgendn/agent-skills/commit/f290312fb6c55a044402e8649afff5c112e660ab"
risk: "medium"
---

## Source

- Issue: https://github.com/LeszekKantorek/skills-library/issues/22
- Original name: `pytorch-training-recipe`.
- Retrieved: 2026-10-21 (Europe/Warsaw).

## License review

- License identifier(s): none found; unlicensed snapshot.
- Evidence: [pinned repository tree](https://github.com/jurgendn/agent-skills/tree/f290312fb6c55a044402e8649afff5c112e660ab) and [package](https://github.com/jurgendn/agent-skills/tree/f290312fb6c55a044402e8649afff5c112e660ab/skills/research-engineering/pytorch-training-recipe). Tracked inventory contains no LICENSE/COPYING file. Repository-wide searches for licensing, copyright and redistribution terms found no license grant covering these packages. Package files contain no separate license notice.
- Scope and file-specific exceptions: no applicable terms identified; no redistribution grant established. Public availability and attribution are not permission.
- Redistribution permissions: unresolved.
- Required notices and other obligations: cannot determine without terms from the rights holder.
- Preserved license/attribution files and compliance actions: no source license available to copy. Added library-authored `SOURCE.md` identifies repository, original path, full commit and retrieval date, and explicitly records the absence of a license.
- Maintainer decision: in this chat on 2026-10-21, the maintainer explicitly requested import with SOURCE.md when a license is missing. Proceeded under that instruction, overriding the curator's default license hold. This does not resolve or represent a license grant. Obtain rights-holder permission or a covering upstream license before relying on redistribution permission.

## Findings

- Files inspected: all original files listed below, plus repository file inventory and repository-wide license-term search.
- Behavior, permissions, and data flows: Instructions recommend implementing and executing staged training checks, generating configs, logging and checkpoints. These imply local writes and compute use. No bundled executable, credential lookup, remote logging service, publication or deletion is specified.
- Dependencies: Task-selected PyTorch or Lightning training environment and data; these are not bundled.
- Risk rationale: `medium` based on the recommended actions above; licensing uncertainty is tracked separately. No malicious override, hidden destructive behavior or safeguard bypass found in these files.
- Compatibility: package-local resources exist; original frontmatter name retained. No collision with existing original skill names. No required external skill dependency found. Scientific correctness and task-specific environments were not validated.

## Import result

- Decision: imported unchanged at the maintainer's explicit direction, with unresolved redistribution permissions recorded above.
- Source file integrity: original Git blobs copied in binary mode; working-tree SHA-256 and staged/committed blob IDs and modes checked against the pinned source.
- Added license/attribution files: library-authored SOURCE.md only; it is not an upstream file or license.
- Checks performed and limitations: full original inventory, file bytes, Git modes, frontmatter, package-local references and catalog/review consistency. No upstream code or installer executed; no training, dependency installation, numerical validation or live external-link check performed.

| Original path | Git mode | Upstream Git blob | SHA-256 |
| --- | --- | --- | --- |
| `SKILL.md` | `100644` | `d4c646c39a8393d4306e55ed797c0daa5b02ee91` | `51e5d0d6ac3244e3abe774d3acc45922e0b8d7acb7ce058c9766bdcee93e13bb` |
| `references/training-recipe-details.md` | `100644` | `172f797dfb057fb2d8260e9ddda8c43113c0ddd5` | `63841f8ecafebc28c2559a5406fa66aea362886965dedc7282fce46b9bc06f27` |
