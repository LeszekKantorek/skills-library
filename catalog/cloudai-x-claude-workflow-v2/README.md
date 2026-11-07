# CloudAI-X Claude workflow

[CloudAI-X/claude-workflow-v2](https://github.com/CloudAI-X/claude-workflow-v2) contains a Claude Code workflow plugin with skills, agents, commands, and hooks. The following report assesses only the named skill at its recorded revision, not the full plugin:

* [designing-architecture](designing-architecture.md)
* [designing-tests](designing-tests.md)

## Installation

**Caution:** The following upstream command selects the repository without a commit pin and can install more than the assessed skill. The separately fetched `skills` installer, its version, selection behavior, and resulting destinations are outside this assessment. Review the installer and its prompts and target paths before use.

The pinned [upstream README](https://github.com/CloudAI-X/claude-workflow-v2/blob/3b5a89ec1c106dd387e372aec073f9401336382a/README.md#quick-start) documents this shell command, which requires Node.js and `npx` on the target machine:

```bash
npx skills add CloudAI-X/claude-workflow-v2
```

The README says this route installs skills, while its separate full-plugin routes include agents, commands, and hooks. The README does not establish an exact user or project destination for this command; actual scope depends on the independently versioned installer and selections. No pinned, single-item installation command was verified. The command was not executed.

## License

The pinned [repository license](https://github.com/CloudAI-X/claude-workflow-v2/blob/3b5a89ec1c106dd387e372aec073f9401336382a/LICENSE) is MIT, copyright 2025–2026 CloudAI-X. It permits use, modification, and redistribution subject to retaining its notice and permission text, and disclaims warranties.
