# Felix Geelhaar's expert skills

[felixgeelhaar/skills](https://github.com/felixgeelhaar/skills) is a collection of advisory prompts. The reports below cover only the named items at the versions recorded in each report; they do not assess the whole repository or other skills.

* [AI expert](ai-expert.md)
* [Business operations expert](bizops-expert.md)
* [Life and leadership coach](coach-expert.md)


## Installation

The [upstream README](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/README.md#installation) gives this Claude Code shell example, requiring Git and a shell with `ls`, `xargs`, `mkdir`, and `cp`:

**Warning:** This command clones the full repository from its moving default branch and copies every matching skill into user-level Claude Code directories. It can overwrite existing `SKILL.md` files and does not install the assessed commit reliably.

```bash
git clone https://github.com/felixgeelhaar/skills.git /tmp/expert-skills
for skill in $(ls -d /tmp/expert-skills/*/SKILL.md | xargs -I{} dirname {} | xargs -I{} basename {}); do
  mkdir -p ~/.claude/skills/$skill
  cp /tmp/expert-skills/$skill/SKILL.md ~/.claude/skills/$skill/SKILL.md
done
```

Run from a shell on the target machine. It clones the full repository into `/tmp/expert-skills` and copies every matching skill into the user's `~/.claude/skills/`, not just this one. `cp` can overwrite existing files. The clone uses the default moving branch; it does not pin this reviewed commit. The Git and shell utilities are independently supplied and were not assessed or run. The README also describes copying a skill into agent rules or prompts, with scope depending on the destination. No source-documented command to install only this item at a pinned revision was verified.


## License

The pinned [repository LICENSE](https://github.com/felixgeelhaar/skills/blob/5a2e3ad8d9f7ddbfd15df295ede6c484dfbd6447/LICENSE) is MIT, copyright 2024–2026 Felix Geelhaar. It permits use, modification and redistribution subject to retaining the notice and permission text, and disclaims warranties. Rights in third-party quotations and frameworks were not independently cleared.
