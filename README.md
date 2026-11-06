# ctojmt skills

Skills for coding agents, by [@ctojmt](https://x.com/ctojmt).

## Install

Install with the [skills CLI](https://github.com/vercel-labs/skills), which works with Claude Code, Cursor, Codex and other agents:

```
npx skills add jmt-es/skills
```

To install a single skill:

```
npx skills add jmt-es/skills --skill rewire
```

Or, in Claude Code, add this repo as a plugin marketplace:

```
/plugin marketplace add jmt-es/skills
```

Then install a skill with the command in its row of the table below.

To install by hand instead, copy a skill's folder into `~/.claude/skills/`.

## Skills

| Skill | Description | Install |
| --- | --- | --- |
| [rewire](skills/rewire/SKILL.md) | Untangle a whole codebase in one pass, so agents read less per change, break less without noticing, and debug faster. | `/plugin install rewire@ctojmt-skills` |

Run it in your agent as `/rewire`, or point it at one area: `/rewire src/billing`.

`rewire` is adapted from [untangle-codebase](https://github.com/caldoai/skills/tree/main/skills/untangle-codebase) by Maze ([@mazeincoding](https://x.com/mazeincoding)), under the MIT license.

## Adding a skill

1. Create `skills/<name>/SKILL.md`.
2. Add an entry for it to `plugins` in [.claude-plugin/marketplace.json](.claude-plugin/marketplace.json).
3. Add a row to the table above.

## License

[MIT](LICENSE)
