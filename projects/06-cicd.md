# Project 6 — CI/CD

## Goal

Automate the safe path from GitHub change to a test deployment.

```mermaid
flowchart LR
 GitHub --> Tests --> DockerBuild[Docker build] --> Registry --> Deploy
```

## Build

- Use GitHub Actions on pull requests/pushes.
- Run application tests and build the image.
- Tag image with immutable commit SHA and push to a registry using stored secrets.
- Deploy to a non-production target only after successful tests.
- Record deployment image tag and show logs on failure.

## Acceptance test

An intentional failing test prevents the build/deploy. A valid change produces a traceable deployed image. Never print secrets.

## Stretch

Add a basic dependency or image scan and triage one finding; do not block learning on building a large security pipeline.
