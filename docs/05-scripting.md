# 05 — Scripting

## Why it matters

You do not need to be a software engineer, but repeated checks and changes should be automated.

## What to learn

In Bash: variables, quoting, conditions, loops, functions, files, exit codes, and environment variables. Use Python as the default second language: variables, functions, conditions, loops, JSON, files, HTTP requests, APIs, environment variables, and error handling.

## Practical examples

A health check reads `HEALTH_URL`, calls an endpoint with a timeout, prints a useful error, and exits non-zero on failure.

## Short lab (25 minutes)

Write `check-health.sh` and `check_health.py`. Read `HEALTH_URL` from the environment, call it, and test both a valid and invalid URL.

## Common mistakes

Hardcoding credentials, ignoring errors, parsing human-formatted output when JSON exists, or leaving Bash variables unquoted.

## When to move on

- [ ] I can write a small Bash check using variables and exit codes.
- [ ] I can write/read a small Python script that calls an HTTP API and handles errors.

## Trusted resources

[GNU Bash manual](https://www.gnu.org/software/bash/manual/) · [Python tutorial](https://docs.python.org/3/tutorial/) · [Python `json` docs](https://docs.python.org/3/library/json.html)
