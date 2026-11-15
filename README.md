# Chargezen agent skills

Skills that teach AI agents (ChatGPT, Claude, Codex, Cursor and personal agents) to work with
[Chargezen](https://chargezen.com), the revenue platform brands run on: Concierge digital employees,
CheckoutOS, SmartyTap texts and emails, loyalty, Spark! creators and affiliates, and subscriptions.

## Install

```sh
npx skills add chargezen/skills
```

Or point your agent at the hosted copy:

> Set up Chargezen for me. Fetch https://chargezen.com/.well-known/agent-skills/get-started/SKILL.md
> and follow it.

## Skills

| Skill | What it does |
| --- | --- |
| [`chargezen-get-started`](skills/chargezen-get-started/SKILL.md) | Connects an existing Chargezen account, or signs a new person up (they confirm their email, phone and card themselves), then does one useful first thing. |

## For agents

- How to get access, sign someone up and what you must never do: https://chargezen.com/auth.md
- MCP server: `https://mcp.chargezen.com/mcp` (OAuth sign-in; product servers at `/mcp/<product>`),
  described at https://chargezen.com/.well-known/mcp.json
- Skill index: https://chargezen.com/.well-known/agent-skills/index.json
- Personal Agent Protocol 1.0: https://chargezen.com/.well-known/poppy.json

The hosted copies on chargezen.com are the source of truth; this repository mirrors them.

## License

MIT. See [LICENSE](LICENSE).
