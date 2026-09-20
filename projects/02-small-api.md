# Project 2 — Small API

## Goal

Understand an application before automating it.

## Build

Use FastAPI, Node.js, Go, or .NET to create:

- `GET /health`
- `GET /users`
- `POST /users`
- PostgreSQL persistence with a `users` table
- Structured/useful request and error logs
- Configuration from `DATABASE_URL` and other environment variables

## Acceptance test

`curl /health` returns a success response; `POST /users` creates one user; `GET /users` returns it; stopping the database creates an understandable logged failure. Do not commit `.env`.

## Stretch

Put Nginx in front of the API and explain a deliberate 502 caused by a wrong upstream port.
