# magnus919/agent-skills

[magnus919/agent-skills](https://github.com/magnus919/agent-skills) provides agent skills. The reports cover only the named items and recorded versions, not the whole repository.

* [programming-principles](programming-principles.md)

## Installation

**Caution:** The pinned README's command installs the full catalog globally for Codex, uses a moving source, and may replace installed skills. The separately fetched `skills` CLI and other packages are unassessed. Check the target and installer before use.

The [upstream README](https://github.com/magnus919/agent-skills/blob/9b34a87ee729f109019ac604681e5796349ea1b2/README.md#installation) requires Node.js/npm and Git. Run on the target machine:

```bash
npx skills add magnus919/agent-skills --skill '*' --agent codex --global --yes
```

The command selects all skills, not just this item; the pinned README documents project scope by omitting `--global`. No supported single-item pin was verified.

Installation commands were not run.
