# Encore (encore-dev)

Encore is a backend application framework and developer cloud that lets engineering teams build type-safe distributed systems in TypeScript (Encore.ts) and Go (Encore.go) using declarative Infrastructure from Code. Developers describe APIs, databases, Pub/Sub, object storage, caches, cron jobs, and secrets as typed code primitives; the framework provisions matching infrastructure locally with no Docker Compose, and Encore Cloud provisions equivalent managed resources in the customer's own AWS or GCP account. The platform ships built-in distributed tracing, a local development dashboard, auto-generated API docs and client SDKs, a Model Context Protocol server for AI agents, preview environments per pull request, and CI/CD — positioning Encore as an opinionated alternative to PaaS and a productivity layer on top of hyperscaler infrastructure.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/encore-dev/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Backend, Framework, Cloud, TypeScript, Go, DeveloperTools, InfrastructureFromCode, Microservices, Observability, Multicloud

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Encore Framework API
The in-process declarative API surface developers use inside Encore.ts and Encore.go applications. Endpoints are declared with `api()` (TypeScript) or `//encore:api` (Go), specifying method, path, expose (public vs internal), auth, and optional sensitive flags. Encore parses the source to derive request/response schemas from TypeScript interfaces or Go structs, enforces runtime validation, and wires up service-to-service calls without manual HTTP plumbing.

**Human URL:** [https://encore.dev/docs/ts/primitives/defining-apis](https://encore.dev/docs/ts/primitives/defining-apis)

- [Documentation — Encore.ts](https://encore.dev/docs/ts/primitives/defining-apis)
- [Documentation — Encore.go](https://encore.dev/docs/go/primitives/defining-apis)
- [OpenAPI](openapi/encore-framework-openapi.yml)
- [JSON Schema — Endpoint](json-schema/encore-api-endpoint-schema.json)
- [JSON Schema — Service](json-schema/encore-service-schema.json)
- [JSON-LD Context](json-ld/encore-dev-context.jsonld)
- [Naftiko Capability — Framework](capabilities/encore-framework.yaml)

### Encore Infrastructure API
Encore's Infrastructure from Code surface — declare PostgreSQL databases, Pub/Sub topics and subscriptions, object storage buckets, caches, cron jobs, and secrets as typed code primitives that Encore provisions locally (Docker-free) and on AWS or GCP via Encore Cloud, without Terraform or YAML.

**Human URL:** [https://encore.dev/docs/ts/primitives](https://encore.dev/docs/ts/primitives)

- [Documentation — Databases](https://encore.dev/docs/ts/primitives/databases)
- [Documentation — Pub/Sub](https://encore.dev/docs/ts/primitives/pubsub)
- [Documentation — Cron Jobs](https://encore.dev/docs/ts/primitives/cron-jobs)
- [Documentation — Object Storage](https://encore.dev/docs/ts/primitives/object-storage)
- [Documentation — Secrets](https://encore.dev/docs/ts/primitives/secrets)
- [JSON Schema — Infrastructure Resource](json-schema/encore-infrastructure-resource-schema.json)
- [Naftiko Capability — Infrastructure](capabilities/encore-infrastructure.yaml)

### Encore Cloud Platform API
The Encore Cloud control surface that takes an Encore application from `git push encore` to a running production deployment in the customer's own AWS or GCP account — automatic infrastructure provisioning, CI/CD, preview environments per pull request, trace and metric ingest, and the developer dashboard at app.encore.cloud.

**Human URL:** [https://encore.dev/docs/platform](https://encore.dev/docs/platform)

- [Documentation](https://encore.dev/docs/platform)
- [Portal — encore.cloud](https://encore.cloud)
- [OpenAPI](openapi/encore-platform-openapi.yml)
- [Naftiko Capability — Platform](capabilities/encore-platform.yaml)

### Encore Observability API
Encore captures distributed traces, structured logs, and runtime metrics automatically from every `api()`, database query, Pub/Sub publish, cron tick, and outbound HTTP call. The local Development Dashboard surfaces traces, the service catalog, an auto-generated architecture flow diagram, the database explorer, and the API explorer. In production, traces and metrics ship to Encore Cloud or forward to Datadog, Grafana, and Sentry.

**Human URL:** [https://encore.dev/docs/ts/observability/tracing](https://encore.dev/docs/ts/observability/tracing)

- [Documentation — Tracing](https://encore.dev/docs/ts/observability/tracing)
- [Documentation — Dev Dashboard](https://encore.dev/docs/ts/observability/dev-dash)
- [Documentation — Flow Diagram](https://encore.dev/docs/ts/observability/flow)
- [Documentation — Service Catalog](https://encore.dev/docs/ts/observability/service-catalog)
- [JSON Schema — Trace Event](json-schema/encore-trace-event-schema.json)
- [Naftiko Capability — Observability](capabilities/encore-observability.yaml)

### Encore MCP Server
Encore ships a built-in Model Context Protocol server (`encore mcp start` for SSE, `encore mcp run` for stdio) that exposes the live Encore application — services, middleware, auth handlers, databases, Pub/Sub topics, cron jobs, buckets, traces, metrics, source files, and documentation — to AI agents like Cursor and Claude Code. Agents can reason about and modify a running backend with full context.

**Human URL:** [https://encore.dev/docs/ts/cli/mcp](https://encore.dev/docs/ts/cli/mcp)

- [Documentation](https://encore.dev/docs/ts/cli/mcp)
- [Model Context Protocol](https://modelcontextprotocol.io)
- [Naftiko Capability — MCP](capabilities/encore-mcp.yaml)

## Common Properties

- [Portal — encore.dev](https://encore.dev)
- [Portal — encore.cloud](https://encore.cloud)
- [Documentation — All Docs](https://encore.dev/docs)
- [Documentation — Encore.ts](https://encore.dev/docs/ts)
- [Documentation — Encore.go](https://encore.dev/docs/go)
- [GettingStarted — TypeScript Quick Start](https://encore.dev/docs/ts/quick-start)
- [GettingStarted — Go Quick Start](https://encore.dev/docs/go/quick-start)
- [Pricing](https://encore.cloud/pricing)
- [GitHubOrganization](https://github.com/encoredev)
- [SourceCode — Encore Framework](https://github.com/encoredev/encore)
- [SourceCode — Examples](https://github.com/encoredev/examples)
- [SourceCode — Runtime API Contract](https://github.com/encoredev/encore.dev)
- [StatusPage](https://status.encore.cloud)
- [Blog — Engineering](https://encore.dev/blog)
- [ChangeLog](https://encore.dev/changelog)
- [Community — Discord](https://encore.dev/discord)
- [SDK — Encore CLI](https://encore.dev/docs/ts/cli/cli-reference)
- [SDK — Generated Clients (TS, Go, JS)](https://encore.dev/docs/ts/develop/client-generation)
- [SDK — Homebrew Tap](https://github.com/encoredev/homebrew-tap)
- [Documentation — AI Integration](https://encore.dev/docs/ts/ai-integration)
- [Documentation — Authentication](https://encore.dev/docs/ts/develop/auth)
- [Documentation — Middleware](https://encore.dev/docs/ts/develop/middleware)
- [Documentation — Streaming APIs](https://encore.dev/docs/ts/develop/streaming-apis)
- [Documentation — Use Cases](https://encore.dev/use-cases)

## Artifacts

Machine-readable specifications organized by format.

### OpenAPI

- [Encore Framework API](openapi/encore-framework-openapi.yml)
- [Encore Cloud Platform API](openapi/encore-platform-openapi.yml)

### JSON Schema

- [Encore API Endpoint](json-schema/encore-api-endpoint-schema.json)
- [Encore Service](json-schema/encore-service-schema.json)
- [Encore Infrastructure Resource](json-schema/encore-infrastructure-resource-schema.json)
- [Encore Trace Event](json-schema/encore-trace-event-schema.json)

### JSON-LD

- [Encore Context](json-ld/encore-dev-context.jsonld)

### Capabilities (Naftiko)

- [Framework](capabilities/encore-framework.yaml)
- [Infrastructure](capabilities/encore-infrastructure.yaml)
- [Platform](capabilities/encore-platform.yaml)
- [Observability](capabilities/encore-observability.yaml)
- [MCP](capabilities/encore-mcp.yaml)

### Commercial artifacts

- [Plans / Pricing](plans/encore-dev-plans-pricing.yml)
- [Rate Limits](rate-limits/encore-dev-rate-limits.yml)
- [FinOps Definition](finops/encore-dev-finops.yml)

### Vocabulary & Rules

- [Vocabulary](vocabulary/encore-dev-vocabulary.yml)
- [Spectral Rules](rules/encore-dev-rules.yml)

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
