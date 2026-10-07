# Instructions for agents

## Preserve imported skills

Import skills as they are, without any modifications. Never change imported sources.

- Copy the complete skill package from an identified, immutable upstream version, preserving every original file byte-for-byte and its relative path and executable permissions.
- Do not edit, rename, translate, reformat, repair, adapt, or remove original files. Preserve frontmatter names, references, links, code, assets, encoding, and line endings exactly as supplied upstream.
- Do not fix missing dependencies, broken references, or compatibility problems inside imported sources. Record findings, limitations, and maintainer decisions in `imports/<name>.md` and `CATALOG.md`.
- The library package directory may use the repository's naming convention; names and paths inside the package must remain unchanged.
- Preserve all original license and attribution files. Add exact copies of applicable upstream license or notice files when required and missing, without overwriting originals; document these additions separately in the import review.
- Verify the complete imported file inventory, bytes, and executable permissions against the pinned upstream snapshot, including committed Git contents. Prevent Git line-ending conversion from changing imported bytes.
- For an upstream update, review and import the new immutable snapshot unchanged. Never patch the imported copy locally.

Follow `.agents/skills/library-curator/SKILL.md` for the import review, licensing, risk assessment, catalog, and pull request workflow.
