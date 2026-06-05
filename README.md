# Encore (encore-dev)

Encore is a backend application framework and developer cloud that lets engineering teams build type-safe distributed systems in TypeScript (Encore.ts) and Go (Encore.go) using declarative Infrastructure from Code. Developers describe APIs, databases, Pub/Sub, object storage, caches, cron jobs, and secrets as typed code primitives; the framework provisions matching infrastructure locally with no Docker Compose, and Encore Cloud provisions equivalent managed resources in the customer's own AWS or GCP account. The platform ships built-in distributed tracing, a local development dashboard, auto-generated API docs and client SDKs, a Model Context Protocol server for AI agents, preview environments per pull request, and CI/CD — positioning Encore as an opinionated alternative to PaaS and a productivity layer on top of hyperscaler infrastructure.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/encore-dev/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/encore-dev/refs/heads/main/apis.yml)

## Scope

- **Position:** Producing

## Tags

- Backend
- Framework
- Cloud
- TypeScript
- Go
- DeveloperTools
- InfrastructureFromCode
- Microservices
- Observability
- Multicloud

## Timestamps

- **Created:** 2026-05-24T00:00:00.000Z
- **Modified:** 2026-05-24

## APIs

### Encore Framework API

The Encore Framework API is the in-process declarative API surface developers use inside Encore.ts and Encore.go applications. Endpoints are declared with the api() function (TypeScript) or //encore:api annotation (Go), specifying method, path, expose (public vs internal), auth, and optional sensitive flags. Encore parses the source to derive request/response schemas from TypeScript interfaces or Go structs, enforces runtime validation, and wires up service-to-service calls without manual HTTP plumbing. Raw endpoints, fallback routes, path parameters, query, header, and cookie parameters are all first-class.

- **Human URL:** [https://encore.dev/docs/ts/primitives/defining-apis](https://encore.dev/docs/ts/primitives/defining-apis)

#### Tags

- Backend
- Framework
- APIs
- Microservices
- TypeScript
- Go

#### Properties

- [Documentation](https://encore.dev/docs/ts/primitives/defining-apis)
- [Documentation](https://encore.dev/docs/go/primitives/defining-apis)
- [OpenAPI](openapi/encore-framework-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/encore-framework.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encore-framework.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/encore-api-endpoint-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/encore-service-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/encore-dev-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Encore Infrastructure API

Encore's Infrastructure from Code API lets developers declare cloud infrastructure resources — PostgreSQL databases, Pub/Sub topics and subscriptions, object storage buckets, cron jobs, caches, and secrets — as typed code primitives inside their backend. Encore parses these declarations to provision matching infrastructure locally (Docker-free) for development and on AWS or GCP in production via Encore Cloud, without Terraform, YAML, or manual wiring.

- **Human URL:** [https://encore.dev/docs/ts/primitives](https://encore.dev/docs/ts/primitives)

#### Tags

- Backend
- Infrastructure
- Databases
- PubSub
- Caching
- ObjectStorage
- Cron
- Secrets

#### Properties

- [Documentation](https://encore.dev/docs/ts/primitives)
- [Documentation](https://encore.dev/docs/ts/primitives/databases)
- [Documentation](https://encore.dev/docs/ts/primitives/pubsub)
- [Documentation](https://encore.dev/docs/ts/primitives/cron-jobs)
- [Documentation](https://encore.dev/docs/ts/primitives/object-storage)
- [Documentation](https://encore.dev/docs/ts/primitives/secrets)
- [JSON Schema](json-schema/encore-infrastructure-resource-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Postman Collection](collections/encore-framework.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encore-framework.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/encore-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encore-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Encore Cloud Platform API

Encore Cloud is the optional hosted platform that takes an Encore application from `git push encore` to a running production deployment in the customer's own AWS or GCP account. The platform handles infrastructure provisioning (managed Postgres, SQS/SNS or Pub/Sub, S3/GCS buckets, IAM, secrets), CI/CD, preview environments per pull request, distributed tracing ingest, metrics, logs, and the developer dashboard at app.encore.cloud.

- **Human URL:** [https://encore.dev/docs/platform](https://encore.dev/docs/platform)

#### Tags

- Cloud
- Deployment
- CICD
- Environments
- Multicloud

#### Properties

- [Documentation](https://encore.dev/docs/platform)
- [Portal](https://encore.cloud)
- [OpenAPI](openapi/encore-platform-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/encore-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encore-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Encore Observability API

Encore captures distributed traces, structured logs, and runtime metrics automatically from every api(), database query, Pub/Sub publish, cron tick, and outbound HTTP call. The local Development Dashboard surfaces traces, the service catalog, an auto-generated architecture flow diagram, the database explorer, and the API explorer. In production, traces and metrics ship to Encore Cloud (20M events/month included on Pro) or forward to Datadog, Grafana, Sentry, and other third-party backends.

- **Human URL:** [https://encore.dev/docs/ts/observability/tracing](https://encore.dev/docs/ts/observability/tracing)

#### Tags

- Observability
- Tracing
- Metrics
- Logs
- DevDashboard

#### Properties

- [Documentation](https://encore.dev/docs/ts/observability/tracing)
- [Documentation](https://encore.dev/docs/ts/observability/dev-dash)
- [Documentation](https://encore.dev/docs/ts/observability/flow)
- [Documentation](https://encore.dev/docs/ts/observability/service-catalog)
- [JSON Schema](json-schema/encore-trace-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Postman Collection](collections/encore-framework.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encore-framework.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/encore-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encore-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Encore MCP Server

Encore ships a built-in Model Context Protocol server (`encore mcp start` for SSE, `encore mcp run` for stdio) that exposes the live Encore application — services, middleware, auth handlers, databases, Pub/Sub topics, cron jobs, buckets, traces, metrics, source files, and documentation — to AI agents like Cursor and Claude Code. This lets agents reason about and modify a running backend with full context, including verifying that a newly added publish call shows up in traces.

- **Human URL:** [https://encore.dev/docs/ts/cli/mcp](https://encore.dev/docs/ts/cli/mcp)

#### Tags

- AI
- MCP
- ModelContextProtocol
- AgenticAI
- DeveloperTools

#### Properties

- [Documentation](https://encore.dev/docs/ts/cli/mcp)
- [Documentation](https://modelcontextprotocol.io)
- [Postman Collection](collections/encore-framework.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encore-framework.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/encore-platform.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encore-platform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/encoredev)
- [Source Code](https://github.com/encoredev/encore)
- [Source Code](https://github.com/encoredev/examples)
- [Source Code](https://github.com/encoredev/encore.dev)
- [Documentation](https://encore.dev/docs)
- [Documentation](https://encore.dev/docs/ts)
- [Documentation](https://encore.dev/docs/go)
- [Getting Started](https://encore.dev/docs/ts/quick-start)
- [Getting Started](https://encore.dev/docs/go/quick-start)
- [Portal](https://encore.cloud)
- [Pricing](https://encore.cloud/pricing)
- [Blog](https://encore.dev/blog)
- [Changelog](https://encore.dev/changelog)
- [Status Page](https://status.encore.cloud)
- [Community](https://encore.dev/discord)
- [Documentation](https://encore.dev/docs/ts/cli/mcp)
- [Documentation](https://encore.dev/docs/ts/ai-integration)
- [Documentation](https://encore.dev/docs/ts/observability/tracing)
- [Documentation](https://encore.dev/docs/ts/observability/dev-dash)
- [Documentation](https://encore.dev/docs/ts/primitives/databases)
- [Documentation](https://encore.dev/docs/ts/primitives/pubsub)
- [Documentation](https://encore.dev/docs/ts/primitives/cron-jobs)
- [Documentation](https://encore.dev/docs/ts/primitives/object-storage)
- [Documentation](https://encore.dev/docs/ts/primitives/secrets)
- [Documentation](https://encore.dev/docs/ts/develop/auth)
- [Documentation](https://encore.dev/docs/ts/develop/middleware)
- [Documentation](https://encore.dev/docs/ts/develop/streaming-apis)
- [SDK](https://encore.dev/docs/ts/cli/cli-reference)
- [SDK](https://encore.dev/docs/ts/develop/client-generation)
- [Documentation](https://encore.dev/docs/ts/develop/api-docs)
- [SDK](https://github.com/encoredev/homebrew-tap)
- [Documentation](https://encore.dev/use-cases)
- [Plans](plans/encore-dev-plans-pricing.yml)
- [Rate Limits](rate-limits/encore-dev-rate-limits.yml)
- [Fin Ops](finops/encore-dev-finops.yml)
- [Vocabulary](vocabulary/encore-dev-vocabulary.yml)
- [Spectral Rules](rules/encore-dev-rules.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
