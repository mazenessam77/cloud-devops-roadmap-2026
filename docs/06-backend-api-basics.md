# 06 — Backend & API basics

## Why it matters

You do not need to become a backend developer, but you should understand the application you deploy.

## What to learn

Learn client/server, HTTP methods and status codes, headers, JSON, REST, authentication versus authorization, tokens, environment variables, ports, logs, health endpoints, reverse proxies, database connections, and connection pools.

## Practical examples

`GET /health` supports health checks. A 500 is an application failure; a 502 usually means a proxy could not use the upstream app. A wrong port prevents proxy-to-app traffic.

## Short lab (30 minutes)

Run the Project 2 API. Use `curl` to call `/health`, `GET /users`, and `POST /users`; change its configured port once, then read the error/log output.

## Common mistakes

Putting passwords in code, exposing stack traces, or treating an app as healthy only because its process exists.

## When to move on

- [ ] I can explain a request through proxy, API, and database.
- [ ] I can explain 500 versus 502 and why a health endpoint matters.

## Trusted resources

[MDN HTTP overview](https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/Overview) · [MDN HTTP status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Status) · [FastAPI tutorial](https://fastapi.tiangolo.com/tutorial/)
