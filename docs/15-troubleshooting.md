# 15 — Troubleshooting

## Why it matters

Troubleshooting is a calm evidence-gathering process, not a race to restart services.

## What to learn

Follow the request path: user → DNS → network → load balancer → server → container → application → database. Check recent deployments and investigate one layer at a time using DNS, ports, process/service state, logs, resource use, and dependency health.

## Practical examples

For a down website ask: does DNS resolve, is the port reachable, is the process/container running, what do logs say, can the app reach its database, are resources exhausted, and what changed recently?

| Scenario | First evidence to collect |
|---|---|
| 502 Bad Gateway | proxy target, app port, upstream logs |
| Service not listening | `systemctl status`, `ss -lntp`, journal logs |
| Disk full | `df -h`, application/journal errors |
| High CPU or memory | `top`, `free -h`, process/app logs |
| Container crash | container exit code, `docker logs`, environment/config |
| Wrong environment variable | deployed configuration and application logs |
| Database unavailable | connection error in app logs and database status |
| Failed deployment | CI/CD or Kubernetes event logs and the changed configuration |

A 502 points to a proxy/upstream issue; CrashLoopBackOff needs pod logs and description.

## Short lab (25 minutes)

Use this loop: **Build → Break → Troubleshoot → Fix → Explain**. In a safe local environment, change an app’s target port or environment variable so it fails. Diagnose it with `curl`, `ss`, service/container logs, and configuration; restore it and write a three-line incident note: symptom, root cause, and fix.

## Common mistakes

Restarting before collecting logs, changing several things at once, assuming the latest change is the cause, or treating an alert as a diagnosis.

## When to move on

- [ ] I can follow a request path and collect evidence at each layer.
- [ ] I can explain a basic diagnosis of a stopped service, 500/502, or container crash.

## Trusted resources

[Kubernetes debugging](https://kubernetes.io/docs/tasks/debug/) · [systemd journalctl manual](https://www.freedesktop.org/software/systemd/man/latest/journalctl.html) · [Google SRE incident response](https://sre.google/workbook/incident-response/)
