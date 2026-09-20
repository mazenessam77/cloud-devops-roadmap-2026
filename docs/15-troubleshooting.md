# 15 — Troubleshooting

## Why it matters

Troubleshooting is a calm evidence-gathering process, not a race to restart services.

## What to learn

Follow the request path: user → DNS → network → load balancer → server → container → application → database. Check recent deployments and investigate one layer at a time using DNS, ports, process/service state, logs, resource use, and dependency health.

## Practical examples

For a down website ask: does DNS resolve, is the port reachable, is the process/container running, what do logs say, can the app reach its database, are resources exhausted, and what changed recently? A 502 points to a proxy/upstream issue; CrashLoopBackOff needs pod logs and description.

## Short lab (25 minutes)

In a safe local environment, change an app’s target port or environment variable so it fails. Diagnose it with `curl`, `ss`, service/container logs, and configuration; restore it and write a three-line incident note.

## Common mistakes

Restarting before collecting logs, changing several things at once, assuming the latest change is the cause, or treating an alert as a diagnosis.

## When to move on

- [ ] I can follow a request path and collect evidence at each layer.
- [ ] I can explain a basic diagnosis of a stopped service, 500/502, or container crash.

## Trusted resources

[Kubernetes debugging](https://kubernetes.io/docs/tasks/debug/) · [systemd journalctl manual](https://www.freedesktop.org/software/systemd/man/latest/journalctl.html) · [Google SRE incident response](https://sre.google/workbook/incident-response/)
