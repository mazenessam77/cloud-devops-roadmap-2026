# 12 — Kubernetes

## Why it matters

Kubernetes manages containerized workloads. Learn it only after Docker and networking are comfortable.

## What to learn

Learn cluster, control plane, worker node, Pod, ReplicaSet, Deployment, Service (ClusterIP/NodePort/LoadBalancer), Namespace, ConfigMap, Secret, Ingress, liveness/readiness probes, requests/limits, PV/PVC, StatefulSet/DaemonSet basics, Job/CronJob, RBAC, ServiceAccount, SecurityContext, HPA, and Helm basics.

## Practical examples

Use `kubectl get pods`, `kubectl describe pod`, and `kubectl logs` first. CrashLoopBackOff means the container repeatedly exits; inspect logs, config, probes, and resources.

## Short lab (30 minutes)

Use kind or minikube. Deploy an API with a Deployment, Service, ConfigMap, readiness probe, and CPU/memory requests; inspect it with `kubectl get`, `describe`, and `logs`.

## Common mistakes

Starting before Docker/networking, committing plaintext secrets, omitting requests/limits, or exposing every Service publicly.

## When to move on

- [ ] I can explain Pod, Deployment, Service, Ingress, ConfigMap, Secret, and probes.
- [ ] I can deploy and diagnose a basic application with `kubectl`.

## Trusted resources

[Kubernetes Basics](https://kubernetes.io/docs/tutorials/kubernetes-basics/) · [Kubernetes concepts](https://kubernetes.io/docs/concepts/) · [kubectl reference](https://kubernetes.io/docs/reference/kubectl/)
