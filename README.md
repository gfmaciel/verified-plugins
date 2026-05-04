# verified-plugins

A public Claude Code + Codex plugin marketplace for teams that want to automate dev work but don't know where to start.

## Install

```bash
claude plugins add-marketplace github:gfmaciel/verified-plugins
```

## Plugins

| Plugin | Description | Usage |
|--------|-------------|-------|
| [one-page-creator](plugins/one-page-creator/) | Generate a one-pager to sell your manager on Claude Code automation | `/one-page-creator` |

## Adding a plugin

1. Create `plugins/<your-plugin-name>/` with this structure:

```
plugins/your-plugin-name/
├── .claude-plugin/
│   └── plugin.json          ← required metadata
├── skills/
│   └── your-plugin-name/
│       ├── SKILL.md         ← skill instructions + frontmatter
│       └── references/      ← optional reference docs
├── AGENTS.md                ← source of truth (plain markdown)
└── CLAUDE.md                ← single line: @AGENTS.md
```

2. `plugin.json` template:

```json
{
  "name": "your-plugin-name",
  "version": "1.0.0",
  "description": "One sentence description",
  "author": { "name": "Your Name" }
}
```

3. `SKILL.md` frontmatter:

```yaml
---
name: your-plugin-name
description: Use when [trigger condition]. One sentence, specific.
---
```

4. Add your plugin to `.claude-plugin/marketplace.json` in the `plugins` array.

5. Open a PR.

### Checklist

- [ ] `plugin.json` has name, version, description, author
- [ ] `SKILL.md` has frontmatter with `name` and `description`
- [ ] `AGENTS.md` is plain markdown (no `@` imports or Claude Code-specific syntax)
- [ ] `CLAUDE.md` contains only `@AGENTS.md`
- [ ] Plugin listed in root `marketplace.json`
- [ ] Plugin tested locally with `claude plugins install <name>@verified-plugins`
