# Kallen for Claude

[Kallen](https://kallen.ai) is a research library of short-form video that already knows what is working: Instagram Reels, YouTube Shorts and LinkedIn posts, each scored against its own creator's usual views and broken down into its hook, format, structure and transcript.

This plugin connects Claude to Kallen's MCP server (`https://kallen.ai/mcp`) and adds slash commands for the most common research jobs. Claude writes the ideas; Kallen supplies the evidence from videos that actually outperformed.

## Install

In Claude Code:

```
/plugin marketplace add theisaacmed/kallen-plugins
/plugin install kallen@kallen
```

The first time a command runs, Claude asks you to sign in to Kallen. The connector is free with a Kallen account; sign up at [kallen.ai](https://kallen.ai).

You can also add Kallen as a connector in Claude without the plugin, using `https://kallen.ai/mcp`.

## Commands

| Command | What it does |
| --- | --- |
| `/kallen:hooks [topic]` | The hook patterns behind recent outliers, with fill-in-the-blank templates and examples |
| `/kallen:formats [topic]` | The formats and structures that are outperforming |
| `/kallen:topics` | The topics winning right now |
| `/kallen:recap <creator>` | What a creator focuses on, how often they post and their best recent videos |
| `/kallen:next-video [topic]` | Evidence for your next video, from what is working now |
| `/kallen:remix <Kallen video ID>` | A reusable blueprint of one video's structure, to adapt in your own words |
| `/kallen:client-ideas <client>` | Ideas for a client, drawn from other creators' winners on the client's angles |

Kallen reads and analyses; it never posts for you. Saved videos and notes stay private to your account.

## Links

- Docs: <https://kallen.ai/docs/mcp>
- Privacy: <https://kallen.ai/privacy> · Terms: <https://kallen.ai/terms>
- Support: support@kallen.ai

## Licence

MIT, for the plugin's prompt text and manifests. See [LICENSE](LICENSE). Kallen's service and data are covered by its [terms](https://kallen.ai/terms).
