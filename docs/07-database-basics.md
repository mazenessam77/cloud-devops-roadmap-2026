# 07 — Database basics

## Why it matters

Applications depend on data. Operations work needs enough database knowledge to connect safely, diagnose basic failures, and protect data.

## What to learn

Use PostgreSQL: database, table, row, primary/foreign keys, `SELECT`, `INSERT`, `UPDATE`, `DELETE`, indexes, transactions, connections, pools, backups/restores, and primary/replica concepts. Know Redis as an in-memory cache with TTLs and possible session storage.

## Practical examples

A connection pool avoids opening a database connection for every request. A backup only counts when a restore test succeeds.

## Short lab (25 minutes)

Run PostgreSQL in Docker, create a `users` table, insert/select one row, then export and restore a small test database.

## Common mistakes

Publicly exposing databases, storing credentials in Git, skipping restore tests, or adding indexes without a reason.

## When to move on

- [ ] I can run basic SQL and explain a table, index, connection pool, and backup.
- [ ] I can explain why Redis/cache data may expire and differ from durable data.

## Trusted resources

[PostgreSQL tutorial](https://www.postgresql.org/docs/current/tutorial.html) · [PostgreSQL backup/restore](https://www.postgresql.org/docs/current/backup.html) · [Redis documentation](https://redis.io/docs/latest/)
