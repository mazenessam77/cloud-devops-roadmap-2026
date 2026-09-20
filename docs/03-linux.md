# 03 — Linux

## Why it matters

Linux runs many cloud workloads. The goal is to operate and troubleshoot a service safely, not memorize every command.

## What to learn

Learn files/directories, users/groups, permissions, `sudo`, shell/Bash, environment variables, pipes/redirection, `grep`, `find`, basic `awk`/`sed`, SSH, packages, processes/signals, cron, and logs. Learn `systemd` with `systemctl` and `journalctl`; inspect disk (`df -h`), memory (`free -h`), CPU (`top`), and listeners (`ss -lntp`).

## Practical examples

For a non-responsive app: check service status, service logs, listening port, local `curl`, then CPU/memory/disk and firewall rules.

## Short lab (30 minutes)

Install Nginx. Run `systemctl status nginx`, `curl localhost`, `sudo ss -lntp`, and `journalctl -u nginx -n 20`. Stop it, observe the failure, recover it, then make a copy of the welcome page unreadable and restore its permissions. Explain the evidence you used.

## Common mistakes

Using `sudo` blindly, restarting before reading logs, using `kill -9` first, or ignoring disk space.

## When to move on

- [ ] I can SSH in, manage files/permissions, and inspect processes.
- [ ] I can investigate a stopped or unreachable systemd service.

## Trusted resources

[Linux Journey](https://linuxjourney.com/) · [GNU Bash manual](https://www.gnu.org/software/bash/manual/) · [systemd documentation](https://systemd.io/)
