# 13 — Monitoring & observability

## Why it matters

You cannot operate a service confidently without evidence of its behavior.

## What to learn

Metrics are numeric measurements over time; logs are event records; traces follow requests across services. Start with Prometheus and Grafana. Watch CPU, memory, disk, request rate, error rate, and latency. Create alerts that have a clear owner and response.

## Practical examples

Metrics show what is happening; logs help explain it; traces follow a request. A sustained 5xx-rate alert should link to a dashboard and a first investigation step.

## Short lab (30 minutes)

Run Prometheus and Grafana locally or in Kubernetes. Create a dashboard for CPU/memory and one API request/error metric; trigger a controlled error and find its log.

## Common mistakes

Collecting everything without questions, alerting without response guidance, or logging secrets.

## When to move on

- [ ] I can explain metrics, logs, and traces.
- [ ] I can use a basic dashboard and describe one actionable alert.

## Trusted resources

[Prometheus overview](https://prometheus.io/docs/introduction/overview/) · [Grafana documentation](https://grafana.com/docs/grafana/latest/) · [OpenTelemetry documentation](https://opentelemetry.io/docs/)
