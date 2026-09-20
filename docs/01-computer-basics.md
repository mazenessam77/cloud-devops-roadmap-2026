# 01 — Computer basics

## Why it matters

Cloud resources are rented computers. CPU, RAM, disk, and processes explain many first troubleshooting clues.

## What to learn

CPU executes work; cores allow parallel work. RAM holds active programs/data; disk persists files. A process is a running program; a thread is a smaller execution path. The operating system manages hardware, files, users, and processes. In client/server, a client asks and a server responds.

## Practical examples

High CPU can slow work; full disk can stop logs or writes; a running process can still be unhealthy.

## Short lab (15 minutes)

On Linux run `nproc`, `free -h`, `df -h`, and `ps aux | head`. Identify CPU cores, available memory, disk free space, and one running process.

## Common mistakes

Confusing RAM with disk, or assuming a process exists means its service works.

## When to move on

- [ ] I can explain CPU, RAM, disk, process, thread, and client/server plainly.
- [ ] I can inspect basic machine resources.

## Trusted resources

[Linux Foundation free courses](https://training.linuxfoundation.org/resources/free-courses/) · [Linux Journey](https://linuxjourney.com/)
