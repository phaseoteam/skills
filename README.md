# Phaseo Skills

Agent skills for building on [Phaseo](https://phaseo.app), the AI gateway that gives you one API for many model providers.

[![skills.sh](https://skills.sh/b/phaseoteam/skills)](https://skills.sh/phaseoteam/skills)

## Install

From this repository:

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
| `phaseo-gateway` | Integrate or migrate to the Phaseo Gateway over REST, the TypeScript or Python SDK, or the Vercel AI SDK. |
| `phaseo-sdk-typescript` | Use the TypeScript and JavaScript SDK, `@phaseo/sdk`. |
| `phaseo-sdk-python` | Use the Python SDK, `phaseo`. |
| `phaseo-agent-sdk-typescript` | Build agent loops with the TypeScript Agent SDK, `@phaseo/agent-sdk`. |
| `openrouter-to-phaseo-migration` | Move an existing OpenRouter integration to Phaseo. |
| `phaseo-routing-presets` | Roll out and debug presets, routing policy and response caching. |
| `phaseo-guardrails` | Configure and debug guardrails for API keys. |
| `phaseo-async-webhooks` | Build async video, batch and webhook integrations. |
| `phaseo-web-search-tools` | Configure web search and web fetch grounding. |
| `phaseo-response-healing` | Recover structured JSON output with response healing. |
| `phaseo-cli` | Operate Phaseo through the `phaseo` CLI. |

## Where these come from

The skills are maintained in the [Phaseo repository](https://github.com/phaseoteam/Phaseo/tree/main/.agents/skills) and published with the [Phaseo docs](https://phaseo.app/docs). The [sync workflow](.github/workflows/sync.yml) copies them here every day, so do not edit `skills/` in this repository; changes belong in the Phaseo repository.

Documentation: https://phaseo.app/docs
