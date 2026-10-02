# Engineering Labs

Small experiments for questions that deserve measurement instead of opinion.

## Planned experiments

- SQL indexing and covering indexes
- Sargability
- Pagination strategies
- Large-table batch updates
- Deadlock reproduction
- EF Core vs Dapper trade-offs
- Async vs synchronous I/O
- Retry and backoff
- Idempotency
- Distributed locking
- Cache stampede
- Outbox / inbox patterns
- Rate limiting
- Allocation and memory behaviour
- OpenTelemetry tracing

## Experiment format

```text
Problem
  ↓
Hypothesis
  ↓
Implementation
  ↓
Measurement
  ↓
Result
  ↓
What changed my mind?
```

Measurements should include the environment and methodology. If there is no measurement, it is a note—not a benchmark.

## Current public experiments

- [KafkaDemo](https://github.com/trandat1114/KafkaDemo)
- [CSharp-Donace-Load-Test-Tool](https://github.com/trandat1114/CSharp-Donace-Load-Test-Tool)
