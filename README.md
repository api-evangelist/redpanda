# Redpanda (redpanda)

Redpanda is a Kafka API-compatible streaming data platform written in C++ with no JVM and no ZooKeeper, optimized for low latency and operational simplicity. The core broker is open source (BSL 1.1) and a fully managed cloud service (Serverless / Dedicated / BYOC) is offered commercially.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/redpanda/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=redpanda-api-evangelist&utm_content=repo)

## Type

- **x-type:** opensource

## Tags

 - Streaming, Kafka, Event Streaming, Real-Time, Data Platform, Open Source, C++, Stream Processing

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-08

## APIs

| API | Description |
|---|---|
| Redpanda Kafka API | Native Kafka wire protocol on TCP 9092 |
| Redpanda Admin API | HTTP REST cluster ops (port 9644) |
| Redpanda Schema Registry API | Confluent-Schema-Registry-compatible REST API |
| Redpanda HTTP Proxy (Pandaproxy) API | REST produce/consume without a Kafka client |
| Redpanda Cloud Control Plane API | Org / cluster / network management |
| Redpanda Cloud Data Plane API | In-cluster topics, ACLs, RBAC, schemas |
| Redpanda Console API | UI backend for topics, consumer groups, schemas |
| Redpanda Connect (Benthos) API | Declarative stream-processing pipelines |
| Redpanda rpk CLI | Operator CLI wrapping all APIs |
| Redpanda Iceberg Topic API | Topic data exposed as Apache Iceberg tables |

## Common Properties

- [Website](https://redpanda.com/)
- [Documentation](https://docs.redpanda.com/)
- [Pricing](https://www.redpanda.com/pricing)
- [GitHub Organization](https://github.com/redpanda-data)
- [Source (redpanda)](https://github.com/redpanda-data/redpanda)
- [Console (open-source)](https://github.com/redpanda-data/console)
- [Redpanda Connect](https://github.com/redpanda-data/connect)
- [License (BSL 1.1)](https://github.com/redpanda-data/redpanda/blob/dev/licenses/bsl.md)
- [Plans](plans/redpanda-plans-pricing.yml) — API Commons Plans 0.1 (reconciled)
- [RateLimits](rate-limits/redpanda-rate-limits.yml) — API Commons Rate Limits 0.1 (reconciled)
- [FinOps](finops/redpanda-finops.yml) — FOCUS-aligned FinOps Framework 1.0 (reconciled)

## Plans Summary

- **Community Edition** — BSL 1.1, free self-host
- **Enterprise (Self-Managed)** — annual license, adds tiered storage, SSO, RBAC, audit
- **Cloud Serverless** — usage-based, $100 trial credit
- **Cloud Dedicated** — single-tenant, throughput-tier hourly
- **Cloud BYOC** — managed in-customer-cloud, management fee + customer's own cloud bill

## Rate Limits Summary

- **Per-client producer/consumer bandwidth quotas** — configurable via Kafka quotas
- **Per-topic throughput quotas** — configurable
- **Connection-creation rate** — configurable
- **Cloud Serverless throughput tier** — tier-defined ingress + egress cap
- **Cloud partition quota** — per-tier

## Artifacts

| Artifact | Path |
|---|---|
| Plans | `plans/redpanda-plans-pricing.yml` |
| Rate Limits | `rate-limits/redpanda-rate-limits.yml` |
| FinOps | `finops/redpanda-finops.yml` |

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
