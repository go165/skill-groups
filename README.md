# skill-groups

Skill groups, GitHub skills group, agent skill groups, and Agent Skills profile
manager search entry for `agent-skill-groups`.

This repository is a transparent navigation entry point for the maintained
project:

<https://github.com/go165/agent-skill-groups>

Documentation:

<https://go165.github.io/agent-skill-groups/>

Search landing page:

<https://go165.github.io/skill-groups/>

## What This Points To

`agent-skill-groups` is a cross-runtime Agent Skills manager. It organizes local
`SKILL.md` directories into scenario groups for Codex, Claude Code, OpenCode,
and generic agent runtimes.

If you searched GitHub for `skill groups`, `skill-groups`, `agent skill groups`,
`github skills group`, or `github skill-group`, this repository points to the
maintained manager rather than an unrelated class project, study group, or game
mod.

Use the canonical project when an agent workstation has too many always-on
skills and needs a repeatable way to:

- inspect installed `SKILL.md` directories
- suggest scenario groups
- switch profiles by runtime
- back up and restore skill directory state
- write managed `AGENTS.md` or `CLAUDE.md` instruction blocks

## Install

```bash
pipx install git+https://github.com/go165/agent-skill-groups.git
agent-skill-groups demo --json
```

## Core Commands

```bash
agent-skill-groups runtimes
agent-skill-groups init --runtime codex --output groups.json
agent-skill-groups status --config groups.json --runtime codex --json --details
agent-skill-groups plan --config groups.json --runtime codex research
agent-skill-groups backup --config groups.json --runtime codex
agent-skill-groups profile --config groups.json --runtime codex research
agent-skill-groups restore --config groups.json --runtime codex backup.json
```

## Why This Repository Exists

Some users search for "skill groups" or "agent skill groups" before they know
the canonical package name. This repository exists only to route those searches
to the maintained project above.

Do not file feature requests here. Use the canonical repository:

<https://github.com/go165/agent-skill-groups/issues>
