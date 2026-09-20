# How to follow the roadmap

Start at Phase 0 and move down the list. **Follow the stages in order, but allow small overlaps during projects.** For example, you can improve a Bash script while starting cloud labs. Move on when you can explain the basics, complete the practical task, and diagnose one small failure.

For major labs, use this loop: **Build → Break → Troubleshoot → Fix → Explain**. Break only safe local or disposable lab environments; record the symptom, evidence, root cause, and fix.

## Security throughout every phase

Security starts on day one: use least privilege and MFA in cloud, keep secrets out of Git and logs, use TLS for web traffic, restrict network access, scan/update dependencies, and avoid running containers as root where practical. It is not a final stage to postpone.

## 0. Foundations — Computer Basics, Networking, Linux, Git

**Study:** CPU/RAM/disk/processes; IP, DNS, TCP, ports, HTTP; Linux files, permissions, services, logs, SSH; Git commits, branches, and Pull Requests.

**Goal:** Be comfortable using a Linux machine and tracing a basic web request.

**Build:** Complete Project 1: launch a Linux VM, connect with SSH, install Nginx, open only needed access, and inspect logs.

**Move on when:** You can use `curl`, `dig`/`nslookup`, `ss`, `systemctl`, and `journalctl` to investigate a simple service issue; you can also commit and push your work with Git.

### Optional open-source practice

After Git/GitHub basics, open source is strongly recommended for real collaboration practice, but it is **not required** for job readiness. Start small: fix documentation or a README, correct an example, add a small test, report a reproducible bug, or improve a script/CI workflow.

The normal workflow is: **Fork → Branch → Change → Test → Pull Request**. Read the project’s contribution guide, keep the change small, and describe what you tested.

## 1. Automation — Bash + Python/Go

**Study:** Bash variables, conditions, loops, functions, exit codes, and environment variables; then simple Python or Go for JSON and HTTP APIs.

**Goal:** Automate repetitive checks instead of relying on manual steps.

**Build:** A health-check script that reads a URL from an environment variable, calls it with a timeout, and returns success or failure.

**Move on when:** You can write a small script, handle an expected error, and explain its exit code.

## 2. Required prerequisite project — API + PostgreSQL

**Study:** [prerequisites.md](prerequisites.md): backend flow, APIs, and basic database design.

**Goal:** Understand what you will later containerize, deploy, and operate.

**Build:** A small API connected to PostgreSQL, with a simple related schema, CRUD endpoints, environment variables, logs, and `/health`.

**Move on when:** You can explain how a request reaches the API and reads/writes database data, and you built the project yourself.

## 3. Cloud — Choose One Provider

**Study:** Choose AWS, Azure, or GCP. Learn IAM, virtual networking, VM/compute, object storage, load balancing, managed databases, logs, and cost controls.

**Goal:** Deploy a simple workload securely on one cloud without trying to learn every provider.

**Build:** Create a small network, VM, restrictive firewall/security rules, object-storage bucket, and budget alert in a sandbox account.

**Move on when:** You can explain public versus private networking, least-privilege access, and where to find application or VM logs.

## 4. Containers — Docker

**Study:** Images, containers, Dockerfiles, ports, volumes, networks, logs, environment variables, and Docker Compose.

**Goal:** Run the same application consistently on your machine and later in cloud environments.

**Build:** Complete Project 3: run Nginx, your backend API, and PostgreSQL with Docker Compose.

**Move on when:** You can build an image, inspect container logs, enter a container, and explain how services communicate in Compose.

## 5. Automation & Infrastructure — CI/CD + Terraform

**Study:** GitHub Actions workflow/job/step/secrets; Terraform providers, resources, variables, outputs, plan, apply, destroy, and state.

**Goal:** Make delivery repeatable and infrastructure reproducible.

**Build:** Create a pipeline that tests and builds your app; use Terraform to provision a small disposable cloud environment.

**Move on when:** You can explain a pipeline run, safely store secrets, review a Terraform plan, and destroy a lab you created.

## 6. Kubernetes

**Study:** Pods, Deployments, Services, Ingress, ConfigMaps, Secrets, probes, requests/limits, and basic `kubectl` troubleshooting.

**Goal:** Deploy and inspect a containerized application on a cluster.

**Build:** Complete Project 7: deploy the API with a Deployment, Service, Ingress, ConfigMap, Secret, probes, and resource settings.

**Move on when:** You can use `kubectl get`, `describe`, and `logs` to find a basic deployment/configuration failure.

## 7. Operations — Monitoring

**Study:** Metrics, logs, traces, Prometheus, Grafana, and alerts. Continue the security practices introduced above.

**Goal:** See whether the app is healthy and use evidence during troubleshooting.

**Build:** Complete Project 8: create a dashboard for resource and API metrics, one actionable alert, and move configuration secrets out of code.

**Move on when:** You can explain metrics versus logs versus traces, find a failure in logs/dashboard data, and describe how you protect credentials.

## 8. Projects

**Study:** Your own work. Revisit weak areas while completing Projects 1–8.

**Goal:** Turn separate tools into evidence that you can build, deploy, automate, and troubleshoot a small system.

**Build:** A portfolio README for your final project: architecture diagram, local/cloud setup, CI/CD route, logs/metrics, security notes, cost cleanup, and one failure you fixed.

**Move on when:** You can give a short, honest walkthrough of the project without reading from notes.

## 9. Start Applying

Start applying for junior Cloud Engineer, DevOps Engineer, and Cloud Operations roles after you can demonstrate Projects 3–6, meet most of the [job-ready checklist](job-ready-checklist.md), and meet this minimum Kubernetes/operations level: deploy a simple app, inspect it with `kubectl get`, `describe`, and `logs`, understand a basic dashboard/alert, and handle secrets safely. You should be able to explain your application path, cloud setup, Docker workflow, Terraform plan/state, CI/CD pipeline, logs, and one troubleshooting story.

You do not need Kubernetes mastery, cluster administration, advanced SRE, every optional project, certifications, or advanced system design. Continue Projects 7–8 while you apply.
