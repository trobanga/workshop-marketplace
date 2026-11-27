# workshop-marketplace

Seed marketplace for the agentic coding workshop. One plugin: `workshop-skills`.

## Install

In Claude Code:

```
/plugin install workshop-skills --marketplace <owner>/<repo>
```

This needs Claude Code 2.1.275 or later. The two-step form:

```
/plugin marketplace add <owner>/<repo>
/plugin install workshop-skills@workshop-marketplace
```

`<owner>/<repo>` is open until the marketplace has a home (see `outline2.md`, Q20).
For a local test, give the path of this directory in place of `<owner>/<repo>`.

## Add your own plugin

1. Create `plugins/<name>/.claude-plugin/plugin.json`.
2. Add skills in `plugins/<name>/skills/<skill>/SKILL.md`.
3. Add one entry to `.claude-plugin/marketplace.json`.
4. Run `claude plugin validate .` and open a PR.
