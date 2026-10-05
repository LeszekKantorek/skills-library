---
link: "https://github.com/magnus919/agent-skills/tree/9b34a87ee729f109019ac604681e5796349ea1b2/programming-principles"
name: "magnus919-agent-skills-programming-principles"
sha: "9b34a87ee729f109019ac604681e5796349ea1b2"
commit: "https://github.com/magnus919/agent-skills/commit/9b34a87ee729f109019ac604681e5796349ea1b2"
risk: "high"
---

## Source
- Issue: https://github.com/LeszekKantorek/skills-library/issues/7
- Original name: programming-principles
- Reviewed: 2026-10-05. Source extracted with git archive at the immutable commit above, outside automatic skill discovery; no source skill was installed or executed.

## License review
- License identifier(s): MIT.
- Evidence links (pinned to the source commit): https://github.com/magnus919/agent-skills/blob/9b34a87ee729f109019ac604681e5796349ea1b2/LICENSE.md
- Derived rule-set license: https://github.com/mattpocock/agent-rules-books/blob/a7d7649044505b9c377c8dca28d2d6a543bc7f8c/LICENSE
- Scope and file-specific exceptions: The package declares MIT and identifies mattpocock/agent-rules-books as its source. Both the containing repository and the upstream rule-set snapshot provide MIT permissions; preserve both notices. Book references are distilled engineering rules, not redistributed books. Refactoring.Guru references explicitly describe paraphrased operational rules and exclude site code, images, and paid course content; those references are distributed under the upstream rule-set MIT license. This is a source-license assessment, not an independent warranty about upstream authorship. No separately licensed bundled executable or asset was found.
- Redistribution permissions: MIT permits copying and redistribution of the package with copyright and permission notices retained.
- Required notices and other obligations: retain the applicable complete copyright, permission, and warranty notices. No copyleft source-sharing obligation or change notice is required by MIT; original package files remain unchanged.
- Preserved license/attribution files and compliance actions: added an exact copy of the source repository LICENSE.md to this package. LICENSE.agent-rules-books is an exact copy of the upstream rule-set license at a7d7649044505b9c377c8dca28d2d6a543bc7f8c, preserving Copyright (c) 2026 Maciej Ciemborowicz. The package LICENSE.md preserves Copyright (c) 2026 Magnus Hedemark. Existing attribution and source links remain unchanged.
- Unresolved questions or blockers: none identified in the inspected license evidence.

## Findings
- Files inspected: full tracked file inventory below; entrypoint, companion documentation/evaluation data, reference guidance, file modes, license/header evidence, paths/links, and static scans for execution, network, secret access, destructive behavior, and instruction overrides.
- Behavior, permissions, and data flows: Markdown guidance for reading code and GitHub context, writing/refactoring code and tests, removing dead code, and recommending automation/deployment/migration practices. The assessment workflow discusses filing GitHub issues. External links identify sources; no automatic transmission, hidden executable, secrets collection, or fixed upload endpoint was found. Full reference policies use binding MUST/OBEY phrasing: this is subordinate task guidance, never permission to override user or project instructions.
- Dependencies: No bundled runtime dependencies. The optional assessment workflow calls skill_view, codebase-inspection (not included), gh, web_extract, and Unix find/grep/head. Generic file reading can load the core and all book references unchanged; the extended workflow requires those host tools/additional skill. Windows-only hosts may lack Unix commands. Frontmatter claims no external dependencies, which does not cover that optional workflow. Do not install missing tooling or import another skill implicitly.
- Risk rationale and assessment gaps: High because recommended actions include deletion of unused code, deployment/operational changes, and potential GitHub issue publication. This rating reflects visible recommended behavior, not malicious payloads or unresolved static assessment gaps. Safeguards: apply only within the requested change, preserve user/project priority, verify callers and behavior before deletion, use disposable test resources, and require explicit authorization for GitHub writes/deployment. Maintainer acceptance of this risk is pending PR review; merging the PR records that acceptance. No symlinks, submodules, executable files, or opaque binary assets in the selected package. This static review does not validate engineering effectiveness or guarantee safe behavior in every consuming project.

## Import result
- Source file integrity: all 34 original files copied from the pinned Git archive and checked by SHA-256; file inventory is complete. Original frontmatter, names, paths, references, encoding, and line endings are unchanged.
- Added license/attribution files and their provenance: LICENSE.md from the pinned containing repository. LICENSE.agent-rules-books is an exact copy of the upstream rule-set license at a7d7649044505b9c377c8dca28d2d6a543bc7f8c, preserving Copyright (c) 2026 Maciej Ciemborowicz. The package LICENSE.md preserves Copyright (c) 2026 Magnus Hedemark. License additions are separate from the original file inventory below and are also byte-checked.
- Checks performed and limitations: tracked regular-file inventory, original-name uniqueness, frontmatter presence, local reference targets, valid evaluation JSON where present, review/catalog consistency, and staged Git-blob identity. Scoped .gitattributes disables text conversion for these packages. The full staged whitespace check reports the pre-existing blank line at EOF in references/refactoring-guru.full-smells-and-priorities.md; it is retained to preserve source bytes. The check passes for library-authored metadata. No installation, test runner, example code, agent evaluation, deployment, or GitHub action from the source skill was executed. External reference URLs are provenance/citation links, not executable dependencies; their ongoing availability is not guaranteed.
- Decision and blockers: accepted for inclusion in the PR with the documented risk and compatibility limitations; no unresolved import blocker. High-risk maintainer acceptance, where applicable, remains pending review and merge of the PR.

## Original file integrity

| Original file | Source Git blob (SHA-1) | Imported SHA-256 |
| --- | --- | --- |
| evals/evals.json | 24d732edd9c511dc003f59b3c0942851bae15834 | 4d37253b9909d70a24782fe4709435b803d4c93773a0e48e98c5b0f5c23167e6 |
| README.md | 31d664e66607eff00b55e583553c67cc9a9f9bf5 | dd02711eda8ab6ffcc73855a3606c8ddb65ca35c4e7db8b40f331ee2b9a9c4c7 |
| references/a-philosophy-of-software-design.full.md | 02d9d5410165937d74c55cd17d9427175180343f | b521814b9d050d0d12594e13aa291029148a971b6f7d5a5ac3e74219de6c8563 |
| references/a-philosophy-of-software-design.mini.md | a7d88383dd909a97b423d5f54d308cb2049e9a5a | ad8d9bd764179c0d2fea95f2bee3e25d443589a12fec84bfead52bdd94b4645a |
| references/clean-architecture.full.md | 8382adb3b3b187c52329ecfd6f0f9dd86850b143 | 1f0366be1720989c63df6da8f15f12e78f8786f6e712eeb16cf3690b4dab6cc4 |
| references/clean-architecture.mini.md | 0f879194b939b9308a5304ff80d542f84520a0f1 | fbead04fa4479bc0d23b8df92e1d04f555e85b9e27994a60209eb311bf342e63 |
| references/clean-code.full.md | 7a07f8935fd6efae6c842c8f65c29a222e0745c7 | 0ec945c383144e2eeb52bdd18cc87668bff73c13421e17cc6e4ba3fc5905965e |
| references/clean-code.mini.md | 26d8320882201ac2f862a3c2e611ff714ef998c8 | a2cd7e30a03376037e441056a5615e7a15c396642daf16f7875a0f5139b65e67 |
| references/code-assessment-workflow.md | cdb20656789c010df43d2d53191f8d6bb3f44b66 | ed5d5ae1db8ebdf647e61435bbf9e33ba4748a4f1b9906be61e8204cc049c439 |
| references/code-complete.full.md | 9636fdab9ae88ccc8999ad7e45064ce535ad95b6 | 57ca8fab93baea0761eeeca6c491fe79b093df47feb4172c0917a96f8ddc95a4 |
| references/code-complete.mini.md | f886e0d5c20cdd0ff024e72e2fe9dff6ce50d1b3 | 88ff0d5bade2b840ae1296b2757a3eee492d505985ea04e4deee158efa127cd7 |
| references/designing-data-intensive-apps.full.md | 1642e3fe05f20f8e75b87de4c895a8e1f813fef4 | 8c1bfe1529076fda8f828ed6939b63bc3016830ad3c705071699a250e98b8f25 |
| references/designing-data-intensive-apps.mini.md | 85be0221f9465bb52c761c2658532df77fa2726b | cb4ca5fa4dc4fe179772f6fc42f4cd8899a7b95677e5cee13602229099063a12 |
| references/domain-driven-design-distilled.full.md | 9d52e0a72b31783175d0724ed4e878e0c8081400 | d665da3c697df36fe04f8bb266381e5b40d158aad5283c1d233d4c47319e5b1c |
| references/domain-driven-design-distilled.mini.md | 07da43f041bd1acf2ab82cdc93e99c58d0da6504 | 45a7976e34feb67628541b03becd44da01d81f7f7e2df0e9fe45e773b7628325 |
| references/domain-driven-design.full.md | 5de1f8b8c1ccce4e0bb33c7d0db9709bc18d65bb | de806ceb828df4408e452361ab587d81f213443ad057017b1f6bed2334d5aaa6 |
| references/domain-driven-design.mini.md | 3275e258ea28dd59022ec32475f15ebfbfad9972 | c29ed300b3d234fa1ae2dbb8233ee20f9795d5d8bb39dbeef1b6e13326f115dc |
| references/implementing-domain-driven-design.full.md | 065c00d6e6148d96029f64ed2e23d3430829f8f1 | cd2c1d404f60720cebca17fcffed9d68d94b1eef4a13bed63a4f59f01db005ad |
| references/implementing-domain-driven-design.mini.md | bbded09713452ec4f547a61cec8af0ee8c9f8a51 | e6688b8380e1e06fbc31cb3c86312527eaca9e1d8cffcd158e5d320581b0b012 |
| references/patterns-of-eaa.full.md | 2f08f321114db1467945ae28473d3b9ea43068f1 | e7f30e7d65005924ec29cc0c6f032aedd0b1bffa22223d5386c5a3140cd76af0 |
| references/patterns-of-eaa.mini.md | b0d73b4b1d7fad100f2f936a7e6dcf6be3ce8249 | 48591b73606b0905e96fb1f1ae74c4d98f240fe49567e21ae578dbbf54d76700 |
| references/refactoring-guru.full-smells-and-priorities.md | 4934d48384d66f1a38bdb538f3fda9ee1b3434f1 | 3366012874b509b8f596d4bf38010588714ba0e95e99984c98ac86b51b4a1f72 |
| references/refactoring-guru.full-technique-playbook-and-safety.md | 87173c982052927aca560c7ab444748bdf5d8029 | 4a59955638ae50142eee9752d2ac18c0e28437a4c8504a79bcf3d4a95a9e2bc9 |
| references/refactoring-guru.full.md | b759abab33720e12a498575a57f59b7e3bf7da61 | 920c208f00b078e985badd87f76609356abf7a138f6978effea5bb6899c1f043 |
| references/refactoring-guru.mini.md | b6f2adc83d8f626d04bd668869e336ca555d541a | a35c914cd5859ccebc45bf7886f0edaca0f9b6070c765bb4b26e23d228b0451d |
| references/refactoring.full.md | 6bcf75c3eda79c38c38f0c18cf7595a00b2cc210 | d7b9cf2b5ca26f3576943ff59cdeee61b65138213777b0e03bfe1075cbd966fc |
| references/refactoring.mini.md | 5fb96556ac7ec7f18d30d22ed8a2487699378932 | 8f4b87f17623283001a984b6735026e4db616c04176f12781fee756f89792a84 |
| references/release-it.full.md | e8e84ca622465899aca32dda00be25544f8eaab1 | ac72b846e9584f376090c8508b2bc66f557ea8d14195ea3b20e15a66b27c4aec |
| references/release-it.mini.md | 10ce0fd98ca1c624f4e859053ef933e6ce2b8dc0 | e5fc51666138115d5f63b06f253da5719de77d55034eb2532ba675d4a43f2ce5 |
| references/the-pragmatic-programmer.full.md | c20070afc6e3a5c8414b0c1253a6e3e19193630c | ea10063caff1989c1442c2aff501a942281fb5b06456e822ab856c701fc5e28d |
| references/the-pragmatic-programmer.mini.md | 22ae23387f8d51bfe82135d30da207a90587e459 | 6e8011e44a38ee6f07d427cfdb27a0e77909645d2da80fc85a8402be74d7a01c |
| references/working-effectively-with-legacy-code.full.md | 74279fd8ed34a9c407f967f97b63a438d76b136f | 8b22bfc3d2851509d4cd8e05fbb9aca9e934f4b6915cb65fe8d6d9d241393fce |
| references/working-effectively-with-legacy-code.mini.md | 1363010311456324796d0b76b6182e8fd27913e9 | 613e3d04ff6377363b674a36cb4bcdd26ce70140695e128b03bfa60fabd19fef |
| SKILL.md | 43184cf160d1e73a681e948cfa430f63599085ae | 0a5f9d1365f17c70403b63d2732460d4360f6e5e55e2fad39fbed696ae885395 |
