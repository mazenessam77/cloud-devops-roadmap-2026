# 09 — Docker

## Why it matters

Containers package an application and dependencies consistently; they do not remove the need to understand logs, ports, or networking.

## What to learn

Learn containers versus VMs, images, containers, Dockerfiles, build/run, ports, volumes, networks, environment variables, logs, `exec`, registries, Docker Compose, multi-stage build basics, and health checks.

## Practical examples

Use `docker logs`, `docker exec`, and `docker compose logs -f` to investigate. A Dockerfile builds an image; Compose defines a multi-container application.

## Short lab (30 minutes)

Containerize Project 2 and run it with PostgreSQL and Nginx in Compose. Add a named volume and healthcheck; use `docker compose logs` to verify it. Then set one required environment variable to a bad value, inspect the failing container/logs, fix it, and explain the root cause.

## Common mistakes

Using `latest` blindly, baking secrets into images, running as root unnecessarily, or assuming a published port means healthy service.

## When to move on

- [ ] I can build, run, log into, and inspect an image/container.
- [ ] I can run an API, database, and proxy with Docker Compose.

## Trusted resources

[Docker get started](https://docs.docker.com/get-started/) · [Docker Compose](https://docs.docker.com/compose/) · [Dockerfile reference](https://docs.docker.com/reference/dockerfile/)
