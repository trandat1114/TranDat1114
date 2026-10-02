# Dream Architecture

A collection of architecture sketches for systems I would like to design carefully before writing production code.

These are **design exercises**, not claims about production systems.

## Design checklist

Every system should make these visible:

1. **Boundaries** — what owns what?
2. **Data** — source of truth, read models, indexes, retention.
3. **Failure** — timeout, retry, duplicate, partial failure, poison message.
4. **Consistency** — where strong consistency matters and where eventual consistency is acceptable.
5. **Idempotency** — what happens when the same request/event arrives twice?
6. **Observability** — logs, metrics, traces, correlation IDs.
7. **Security** — identity, authorization, secrets, audit trail.
8. **Operations** — deployment, rollback, backup, recovery.
9. **Cost** — what scales with traffic and what remains fixed.
10. **Trade-offs** — what the design deliberately does not solve.

## Planned designs

### 001 — Large-scale Water Billing

```text
Customer / Mobile / Portal
          |
       API Gateway
          |
   +------+------+
   |             |
 Billing API   Payment API
   |             |
   +------+------+
          |
     Event Bus
          |
  +-------+--------+
  |       |        |
Invoice  Payment  Reporting
Worker   Worker    Pipeline
  |       |        |
  +-------+--------+
          |
     SQL / Read Models
          |
 Observability / Audit
```

Focus:
- billing-cycle processing
- payment reconciliation
- batch operations over large tables
- idempotent synchronization
- reporting without damaging transactional workloads

### 002 — Payment Reconciliation

Focus:
- bank transaction ingestion
- duplicate callbacks
- pending payments
- matching rules
- reconciliation queues
- auditability

### 003 — Booking Platform

Focus:
- inventory consistency
- reservation expiration
- concurrent booking
- payment boundary
- asynchronous confirmation

### 004 — Event-driven Commerce

Focus:
- order lifecycle
- outbox pattern
- consumers
- retries and dead-letter handling
- read models

### 005 — Personal Cloud

Focus:
- object storage
- metadata
- synchronization
- remote access
- backup and disaster recovery

## Decision record format

> Context → Decision → Alternatives → Failure modes → Operational consequences → What would change my mind?

These documents are deliberately allowed to be wrong. The point is to make the reasoning inspectable.
