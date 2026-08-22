# LangWatch (langwatch)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

LangWatch is an open-source LLM observability, evaluation, and AI agent testing platform. Built around OpenTelemetry-native tracing, LangWatch lets teams instrument LLM applications (LangChain, LangGraph, DSPy, OpenAI Agents, LiteLLM, Pydantic AI, CrewAI, AWS Bedrock, and more), run real-time and batch evaluations, version and deploy prompts, simulate multi-turn agent conversations against scripted scenarios and Judge Agents, manage labeled datasets, and govern model traffic through a virtual-key AI Gateway with budgets and semantic caching. The platform exposes a REST API at app.langwatch.ai, ships Python and TypeScript SDKs plus an MCP server, publishes the companion `scenario` agent-testing framework and `better-agents` standards, and runs on Apache-2.0 core (with `ee/` enterprise modules under commercial license) — deployable as LangWatch Cloud or self-hosted via Docker Compose, Helm, Kind, or full Kubernetes.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/langwatch/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/langwatch/refs/heads/main/apis.yml)

## Scope

- **Type:** contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- AI
- Artificial Intelligence
- LLM
- LLM Observability
- LLM Evaluation
- Agent Testing
- Agent Simulation
- Prompt Management
- Datasets
- Tracing
- OpenTelemetry
- AI Gateway
- DSPy
- LangChain
- Open Source
- MCP
- FinOps

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### LangWatch Traces API

Search, retrieve, share, and unshare traces produced by instrumented LLM applications. Traces are the foundational observability primitive in LangWatch and arrive via OTLP/OpenTelemetry from Python or TypeScript SDKs (or any OTel-compliant client). Endpoints include /api/traces/search, /api/traces/{traceId}, /api/trace/{id}/share, and /api/trace/{id}/unshare.

- **Human URL:** [https://langwatch.ai/docs/api-reference/traces](https://langwatch.ai/docs/api-reference/traces)

#### Tags

- Traces
- Observability
- OpenTelemetry

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/traces)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Evaluators API

Configure and manage scorer evaluators — RAG quality (RAGAS), safety (Azure Content Safety, OpenAI Moderation, PII), format validation, semantic similarity, language detection, and LLM-as-Judge variants — that grade traces and dataset records.

- **Human URL:** [https://langwatch.ai/docs/api-reference/evaluators](https://langwatch.ai/docs/api-reference/evaluators)

#### Tags

- Evaluations
- Evaluators
- RAGAS
- Safety

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/evaluators)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Monitors API

Create, toggle, and manage online monitors that automatically run configured evaluators against incoming production traces in real time.

- **Human URL:** [https://langwatch.ai/docs/api-reference/monitors](https://langwatch.ai/docs/api-reference/monitors)

#### Tags

- Monitors
- Online Evaluations
- Production

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/monitors)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Datasets API

Manage evaluation, regression, and fine-tuning datasets and their records. Supports CSV upload, programmatic record CRUD, and conversion of production traces into reusable test cases.

- **Human URL:** [https://langwatch.ai/docs/api-reference/datasets](https://langwatch.ai/docs/api-reference/datasets)

#### Tags

- Datasets
- Records
- Fine-Tuning

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/datasets)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Prompts API

Version, tag, sync, and restore prompts across projects. Backs the LangWatch Studio prompt editor and supports feature-flag-style deployment of prompt versions in production code.

- **Human URL:** [https://langwatch.ai/docs/api-reference/prompts](https://langwatch.ai/docs/api-reference/prompts)

#### Tags

- Prompts
- Versioning
- Deployment

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/prompts)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Scenarios API

Define multi-turn agent test scenarios used by the open-source `scenario` framework. Scenarios pair an Agent Under Test, a User Simulator Agent, and a Judge Agent (with optional script DSL) and run via pytest-compatible runners locally or in CI.

- **Human URL:** [https://github.com/langwatch/scenario](https://github.com/langwatch/scenario)

#### Tags

- Scenarios
- Agent Testing
- Simulations

#### Properties

- [Documentation](https://github.com/langwatch/scenario)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Simulation Runs API

Query and retrieve completed agent simulation runs and batches, including Judge Agent verdicts, transcripts, and per-turn evaluator scores.

- **Human URL:** [https://langwatch.ai/docs/api-reference/simulation-runs](https://langwatch.ai/docs/api-reference/simulation-runs)

#### Tags

- Simulations
- Agent Testing
- Batches

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/simulation-runs)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Suites API

Manage and execute batch test suites that compose scenarios, datasets, and evaluators into reproducible experiments and regression runs.

- **Human URL:** [https://langwatch.ai/docs/api-reference/suites](https://langwatch.ai/docs/api-reference/suites)

#### Tags

- Suites
- Experiments
- Batches

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/suites)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Experiments API

Trigger and inspect batch experiment runs (including DSPy-driven prompt and pipeline optimization runs) by slug, with full per-run telemetry.

- **Human URL:** [https://langwatch.ai/docs/api-reference/experiments](https://langwatch.ai/docs/api-reference/experiments)

#### Tags

- Experiments
- Batches
- DSPy

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/experiments)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Annotations API

Collaborative annotation and labeling workflows over traces — used by domain experts and PMs to produce graded examples for evaluations and fine-tuning datasets.

- **Human URL:** [https://langwatch.ai/docs/api-reference/annotations](https://langwatch.ai/docs/api-reference/annotations)

#### Tags

- Annotations
- Labeling
- Human Feedback

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/annotations)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Analytics API

Time-series analytics over traces, tokens, costs, latency, and evaluator scores — the data source behind LangWatch dashboards and graphs.

- **Human URL:** [https://langwatch.ai/docs/api-reference/analytics](https://langwatch.ai/docs/api-reference/analytics)

#### Tags

- Analytics
- Time Series
- Dashboards

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/analytics)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Dashboards API

Create, reorder, update, and embed dashboards composed of analytics graphs and saved trace searches.

- **Human URL:** [https://langwatch.ai/docs/api-reference/dashboards](https://langwatch.ai/docs/api-reference/dashboards)

#### Tags

- Dashboards
- Graphs
- Visualization

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/dashboards)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Projects API

Programmatically provision and manage projects and team workspaces — the top-level isolation boundary for traces, prompts, datasets, and gateway routing.

- **Human URL:** [https://langwatch.ai/docs/api-reference/projects](https://langwatch.ai/docs/api-reference/projects)

#### Tags

- Projects
- Teams
- Provisioning

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/projects)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch API Keys API

Create, list, and revoke project API keys for SDK and automation use. Authenticates as `project_api_key` against the LangWatch REST API.

- **Human URL:** [https://langwatch.ai/docs/api-reference/api-keys](https://langwatch.ai/docs/api-reference/api-keys)

#### Tags

- API Keys
- Authentication
- Service Accounts

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/api-keys)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Secrets API

Encrypted credential storage for evaluator and integration secrets (model-provider keys, third-party API keys) used by hosted runs.

- **Human URL:** [https://langwatch.ai/docs/api-reference/secrets](https://langwatch.ai/docs/api-reference/secrets)

#### Tags

- Secrets
- Credentials
- Vault

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/secrets)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Model Providers API

Configure model-provider credentials and per-project model defaults used by evaluators, judges, and the AI Gateway.

- **Human URL:** [https://langwatch.ai/docs/api-reference/model-providers](https://langwatch.ai/docs/api-reference/model-providers)

#### Tags

- Model Providers
- Model Defaults
- Routing

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/model-providers)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch AI Gateway API

OpenAI/Anthropic-compatible governance proxy. Manages provider bindings, virtual keys (with rotate and revoke), per-team budgets, and semantic cache rules under /api/gateway/v1/* — written in Go.

- **Human URL:** [https://langwatch.ai/docs/api-reference/gateway](https://langwatch.ai/docs/api-reference/gateway)

#### Tags

- AI Gateway
- Virtual Keys
- Budgets
- Caching
- Governance

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/gateway)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Workflows API

Compose, version, and run optimization-studio workflows that chain prompts, datasets, evaluators, and DSPy optimizers.

- **Human URL:** [https://langwatch.ai/docs/api-reference/workflows](https://langwatch.ai/docs/api-reference/workflows)

#### Tags

- Workflows
- Optimization Studio
- DSPy

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/workflows)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Agents API

Define and update agent records used by Agent Simulations and Scenarios — wiring system prompts, tools, and evaluator suites into reproducible agent definitions.

- **Human URL:** [https://langwatch.ai/docs/api-reference/agents](https://langwatch.ai/docs/api-reference/agents)

#### Tags

- Agents
- Better Agents
- Configuration

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/agents)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### LangWatch Triggers API

Create and manage event-driven triggers that fire actions (alerts, webhooks, eval runs) when trace conditions or monitor scores match.

- **Human URL:** [https://langwatch.ai/docs/api-reference/triggers](https://langwatch.ai/docs/api-reference/triggers)

#### Tags

- Triggers
- Alerts
- Automation

#### Properties

- [Documentation](https://langwatch.ai/docs/api-reference/triggers)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langwatch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langwatch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://langwatch.ai)
- [Documentation](https://langwatch.ai/docs/)
- [Getting Started](https://langwatch.ai/docs/integration/quickstart)
- [Documentation](https://langwatch.ai/docs/api-reference)
- [OpenAPI](openapi/langwatch-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Application](https://app.langwatch.ai)
- [Sign Up](https://app.langwatch.ai/auth/signup)
- [Pricing](https://langwatch.ai/pricing)
- [Plans](plans/langwatch-plans-pricing.yml)
- [Rate Limits](rate-limits/langwatch-rate-limits.yml)
- [Fin Ops](finops/langwatch-finops.yml)
- [Documentation](https://langwatch.ai/docs/self-hosting/overview)
- [Documentation](https://langwatch.ai/docs/observability)
- [Documentation](https://langwatch.ai/docs/evaluations)
- [Documentation](https://langwatch.ai/docs/prompt-management)
- [Documentation](https://langwatch.ai/docs/simulations)
- [Documentation](https://langwatch.ai/docs/llms.txt)
- [GitHub Organization](https://github.com/langwatch)
- [Source Code](https://github.com/langwatch/langwatch)
- [Source Code](https://github.com/langwatch/scenario)
- [Source Code](https://github.com/langwatch/better-agents)
- [Source Code](https://github.com/langwatch/langevals)
- [Source Code](https://github.com/langwatch/cookbooks)
- [Source Code](https://github.com/langwatch/skills)
- [SDK](https://pypi.org/project/langwatch/)
- [SDK](https://www.npmjs.com/package/langwatch)
- [M C P](https://www.npmjs.com/package/@langwatch/mcp-server)
- [License](https://github.com/langwatch/langwatch/blob/main/LICENSE)
- [Terms of Service](https://langwatch.ai/terms)
- [Privacy Policy](https://langwatch.ai/privacy)
- [Blog](https://langwatch.ai/blog)
- [Changelog](https://langwatch.ai/docs/changelog)
- [Forum](https://discord.gg/langwatch)
- [LinkedIn](https://www.linkedin.com/company/langwatch)
- [Twitter](https://twitter.com/langwatchai)
- [YouTube](https://www.youtube.com/@langwatch)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
