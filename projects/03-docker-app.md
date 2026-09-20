# Project 3 — Docker application

## Goal

Run the same application as a reproducible three-service stack.

## Build

- Containerize backend API with a Dockerfile.
- Run PostgreSQL with a named volume.
- Run Nginx as the public entry point.
- Define backend/database/internal networking in Docker Compose.
- Use environment variables and `.dockerignore`; do not bake secrets into images.
- Add a backend healthcheck and document `docker compose logs`, `ps`, `exec`, and `down`.

## Architecture

`Nginx → API → PostgreSQL`. Verify persistence by recreating containers without removing the database volume.

## Stretch

Use a multi-stage build and run the API as a non-root user.
