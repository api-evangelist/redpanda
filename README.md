# Redpanda (redpanda)

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

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/redpanda/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/redpanda/refs/heads/main/apis.yml)

## Tags

- Streaming
- Kafka
- Event Streaming
- Real-Time
- Data Platform
- Open Source
- C++
- Stream Processing

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-19

## APIs

### Redpanda Kafka API

Redpanda implements the Apache Kafka wire protocol natively, allowing existing Kafka clients (producers, consumers, AdminClient, Streams, Connect) to work unchanged against Redpanda brokers on TCP port 9092 (or the cluster's configured Kafka API port).

#### Tags

- Kafka
- Wire Protocol
- Producers
- Consumers

#### Properties

- [Documentation](https://docs.redpanda.com/current/develop/kafka-clients/)
- [API Reference](https://kafka.apache.org/protocol)

### Redpanda Admin API

The Redpanda Admin API is a built-in HTTP REST API (default port 9644) exposing cluster operations not covered by the Kafka protocol — broker membership, decommissioning, rebalance, license, debug bundle, configuration, leadership, security, and partitions.

#### Tags

- Admin
- Cluster
- Brokers
- Configuration
- Operations

#### Properties

- [Documentation](https://docs.redpanda.com/api/admin-api/)
- [API Reference](https://docs.redpanda.com/current/reference/api-reference/admin-api/)
- [OpenAPI](openapi/redpanda-admin-cluster-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Open Collection](collections/redpanda-admin-cluster.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/redpanda-admin-broker-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Open Collection](collections/redpanda-admin-broker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/redpanda-admin-partition-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Open Collection](collections/redpanda-admin-partition.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/redpanda-admin-debug-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Open Collection](collections/redpanda-admin-debug.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/redpanda-admin-transform-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Open Collection](collections/redpanda-admin-transform.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/redpanda-admin-usage-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Open Collection](collections/redpanda-admin-usage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Redpanda Schema Registry API

The Redpanda Schema Registry API is a Confluent-Schema-Registry-compatible REST API for managing Avro, JSON Schema, and Protobuf schema versions and subjects bound to topic events.

#### Tags

- Schema Registry
- Avro
- JSON Schema
- Protobuf

#### Properties

- [Documentation](https://docs.redpanda.com/current/manage/schema-reg/)
- [API Reference](https://docs.redpanda.com/api/schema-registry-api/)

### Redpanda HTTP Proxy (Pandaproxy) API

The Redpanda HTTP Proxy (Pandaproxy) provides a REST API for producing and consuming topic data without a Kafka client library, useful for environments where embedding a Kafka driver is impractical.

#### Tags

- HTTP Proxy
- REST
- Producers
- Consumers

#### Properties

- [Documentation](https://docs.redpanda.com/current/develop/http-proxy/)
- [API Reference](https://docs.redpanda.com/api/pandaproxy/)

### Redpanda Cloud Control Plane API

The Redpanda Cloud Control Plane API manages organization-wide resources — clusters, networks, resource groups, users, and serverless namespaces — across the Redpanda Cloud (Serverless, Dedicated, BYOC) deployments.

#### Tags

- Cloud
- Control Plane
- Clusters
- Networks
- Organizations
- Resource Groups

#### Properties

- [Documentation](https://docs.redpanda.com/redpanda-cloud/manage/api/)

### Redpanda Cloud Data Plane API

The Redpanda Cloud Data Plane API manages in-cluster resources — topics, ACLs, RBAC, users, schema registry, and connectors — for an individual Redpanda Cloud cluster.

#### Tags

- Cloud
- Data Plane
- Topics
- ACLs
- Users

#### Properties

- [Documentation](https://docs.redpanda.com/redpanda-cloud/manage/api/)

### Redpanda Console API

The Redpanda Console API powers the Redpanda Console UI (open-source) — topics, consumer groups, broker view, schema registry browsing, and ACL management — and can be called directly to embed Console functionality.

#### Tags

- Console
- UI
- Backend API

#### Properties

- [Documentation](https://docs.redpanda.com/current/manage/console/)
- [Source](https://github.com/redpanda-data/console)

### Redpanda Connect (Benthos) API

Redpanda Connect (formerly Benthos) is a declarative stream-processor exposing an HTTP API for managing pipelines, inputs, outputs, processors, and metrics — bridging Kafka, S3, databases, and HTTP sinks.

#### Tags

- Stream Processing
- Connectors
- Benthos
- ETL

#### Properties

- [Documentation](https://docs.redpanda.com/redpanda-connect/about/)
- [Source](https://github.com/redpanda-data/connect)

### Redpanda rpk CLI Surface

rpk is the Redpanda command-line tool, wrapping the Kafka, Admin, Schema Registry, and Cloud APIs into operator-friendly commands for deployment, configuration, topic management, ACLs, and benchmarking.

#### Tags

- CLI
- rpk
- Operations

#### Properties

- [Documentation](https://docs.redpanda.com/current/reference/rpk/)
- [Source](https://github.com/redpanda-data/redpanda)

### Redpanda Iceberg Topic API

Redpanda Iceberg Topics expose topic data as Apache Iceberg tables in object storage, accessible from the Iceberg REST catalog and consumable by query engines like Spark, Trino, and Snowflake.

#### Tags

- Iceberg
- Lakehouse
- Tiered Storage

#### Properties

- [Documentation](https://docs.redpanda.com/current/manage/iceberg/)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/redpanda-data)
- [Website](https://redpanda.com/)
- [Documentation](https://docs.redpanda.com/)
- [API Reference](https://docs.redpanda.com/api/)
- [Getting Started](https://docs.redpanda.com/current/get-started/)
- [Pricing](https://www.redpanda.com/pricing)
- [Sign Up](https://cloud.redpanda.com/signup)
- [Login](https://cloud.redpanda.com/)
- [GitHub Organization](https://github.com/redpanda-data)
- [Source](https://github.com/redpanda-data/redpanda)
- [License](https://github.com/redpanda-data/redpanda/blob/dev/licenses/bsl.md)
- [Helm  Charts](https://github.com/redpanda-data/helm-charts)
- [Console](https://github.com/redpanda-data/console)
- [Connect](https://github.com/redpanda-data/connect)
- [Operator](https://github.com/redpanda-data/redpanda-operator)
- [Examples](https://github.com/redpanda-data/redpanda-examples)
- [Status Page](https://status.redpanda.com/)
- [Blog](https://www.redpanda.com/blog)
- [Changelog](https://docs.redpanda.com/current/release-notes/)
- [Governance](https://www.redpanda.com/about)
- [X ( Twitter)](https://x.com/redpandadata)
- [YouTube](https://www.youtube.com/@RedpandaData)
- [Slack  Community](https://redpandacommunity.slack.com/)
- [rpk  C L I](https://docs.redpanda.com/current/reference/rpk/)
- [Plans](plans/redpanda-plans-pricing.yml)
- [Rate Limits](rate-limits/redpanda-rate-limits.yml)
- [Fin Ops](finops/redpanda-finops.yml)
- [Integrations](https://www.redpanda.com/partners)
- [M C P Server](https://www.redpanda.com/blog/building-low-code-mcp-servers-in-redpanda-cloud)
- [L L Ms Txt](https://docs.redpanda.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
