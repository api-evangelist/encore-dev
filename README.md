# Encore

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

Encore is a backend application framework and developer cloud that lets engineering teams build type-safe distributed systems in TypeScript (Encore.ts) and Go (Encore.go) using declarative Infrastructure from Code. Developers describe APIs, databases, Pub/Sub, object storage, caches, cron jobs, and secrets as typed code primitives; the framework provisions matching infrastructure locally with no Docker Compose, and Encore Cloud provisions equivalent managed resources in the customer's own AWS or GCP account. The platform ships built-in distributed tracing, a local development dashboard, auto-generated API docs and client SDKs, a Model Context Protocol server for AI agents, preview environments per pull request, and CI/CD — positioning Encore as an opinionated alternative to PaaS and a productivity layer on top of hyperscaler infrastructure.

**Areas:** Backend · Framework · Cloud · TypeScript · Go · Developer Tools · Infrastructure from Code · Microservices · Observability · Multi-Cloud

## Encore on APIs.io

Everything profiled for Encore is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/encore-dev/](https://apis.io/providers/encore-dev/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [Encore Infrastructure API](https://apis.io/apis/encore-dev/encore-infrastructure-api/) — Encore's Infrastructure from Code API lets developers declare cloud infrastructure resources — PostgreSQL databases, Pub/Sub topics and subscriptions,…
- [Encore Observability API](https://apis.io/apis/encore-dev/encore-observability-api/) — Encore captures distributed traces, structured logs, and runtime metrics automatically from every api(), database query, Pub/Sub publish, cron tick, and…
- [Encore MCP Server](https://apis.io/apis/encore-dev/encore-mcp-server/) — Encore ships a built-in Model Context Protocol server (`encore mcp start` for SSE, `encore mcp run` for stdio) that exposes the live Encore application —…
- [Encore Apps API](https://apis.io/apis/encore-dev/encore-dev-apps-api/) — The Apps API from Encore — 5 operation(s) for apps.
- [Encore API](https://apis.io/apis/encore-dev/encore-dev-encore-api/) — The Encore API from Encore — 2 operation(s) for encore.
- [Encore Framework API](https://apis.io/apis/encore-dev/encore-dev-encore-framework-api-api/) — The Encore Framework API API from Encore — 1 operation(s) for encore framework api.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [encore-dev](https://apis.io/servers/encore-dev/encore-dev/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Encore Dev Agentic Access](https://apis.io/agentic-access/encore-dev/encore-dev-agentic-access/)

#### JSON Schema (4)

The data models the API reads and writes.

- [Encore API Endpoint](https://apis.io/schemas/encore-dev/encore-api-endpoint/)
- [Encore Infrastructure Resource](https://apis.io/schemas/encore-dev/encore-infrastructure-resource/)
- [Encore Service](https://apis.io/schemas/encore-dev/encore-service/)
- [Encore Trace Event](https://apis.io/schemas/encore-dev/encore-trace-event/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Encore Dev Context](https://apis.io/jsonld/encore-dev/encore-dev-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Encore Vocabulary](https://apis.io/vocabularies/encore-dev/encore-dev-vocabulary/)

#### Collections (8)

Postman and Open Collection request collections.

- [Encore Framework Apps API](https://apis.io/collections/encore-dev/open-encore-dev-apps-api/)
- [Framework Apps Encore API](https://apis.io/collections/encore-dev/open-encore-dev-encore-api/)
- [Encore Framework Apps Encore Framework API API](https://apis.io/collections/encore-dev/open-encore-dev-encore-framework-api-api/)
- [Encore Framework API](https://apis.io/collections/encore-dev/open-encore-framework/)
- [Encore Cloud Platform API](https://apis.io/collections/encore-dev/open-encore-platform/)
- [Encore Framework Apps API](https://apis.io/collections/encore-dev/postman-encore-dev-apps-api/)
- [Framework Apps Encore API](https://apis.io/collections/encore-dev/postman-encore-dev-encore-api/)
- [Encore Framework Apps Encore Framework API API](https://apis.io/collections/encore-dev/postman-encore-dev-encore-framework-api-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Encore — jsonschema rules](https://apis.io/rules/encore-dev/encore-dev-jsonschema-spectral-rules/)
- [Encore API Rules](https://apis.io/rules/encore-dev/encore-dev-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Encore Dev Domain Security](https://apis.io/security/encore-dev/encore-dev-domain-security/)
- [Encore Dev Vulnerability Disclosure](https://apis.io/security/encore-dev/encore-dev-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Encore Dev Plans Pricing](https://apis.io/plans/encore-dev/encore-dev-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Encore Dev Rate Limits](https://apis.io/rate-limits/encore-dev/encore-dev-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Encore Dev Finops](https://apis.io/finops/encore-dev/encore-dev-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.encore.dev/)
- [Documentation](https://encore.dev/docs)
- [Getting started](https://encore.dev/docs/ts/quick-start)
- [Pricing](https://encore.cloud/pricing)
- [Changelog](https://encore.dev/changelog)
- [Blog](https://encore.dev/blog)
- [GitHub](https://github.com/encoredev)
- [Status](https://status.encore.cloud)

## API Evangelist rating

**Kin Score 45.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 60.0 |
| Contract quality | 55.2 |
| Contract governance | 27.3 |
| Operational transparency | 55.3 |
| Developer ergonomics | 56.0 |
| Access clarity | 18.4 |

**Agent readiness 47.9** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 22.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/encore-dev/](https://apis.io/providers/encore-dev/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Encore: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/encore-dev/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
