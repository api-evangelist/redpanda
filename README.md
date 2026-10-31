# Redpanda

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

Redpanda is a Kafka API-compatible streaming data platform written in C++ with no JVM and no ZooKeeper, optimized for low latency and operational simplicity. The core broker (redpanda) is open source and available under the Business Source License 1.1, and a fully managed cloud service (Redpanda Cloud — Serverless, Dedicated, BYOC) is offered commercially. Redpanda Connect (formerly Benthos) provides stream processing. The platform exposes the Kafka wire protocol, an Admin API, a Schema Registry API, an HTTP Proxy (Pandaproxy), Kafka-compatible client APIs, and the Redpanda Cloud Control Plane and Data Plane APIs for managed deployments.

**Areas:** Streaming · Kafka · Event Streaming · Real-Time · Data Platform · Open Source · C++ · Stream Processing

## Redpanda on APIs.io

Everything profiled for Redpanda is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/redpanda/](https://apis.io/providers/redpanda/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [Redpanda Kafka API](https://apis.io/apis/redpanda/redpanda-kafka-api/) — Redpanda implements the Apache Kafka wire protocol natively, allowing existing Kafka clients (producers, consumers, AdminClient, Streams, Connect) to work…
- [Redpanda Admin API](https://apis.io/apis/redpanda/redpanda-admin-api/) — The Redpanda Admin API is a built-in HTTP REST API (default port 9644) exposing cluster operations not covered by the Kafka protocol — broker membership,…
- [Redpanda Schema Registry API](https://apis.io/apis/redpanda/redpanda-schema-registry-api/) — The Redpanda Schema Registry API is a Confluent-Schema-Registry-compatible REST API for managing Avro, JSON Schema, and Protobuf schema versions and…
- [Redpanda HTTP Proxy (Pandaproxy) API](https://apis.io/apis/redpanda/redpanda-http-proxy-api/) — The Redpanda HTTP Proxy (Pandaproxy) provides a REST API for producing and consuming topic data without a Kafka client library, useful for environments…
- [Redpanda Cloud Control Plane API](https://apis.io/apis/redpanda/redpanda-cloud-control-plane-api/) — The Redpanda Cloud Control Plane API manages organization-wide resources — clusters, networks, resource groups, users, and serverless namespaces — across…
- [Redpanda Cloud Data Plane API](https://apis.io/apis/redpanda/redpanda-cloud-data-plane-api/) — The Redpanda Cloud Data Plane API manages in-cluster resources — topics, ACLs, RBAC, users, schema registry, and connectors — for an individual Redpanda…
- [Redpanda Console API](https://apis.io/apis/redpanda/redpanda-console-api/) — The Redpanda Console API powers the Redpanda Console UI (open-source) — topics, consumer groups, broker view, schema registry browsing, and ACL management —…
- [Redpanda Connect (Benthos) API](https://apis.io/apis/redpanda/redpanda-connect-api/) — Redpanda Connect (formerly Benthos) is a declarative stream-processor exposing an HTTP API for managing pipelines, inputs, outputs, processors, and metrics…
- [Redpanda rpk CLI Surface](https://apis.io/apis/redpanda/redpanda-rpk-api/) — rpk is the Redpanda command-line tool, wrapping the Kafka, Admin, Schema Registry, and Cloud APIs into operator-friendly commands for deployment,…
- [Redpanda Iceberg Topic API](https://apis.io/apis/redpanda/redpanda-iceberg-topic-api/) — Redpanda Iceberg Topics expose topic data as Apache Iceberg tables in object storage, accessible from the Iceberg REST catalog and consumable by query…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (2)

Model Context Protocol servers that expose the API to agents.

- [MCP Server](https://apis.io/servers/redpanda/mcp-server/)
- [redpanda](https://apis.io/servers/redpanda/redpanda/)

#### Collections (6)

Postman and Open Collection request collections.

- [API Collection](https://apis.io/collections/redpanda/open-redpanda-admin-broker/)
- [API Collection](https://apis.io/collections/redpanda/open-redpanda-admin-cluster/)
- [API Collection](https://apis.io/collections/redpanda/open-redpanda-admin-debug/)
- [API Collection](https://apis.io/collections/redpanda/open-redpanda-admin-partition/)
- [API Collection](https://apis.io/collections/redpanda/open-redpanda-admin-transform/)
- [API Collection](https://apis.io/collections/redpanda/open-redpanda-admin-usage/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Redpanda Domain Security](https://apis.io/security/redpanda/redpanda-domain-security/)
- [Redpanda Trust Center](https://apis.io/security/redpanda/redpanda-trust-center/)
- [Redpanda Vulnerability Disclosure](https://apis.io/security/redpanda/redpanda-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Redpanda Plans Pricing](https://apis.io/plans/redpanda/redpanda-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Redpanda Rate Limits](https://apis.io/rate-limits/redpanda/redpanda-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Redpanda Finops](https://apis.io/finops/redpanda/redpanda-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://redpanda.com/)
- [Documentation](https://docs.redpanda.com/)
- [Getting started](https://docs.redpanda.com/current/get-started/)
- [API reference](https://docs.redpanda.com/api/)
- [Pricing](https://www.redpanda.com/pricing)
- [Changelog](https://docs.redpanda.com/current/release-notes/)
- [Blog](https://www.redpanda.com/blog)
- [GitHub](https://github.com/redpanda-data)
- [Status](https://status.redpanda.com/)

## API Evangelist rating

**Kin Score 33.2** — thin · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 63.3 |
| Contract quality | 30.5 |
| Contract governance | 0.0 |
| Operational transparency | 36.8 |
| Developer ergonomics | 38.1 |
| Access clarity | 32.9 |

**Agent readiness 23.5** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/redpanda/](https://apis.io/providers/redpanda/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Redpanda: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/redpanda/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
