# Project 1 — Linux Server

## Goal

Operate a small Linux web server and document how to diagnose it.

## Build

- Launch a Linux VM in a safe lab account.
- Connect over SSH with a key; create a non-root user with limited sudo.
- Install Nginx and publish a simple page.
- Create a small `systemd` service (for example, a health-check script or tiny API).
- Inspect `systemctl status`, `journalctl`, Nginx access/error logs, `ss -lntp`, `df -h`, and `free -h`.
- Open only HTTP/HTTPS and temporary restricted SSH access in firewall/security-group rules.

## Evidence to save

README screenshots or command output showing service status, listener, logs, and firewall rule—not private IPs, keys, or credentials.

## Stretch

Break the service by changing its port, identify the mismatch, and write the diagnosis.
