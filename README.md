# AI Stats Skills

Public installable skills for the AI Stats ecosystem.

[![skills.sh](https://skills.sh/b/AI-Stats/skills)](https://skills.sh/AI-Stats/skills)

This repository is intended to be published as its own standalone skills source for [`skills.sh`](https://skills.sh/) and compatible coding agents.

## Install

Canonical public source:

```text
AI-Stats/skills
```

List available skills:

```bash
npx skills add AI-Stats/skills --list
```

Install all public AI Stats skills for Codex:

```bash
npx skills add AI-Stats/skills --agent codex --skill '*'
```

Install one specific skill:

```bash
npx skills add AI-Stats/skills --agent codex --skill ai-stats-gateway
```

## Available skills

- `ai-stats-gateway`
- `ai-stats-guardrails`
- `ai-stats-response-healing`
- `ai-stats-web-search-tools`
- `ai-stats-async-webhooks`
- `ai-stats-routing-presets`
- `ai-stats-sdk-typescript`
- `ai-stats-sdk-python`
- `ai-stats-agent-sdk-typescript`
- `openrouter-to-ai-stats-migration`

## Repository shape

This repository intentionally contains only public AI Stats skills under `skills/<skill-name>/SKILL.md`.

Internal or workflow-specific helper skills remain in the main product repository and are not part of this public distribution surface.

## Local validation

From the repository root:

```bash
npx skills add . --list --agent codex
```
