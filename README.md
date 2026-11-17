# Chargezen agent skills

Skills that teach AI agents (ChatGPT, Claude, Codex, Cursor and personal agents) to work with
[Chargezen](https://chargezen.com), the revenue platform brands run on: Concierge digital employees,
CheckoutOS, SmartyTap texts and emails, loyalty, Spark! creators and affiliates, and subscriptions.

## Install

```sh
npx skills add chargezen/skills
```

Or point your agent at a hosted copy, starting with:

> Set up Chargezen for me. Fetch https://chargezen.com/.well-known/agent-skills/get-started/SKILL.md
> and follow it.

## Skills

| Skill | What it does |
| --- | --- |
| [`chargezen-get-started`](skills/chargezen-get-started/SKILL.md) | Connects an existing Chargezen account, or signs a new person up (they confirm their email, phone and card themselves), then does one useful first thing. |
| [`chargezen`](skills/chargezen/SKILL.md) | The shared rules: how to reach Chargezen's tools, the safe order for changes (read, draft, preview, go live on the person's OK) and what never to do. Every other skill follows it. |
| [`chargezen-weekly-brief`](skills/chargezen-weekly-brief/SKILL.md) | Read-only: shipping, best sellers and stock, subscriptions, customers waiting, campaigns and creator commissions, then the three things that need the merchant. |
| [`chargezen-inbox-triage`](skills/chargezen-inbox-triage/SKILL.md) | Works through customers waiting on a reply, checks their real order and subscription, drafts each reply for approval, and sends, assigns, tags or closes. |
| [`chargezen-campaign`](skills/chargezen-campaign/SKILL.md) | Builds an email, text or WhatsApp campaign as a draft from a brief, counts recipients and text cost, sends a test, and launches on the merchant's OK. |
| [`chargezen-win-back`](skills/chargezen-win-back/SKILL.md) | Sizes what cancellations cost, then builds a flow that invites canceled subscribers back with the merchant's offer. |
| [`chargezen-payment-recovery`](skills/chargezen-payment-recovery/SKILL.md) | Builds a flow for failed renewal payments: a kind email and text with a secure card-update link, and a team alert when retries run out. |
| [`chargezen-subscribe-and-save`](skills/chargezen-subscribe-and-save/SKILL.md) | Sets up delivery options and a subscriber discount for a product, shows what shoppers will see, and creates it on the merchant's OK. |
| [`chargezen-loyalty-review`](skills/chargezen-loyalty-review/SKILL.md) | Reviews points, rewards, tiers, referrals and rewards emails against real activity, and makes up to three approved changes. |
| [`chargezen-creator-review`](skills/chargezen-creator-review/SKILL.md) | Read-only Spark! review: top creators, what's owed, whether the balance covers it, refunds and pending applications. |

## For Claude Code

The same skills with slash commands (`/weekly-brief`, `/win-back`, …) ship as a plugin:

```
/plugin marketplace add chargezen/claude-plugins
/plugin install chargezen@chargezen
```

## For agents

- How to get access, sign someone up and what you must never do: https://chargezen.com/auth.md
- MCP server: `https://mcp.chargezen.com/mcp` (OAuth sign-in; product servers at `/mcp/<product>`),
  described at https://chargezen.com/.well-known/mcp.json
- Skill index: https://chargezen.com/.well-known/agent-skills/index.json
- Personal Agent Protocol 1.0: https://chargezen.com/.well-known/poppy.json

The hosted copies on chargezen.com are the source of truth; this repository mirrors them.

## License

MIT. See [LICENSE](LICENSE).
