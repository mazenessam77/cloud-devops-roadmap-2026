# 02 — Networking

## Why it matters

Deployments and outages often come down to a name, route, firewall rule, or port.

## What to learn

Learn IPv4, public/private IPs, CIDR and subnets, gateway and routing, ports, TCP/UDP, DNS, DHCP, NAT, and firewalls. HTTP carries web requests; HTTPS adds TLS. A load balancer spreads traffic; a reverse proxy forwards traffic to an app.

## Practical examples

The request path is `user → DNS → load balancer → application → database`. `curl` checks HTTP; `dig`/`nslookup` checks DNS; `ss -lntp` lists listening TCP ports.

## Short lab (20 minutes)

Run `dig example.com`, `curl -I https://example.com`, and `ss -lntp`. Then use `curl` against an intentionally wrong local port, identify the connection error, find the real listener, fix the port, and explain the result.

## Common mistakes

Treating ping as proof an app works, confusing IP and port, or opening every firewall port.

## When to move on

- [ ] I can explain IP, DNS, TCP, ports, HTTP, TLS, and a firewall.
- [ ] I can trace a basic request from browser to application.

## Trusted resources

[Cloudflare Learning Center](https://www.cloudflare.com/learning/) · [Cisco Networking Academy](https://www.netacad.com/courses/networking) · [MDN HTTP overview](https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/Overview)
