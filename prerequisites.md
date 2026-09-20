# Useful prerequisites: understand what you deploy

This is **helpful background**, not a second roadmap. Learn enough to recognize how an application works when you deploy or troubleshoot it. You do **not** need to become a backend developer or a database administrator (DBA).

Read this after Linux and Git, alongside Bash/Python and Project 2. Return to it when a term appears in a Docker, cloud, or troubleshooting task.

## Application basics

| Topic | Enough for this roadmap |
|---|---|
| Client/server | A client sends a request; a server receives it and sends a response. |
| HTTP request/response | Know URL, method, headers, body, status code, and why 200, 404, 500, and 502 differ. |
| REST APIs | Recognize endpoints such as `GET /users` and `POST /users`; test them with `curl`. |
| JSON | Read and write simple objects and arrays exchanged by APIs. |
| Auth basics | Authentication identifies a user/service; authorization decides what it may do. Keep tokens out of Git and logs. |
| Environment variables | Configuration such as `PORT` or `DATABASE_URL` belongs outside source code. |
| Application ports | An app listens on a port; a reverse proxy/load balancer must forward to the correct one. |
| Logging | Logs record events and errors. Know where to find them and never log secrets. |
| Health checks | `/health` or a similar endpoint lets a platform decide whether an app is alive/ready. |

## Database basics

| Topic | Enough for this roadmap |
|---|---|
| SQL/database | A database stores tables and rows. Recognize basic `SELECT`, `INSERT`, `UPDATE`, and `DELETE`. |
| Connection pools | Apps reuse a limited set of database connections; too many or exhausted connections can cause failures. |
| Redis/cache | Redis often holds temporary cached values or sessions. A TTL is an expiration time; a cache is not automatically durable data. |

## Small practical target

Build or run a tiny API with `GET /health`, `GET /users`, and `POST /users`, backed by PostgreSQL. Set its database URL and port using environment variables. Then stop the database and inspect the application log. That is enough context for the Docker, cloud, CI/CD, Terraform, Kubernetes, and monitoring stages.

## What you do not need now

You do not need advanced framework design, microservices, database tuning, replication setup, query-planner expertise, or a full backend course. The deeper guides remain available in [docs/06-backend-api-basics.md](docs/06-backend-api-basics.md) and [docs/07-database-basics.md](docs/07-database-basics.md) when you need them.

## Completion check

- [ ] I can explain a request going from client to API to database and back.
- [ ] I can read JSON and use `curl` against a simple endpoint.
- [ ] I know why an app port, environment variable, log, and health endpoint matter.
- [ ] I can explain a table, connection pool, and cache without claiming DBA-level knowledge.
