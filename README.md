# pragmatic

a collection of agent skills that encourage pragmatic programming to improve LLM code review and code generation.

## skills


|                                                                        |                                                                                                   |
| ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| [do-not-reinvent-the-wheel](skills/do-not-reinvent-the-wheel/SKILL.md) | prefer well-maintained libraries over hand-rolled implementations when writing or reviewing code. |


## install

with [agent skills](https://agentskills.io) compatible agents (Cursor, Claude Code, Codex, etc.):

```bash
npx skills add gabrielemidulla/pragmatic
```

## website / cloudflare pages

Build output lives in `website/dist/` after `npm run build` inside [`website/`](website/).

In the Cloudflare dashboard, **do not** use `wrangler deploy` (Workers). Use **`wrangler pages deploy`** so `wrangler.jsonc` and `pages_build_output_dir` apply.

Example **build command**:

```bash
cd website && npm ci && npm run build
```

If you use a **separate deploy command** (or a single combined step), use:

```bash
cd website && npx wrangler pages deploy
```

Or one line (install + build + upload):

```bash
cd website && npm ci && npm run build && npx wrangler pages deploy
```

Alternatively, skip Wrangler on deploy: set **build output directory** to `website/dist` and use only the build command above—Pages will publish that folder without a custom deploy command.

## license

MIT. see [LICENSE](LICENSE).