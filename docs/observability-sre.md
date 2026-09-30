# Observability and SRE Interview Guide

## Core concepts

- Metrics, logs, traces and events
- SLI, SLO and SLA
- Error budgets
- p50, p95 and p99 latency
- Golden signals: latency, traffic, errors and saturation
- Alert fatigue
- Incident response
- Runbooks and postmortems

## Scenario

Users report intermittent 5xx responses but CPU is normal.

A strong investigation checks:

1. Error rate by endpoint/version.
2. Load balancer target health.
3. Application logs and traces.
4. Database/downstream latency.
5. Recent releases/configuration changes.
6. Saturation that CPU does not expose.
7. Whether rollback changes the signal.

Then define the prevention: SLO-based alerting, better tracing, deployment health gates or capacity controls.
