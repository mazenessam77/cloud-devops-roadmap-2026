# Project 7 — Kubernetes

## Goal

Deploy the application after first proving it works in Docker Compose.

## Build

- Deployment and Service for API
- Ingress for HTTP routing
- ConfigMap and Secret (secret values injected outside Git)
- readiness/liveness probes on `/health`
- CPU/memory requests and limits
- PostgreSQL through a managed DB or a deliberately documented PVC-based lab
- Basic namespace and ServiceAccount/RBAC awareness
- A simple Helm chart or Helm values-based release

## Acceptance test

Scale replicas, view `kubectl get/describe/logs`, roll out a new image, and deliberately diagnose a wrong environment variable or probe configuration.

## Stretch

Add an HPA only after metrics are available and you can explain what it uses.
