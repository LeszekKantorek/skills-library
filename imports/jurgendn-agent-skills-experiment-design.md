---
link: "https://github.com/jurgendn/agent-skills/tree/f290312fb6c55a044402e8649afff5c112e660ab/skills/research-experimentation/experiment-design"
name: "jurgendn-agent-skills-experiment-design"
sha: "f290312fb6c55a044402e8649afff5c112e660ab"
commit: "https://github.com/jurgendn/agent-skills/commit/f290312fb6c55a044402e8649afff5c112e660ab"
risk: "medium"
---

## Source

- Issue: https://github.com/LeszekKantorek/skills-library/issues/22
- Original name: `experiment-design`.
- Retrieved: 2026-10-21 (Europe/Warsaw).

## License review

- License identifier(s): none found; unlicensed snapshot.
- Evidence: [pinned repository tree](https://github.com/jurgendn/agent-skills/tree/f290312fb6c55a044402e8649afff5c112e660ab) and [package](https://github.com/jurgendn/agent-skills/tree/f290312fb6c55a044402e8649afff5c112e660ab/skills/research-experimentation/experiment-design). Tracked inventory contains no LICENSE/COPYING file. Repository-wide searches for licensing, copyright and redistribution terms found no license grant covering these packages. Package files contain no separate license notice.
- Scope and file-specific exceptions: no applicable terms identified; no redistribution grant established. Public availability and attribution are not permission.
- Redistribution permissions: unresolved.
- Required notices and other obligations: cannot determine without terms from the rights holder.
- Preserved license/attribution files and compliance actions: no source license available to copy. Added library-authored `SOURCE.md` identifies repository, original path, full commit and retrieval date, and explicitly records the absence of a license.
- Maintainer decision: in this chat on 2026-10-21, the maintainer explicitly requested import with SOURCE.md when a license is missing. Proceeded under that instruction, overriding the curator's default license hold. This does not resolve or represent a license grant. Obtain rights-holder permission or a covering upstream license before relying on redistribution permission.

## Findings

- Files inspected: all original files listed below, plus repository file inventory and repository-wide license-term search.
- Behavior, permissions, and data flows: Instructions recommend experiment planning, sanity training runs and a bundled local scaling fitter. The script reads command-line arrays or a caller-specified JSON file, uses NumPy and scipy.optimize.curve_fit, and prints reports. No network calls, subprocesses, credential access, deletion or file writes appear in the script.
- Dependencies: Optional Python 3 script requires NumPy and SciPy, not bundled; dependencies were not installed. The stale scaling-law-tracker name appears only in the script docstring and is not an operational skill dependency.
- Risk rationale: `medium` based on the recommended actions above; licensing uncertainty is tracked separately. No malicious override, hidden destructive behavior or safeguard bypass found in these files.
- Compatibility: package-local resources exist; original frontmatter name retained. No collision with existing original skill names. No required external skill dependency found. Scientific correctness and task-specific environments were not validated.

## Import result

- Decision: imported unchanged at the maintainer's explicit direction, with unresolved redistribution permissions recorded above.
- Source file integrity: original Git blobs copied in binary mode; working-tree SHA-256 and staged/committed blob IDs and modes checked against the pinned source.
- Added license/attribution files: library-authored SOURCE.md only; it is not an upstream file or license.
- Checks performed and limitations: full original inventory, file bytes, Git modes, frontmatter, package-local references and catalog/review consistency. No upstream code or installer executed; no training, dependency installation, numerical validation or live external-link check performed.

| Original path | Git mode | Upstream Git blob | SHA-256 |
| --- | --- | --- | --- |
| `SKILL.md` | `100644` | `903c919e39b91570018498c3107f765e30089bac` | `771751b38ca0100584d1f96eb33a7fb0cb4810d977383cc67d53dc4228250e3e` |
| `references/experiment-design-checklist.md` | `100644` | `2256beaf6de89dab28e637392d22dfc9b7126929` | `36720f280f8690ada7201c334adc4f3577a87035fdd06559502d6dedd3fd1ffa` |
| `scripts/fit_scaling_law.py` | `100755` | `167165e064935e4a494d5d0a75b56d2fb4679361` | `e4972d270221ceb9c478cddc9aea554abd2e256eb220b503b4d922ef2cffd833` |
