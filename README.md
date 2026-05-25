# LangWatch (langwatch)

LangWatch is an open-source LLM observability, evaluation, and AI agent testing platform. OpenTelemetry-native tracing across LangChain, LangGraph, DSPy, OpenAI Agents, LiteLLM, Pydantic AI, CrewAI, AWS Bedrock, and more — paired with real-time and batch evaluators, prompt versioning, multi-turn agent simulations (open-source `scenario` framework with User Simulator and Judge Agents), datasets, an OpenAI/Anthropic-compatible AI Gateway with virtual keys and budgets, and a published REST API. Apache-2.0 core (with `ee/` enterprise modules under commercial license); MIT-licensed SDKs; deployable as LangWatch Cloud or self-hosted via Docker Compose, Helm, Kind, or full Kubernetes.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/langwatch/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - AI, Artificial Intelligence, LLM, LLM Observability, LLM Evaluation, Agent Testing, Agent Simulation, Prompt Management, Datasets, Tracing, OpenTelemetry, AI Gateway, DSPy, LangChain, Open Source, MCP, FinOps

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Plans

| Plan | Currency | Price | Included Events / Month | Retention | Notes |
|---|---|---|---|---|---|
| Developer | EUR / USD | Free | 50,000 | 14 days | 2 users, 3 scenarios, community support |
| Growth | EUR | 59 / core seat / month | 200,000 (+ EUR 0.0005 / event) | 30 days (+ EUR 3 / GB) | Unlimited lite-users, private support |
| Enterprise / Regulated | USD | Custom | Contract | Custom | On-prem, hybrid, SSO, SOC 2 / ISO 27001 |
| Self-Hosted OSS | USD | Free (Apache-2.0) | Unlimited | Unlimited | Docker Compose / Helm / Kind |

See [plans/langwatch-plans-pricing.yml](plans/langwatch-plans-pricing.yml), [rate-limits/langwatch-rate-limits.yml](rate-limits/langwatch-rate-limits.yml), and [finops/langwatch-finops.yml](finops/langwatch-finops.yml).

## Canonical OpenAPI

The full LangWatch REST surface lives in a single OpenAPI 3.1 document maintained inside the [langwatch/langwatch](https://github.com/langwatch/langwatch) monorepo. A mirrored copy is stored here at [openapi/langwatch-openapi.json](openapi/langwatch-openapi.json) and is referenced by every API entry below.

## APIs

### LangWatch Traces API
Search, retrieve, and share LLM application traces ingested via OpenTelemetry.

**Human URL:** [https://langwatch.ai/docs/api-reference/traces](https://langwatch.ai/docs/api-reference/traces)

- [Documentation](https://langwatch.ai/docs/api-reference/traces)
- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Traces](capabilities/traces.yaml)

### LangWatch Evaluators API
Configure and manage scorer evaluators — RAGAS, safety, PII, semantic similarity, LLM-as-Judge variants.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Evaluators](capabilities/evaluators.yaml)

### LangWatch Monitors API
Online monitors that automatically score incoming production traces.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Monitors](capabilities/monitors.yaml)

### LangWatch Datasets API
Manage evaluation, regression, and fine-tuning datasets and their records.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Datasets](capabilities/datasets.yaml)

### LangWatch Prompts API
Version, tag, sync, and restore prompts across projects with feature-flag-style deployment.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Prompts](capabilities/prompts.yaml)

### LangWatch Scenarios API
Define multi-turn agent test scenarios used by the open-source `scenario` framework.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Scenarios](capabilities/scenarios.yaml)

### LangWatch Simulation Runs API
Query and retrieve completed agent simulation runs and batches.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Simulation Runs](capabilities/simulation-runs.yaml)

### LangWatch Suites API
Compose and execute batch test suites combining scenarios, datasets, and evaluators.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Suites](capabilities/suites.yaml)

### LangWatch Experiments API
Trigger and inspect batch experiment runs (including DSPy-driven optimization runs).

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Experiments](capabilities/experiments.yaml)

### LangWatch Annotations API
Collaborative annotation and labeling workflows over traces.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Annotations](capabilities/annotations.yaml)

### LangWatch Analytics API
Time-series analytics over traces, tokens, cost, latency, and evaluator scores.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Analytics](capabilities/analytics.yaml)

### LangWatch Dashboards API
Create, reorder, and manage dashboards and their composed graphs.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Dashboards](capabilities/dashboards.yaml)

### LangWatch Projects API
Provision and manage projects (workspaces) — the top-level isolation boundary.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Projects](capabilities/projects.yaml)

### LangWatch API Keys API
Create, list, and revoke project API keys used by SDKs and automation.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — API Keys](capabilities/api-keys.yaml)

### LangWatch Secrets API
Encrypted credential storage for evaluator and integration secrets.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Secrets](capabilities/secrets.yaml)

### LangWatch Model Providers API
Configure model-provider credentials and per-project model defaults.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Model Providers](capabilities/model-providers.yaml)

### LangWatch AI Gateway API
OpenAI/Anthropic-compatible governance proxy — virtual keys, provider bindings, budgets, semantic cache rules.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — AI Gateway](capabilities/ai-gateway.yaml)

### LangWatch Workflows API
Compose, version, and run optimization-studio workflows.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Workflows](capabilities/workflows.yaml)

### LangWatch Agents API
Define and update agent records used by simulations and scenarios.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Agents](capabilities/agents.yaml)

### LangWatch Triggers API
Event-driven triggers that fire on trace conditions and monitor scores.

- [OpenAPI](openapi/langwatch-openapi.json)
- [Naftiko Capability — Triggers](capabilities/triggers.yaml)

## SDKs, MCP, and Companion Repos

- **Python SDK** — [`pip install langwatch`](https://pypi.org/project/langwatch/) (instruments OpenAI, Azure, LiteLLM, DSPy, LangChain, plus any OTel client)
- **TypeScript SDK** — [`npm i langwatch`](https://www.npmjs.com/package/langwatch)
- **MCP Server** — [`@langwatch/mcp-server`](https://www.npmjs.com/package/@langwatch/mcp-server) exposes Observability, Prompts, Datasets, Scenarios, and Evaluator tools to Claude / Cursor / other MCP clients
- **scenario** — [github.com/langwatch/scenario](https://github.com/langwatch/scenario) — open-source multi-turn agent testing with User Simulator and Judge Agents
- **better-agents** — [github.com/langwatch/better-agents](https://github.com/langwatch/better-agents) — standards for building agents
- **langevals** — [github.com/langwatch/langevals](https://github.com/langwatch/langevals) — evaluator aggregation
- **cookbooks** — [github.com/langwatch/cookbooks](https://github.com/langwatch/cookbooks) — Jupyter example notebooks

## Self-Hosting

- Docker Compose, Helm chart, Kind, or full Kubernetes
- Data layer: PostgreSQL + Redis + ClickHouse + OpenSearch
- Apache-2.0 core; `ee/` modules require commercial license

## Common Properties

See [apis.yml](apis.yml) for the full `common` block — Portal, Documentation, API Reference, Self-Hosting docs, Pricing, OpenAPI, Application (Cloud Dashboard), SignUp, ChangeLog, Discord, LinkedIn, Twitter, YouTube, and the consolidated Features list.

## Maintainer

- Kin Lane — kin@apievangelist.com — [@apievangelist](https://twitter.com/apievangelist)
