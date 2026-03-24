# pragmatic

Agent skills that encourage pragmatic programming: lean on proven tools, avoid unnecessary custom code, and keep LLM-assisted development grounded in maintainable habits.

## Skills

| Skill | Summary |
|-------|---------|
| [do-not-reinvent-the-wheel](skills/do-not-reinvent-the-wheel/SKILL.md) | Prefer well-maintained libraries over hand-rolled implementations when writing or reviewing code. |

## Install

With [Agent Skills](https://agentskills.io)–compatible agents (Cursor, Claude Code, Codex, etc.):

```bash
npx skills add gabrielemidulla/pragmatic@do-not-reinvent-the-wheel
```

Add more skills from this repo by changing the name after `@` as new skills are published under `skills/<name>/`.

## Listing on skills.sh

This repository follows the standard layout: one folder per skill under `skills/`, each containing a `SKILL.md` with YAML frontmatter (`name`, `description`, and optional `license` / `metadata`). After you push to GitHub, import the repo on [skills.sh](https://skills.sh) (or connect a webhook) so the directory can index and surface your skills.

## License

MIT. See [LICENSE](LICENSE).
