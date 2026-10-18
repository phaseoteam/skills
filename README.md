# Phaseo Skills

Agent skills and the Phaseo plugin for building on [Phaseo](https://phaseo.app), the AI gateway that gives you one API for many model providers.

[![skills.sh](https://skills.sh/b/phaseoteam/skills)](https://skills.sh/phaseoteam/skills)

## Install the plugin

The Phaseo plugin bundles every skill below, the Phaseo MCP (live models, pricing and usage for your account) and the Phaseo Docs MCP.

Claude Code:

```bash
claude plugin marketplace add phaseoteam/skills
claude plugin install phaseo@phaseo
```

Or, inside Claude Code: `/plugin install phaseo --marketplace phaseoteam/skills`. Then run `/mcp` and sign in to `plugin:phaseo:phaseo`.

Codex:

```bash
codex plugin marketplace add phaseoteam/skills
codex plugin add phaseo@phaseo
codex mcp login phaseo
```

## Install only the skills

For any agent that supports skills:

```bash
npx skills add phaseoteam/skills
```

Or from the Phaseo docs, which serve the same skills:

```bash
npx skills add https://phaseo.app/docs
```

List the skills without installing, or install every skill for one agent:

```bash
npx skills add phaseoteam/skills --list
npx skills add phaseoteam/skills --agent codex --skill '*'
```

## Skills

| Skill | Use it to |
| --- | --- |
| `phaseo-gateway` | Integrate with the Phaseo Gateway over REST, the TypeScript or Python SDK, or the Vercel AI SDK. |
| `phaseo-migration` | Move from OpenAI, Anthropic, OpenRouter, Vercel AI Gateway, LiteLLM, Cloudflare AI Gateway, Helicone or LLM Gateway. |
| `openrouter-to-phaseo-migration` | Move an OpenRouter integration in depth. |
| `phaseo-model-selection` | Choose and pin model IDs by capability, context, price and lifecycle. |
| `phaseo-usage-monitoring` | Track credits and spend, and debug a request's cost or failure. |
| `phaseo-sdk-typescript` | Use the TypeScript and JavaScript SDK, `@phaseo/sdk`. |
| `phaseo-sdk-python` | Use the Python SDK, `phaseo`. |
| `phaseo-agent-sdk-typescript` | Build agent loops with the TypeScript Agent SDK, `@phaseo/agent-sdk`. |
| `phaseo-routing-presets` | Roll out and debug presets, routing policy and response caching. |
| `phaseo-guardrails` | Configure and debug guardrails for API keys. |
| `phaseo-async-webhooks` | Build async video, batch and webhook integrations. |
| `phaseo-web-search-tools` | Configure web search and web fetch grounding. |
| `phaseo-response-healing` | Recover structured JSON output with response healing. |
| `phaseo-cli` | Operate Phaseo through the `phaseo` CLI. |

The plugin also includes `phaseo`, a skill for the Phaseo MCP tools.

## Where these come from

The skills are maintained in the [Phaseo repository](https://github.com/phaseoteam/Phaseo/tree/main/.agents/skills) and published with the [Phaseo docs](https://phaseo.app/docs); the plugin lives in [`apps/mcp/plugin/phaseo`](https://github.com/phaseoteam/Phaseo/tree/main/apps/mcp/plugin/phaseo). The [sync workflow](.github/workflows/sync.yml) copies both here every day, so do not edit `skills/` or `plugins/` in this repository; changes belong in the Phaseo repository. The marketplace files in `.claude-plugin/` and `.agents/plugins/` are maintained here.

Documentation: https://phaseo.app/docs

## License

MIT. See [LICENSE](LICENSE).
