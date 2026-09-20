# How to follow the roadmap

## Where to start

Start with [ROADMAP.md](ROADMAP.md) to see the whole path. Then work through the numbered docs in this exact order. Use one notebook or repository to save commands, notes, mistakes, and project evidence. Do not study several stages at once.

1. Computer Basics → Networking → Linux
2. Git → Bash + Python/Go
3. Read [prerequisites.md](prerequisites.md) while building the small API; this is useful context, not a detour.
4. Choose one cloud provider → Docker → CI/CD → Terraform
5. Kubernetes → Monitoring & Observability → Basic Security
6. Complete and document projects as you go.

## When to move on

Move on when you can explain the topic simply, complete its lab without blindly copying commands, and diagnose one small intentional failure. You do not need to memorize every command, finish every resource, or earn a certification before continuing.

## Readiness checks by stage

### Computer basics

- [ ] I can explain CPU, RAM, disk, process, and client/server.
- [ ] I can use `ps`, `free -h`, and `df -h` to inspect a machine.

### Networking

- [ ] I can explain IP, DNS, TCP, ports, HTTP, and a firewall.
- [ ] I can use `curl`, `dig`/`nslookup`, and `ss` for a basic connection check.

### Linux

- [ ] I can navigate files, use permissions, connect with SSH, and use `sudo` carefully.
- [ ] I can inspect a service with `systemctl`, `journalctl`, logs, `ss`, `df -h`, and `free -h`.

### Git and scripting

- [ ] I can branch, commit, push, and open a pull request.
- [ ] I can write a small Bash health-check script and a Python/Go script that reads config and handles errors.

### Cloud

- [ ] I can use one provider’s IAM, network, VM, storage, load balancer, managed database, logs, and cost controls.
- [ ] I can explain public/private networking and avoid public database access.

### Docker

- [ ] I can build an image, run it, inspect logs, and use Docker Compose for API + database + Nginx.
- [ ] I can explain image versus container and where environment variables/volumes belong.

### CI/CD and Terraform

- [ ] I can make GitHub Actions test and build an image, with secrets stored safely.
- [ ] I can run `terraform init`, `plan`, and `apply`, explain state, and clean up a lab safely.

### Kubernetes

- [ ] I can deploy an app with Deployment, Service, Ingress, ConfigMap, Secret, probes, and requests/limits.
- [ ] I can inspect a failing Pod with `kubectl get`, `describe`, and `logs`.

### Monitoring and security

- [ ] I can use a Grafana dashboard for CPU/memory and request/error/latency metrics.
- [ ] I can explain logs versus metrics versus traces, least privilege, TLS, and secret handling.

## What level is enough?

At every stage, aim for **working competence**: build one small thing, explain it in everyday language, and troubleshoot a common failure. Skip advanced internals and learn them only when a real project or job needs them. The [Learn Later section](ROADMAP.md#learn-later) names those topics.

## When to start applying

Start applying when you can demonstrate Projects 3–6 and most of the [job-ready checklist](job-ready-checklist.md). You should be able to walk through your architecture, deployment route, logs/metrics, secure configuration, and one failure you fixed. Do not wait for Kubernetes mastery, every optional project, or advanced engineering topics; continue learning while you apply.
