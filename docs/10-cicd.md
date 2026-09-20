# 10 — CI/CD

## Why it matters

CI/CD makes delivery repeatable and reviewable. Start with GitHub Actions and a small safe workflow.

## What to learn

CI builds/tests changes. Continuous Delivery keeps releases deployable; Continuous Deployment releases automatically. Learn workflows, jobs, steps, triggers, artifacts, secrets, environments, build, test, and deploy.

## Practical examples

Use `push → test → build image → push registry → deploy`. Tag images with an immutable commit SHA and store credentials as repository/environment secrets.

## Short lab (25 minutes)

Create a GitHub Actions workflow that checks out Project 2, installs dependencies, and runs tests. Intentionally make a test or configuration step fail, inspect the workflow log, fix it, rerun it, and explain why the deployment did not proceed.

## Common mistakes

Leaking secrets in logs, deploying untested code, and relying only on mutable image tags.

## When to move on

- [ ] I can explain a workflow, job, step, artifact, and secret.
- [ ] I can make a push trigger tests and understand a failed run.

## Trusted resources

[GitHub Actions quickstart](https://docs.github.com/en/actions/get-started/quickstart) · [GitHub Actions CI](https://docs.github.com/en/actions/get-started/continuous-integration)
