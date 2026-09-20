# 14 — Basic security

## Why it matters

Security is daily operational hygiene: limit access, protect credentials, encrypt traffic, and update software.

## What to learn

Learn least privilege, IAM, MFA, secret management, TLS, secure SSH, narrow firewall rules, image/dependency scanning basics, Kubernetes RBAC, non-root containers, and routine updates.

## Practical examples

Use an IAM role or service account rather than long-lived keys. Put a database password in a secret manager or local environment file, never source code, an image, or logs.

## Short lab (20 minutes)

Enable MFA; add `.env` to `.gitignore`; move a sample password from code into an environment variable; run a container as a non-root user if its image supports it.

## Common mistakes

Wide-open SSH, committing `.env`, using administrator access for everything, assuming Base64 is encryption, or delaying updates indefinitely.

## When to move on

- [ ] I can explain least privilege, secret handling, TLS, and secure SSH basics.
- [ ] I can keep credentials out of Git and narrow basic network access.

## Trusted resources

[OWASP Top 10](https://owasp.org/www-project-top-ten/) · [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/) · [AWS IAM best practices](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)
