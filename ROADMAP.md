# Main roadmap

Move forward when you can explain the previous stage and finish its small lab. Do not wait for perfection before projects or applications.

```mermaid
flowchart TD
    A[Computer Basics] --> B[Networking]
    B --> C[Linux]
    C --> D[Git & GitHub]
    D --> E[Bash + Python/Go]
    E --> P[Required prerequisite project<br/>Small API + PostgreSQL]
    P --> G[Docker]
    G --> F[One Cloud Provider]
    F --> H[CI/CD + Terraform]
    H --> J[Kubernetes]
    J --> K[Monitoring & Observability]
    K --> M[Projects]
    M --> N[Start Applying]

    S[Security throughout<br/>least privilege · secrets · TLS · updates] -.-> G
    S -.-> F
    S -.-> H
    S -.-> J

    K -. Learn later .-> O[Learn Later<br/>SRE<br/>Platform Engineering<br/>GitOps<br/>Service Mesh<br/>Multi-cloud<br/>Advanced Cloud Security]

    classDef main fill:#eff6ff,stroke:#1d4ed8,color:#0f172a,stroke-width:1px;
    classDef final fill:#0f3b75,stroke:#0f3b75,color:#ffffff,stroke-width:1px;
    classDef later fill:#f8fafc,stroke:#64748b,color:#334155,stroke-width:1px;
    class A,B,C,D,E,P,G,F,H,J,K,M main;
    class N final;
    class O,S later;
```

## Milestones

1. **Foundation:** finish computer, networking, Linux, Git, and scripting; run Project 1.
2. **Required application context:** after scripting, use [prerequisites.md](prerequisites.md) to build Project 2. Learn what you deploy, without becoming a backend developer or DBA.
3. **Delivery:** containerize the application first, deploy that Dockerized application to one cloud, automate it, and provision it with Terraform (Projects 3–6).
4. **Operations:** deploy the same app to Kubernetes and observe it (Projects 7–8).

Start applying once you can confidently demo Projects 3–6 **and** meet the minimum Kubernetes/operations baseline: deploy a simple app, inspect it with `kubectl get`, `describe`, and `logs`, read a basic dashboard, and protect secrets. This is working knowledge, not Kubernetes mastery. Projects 7–8 make the portfolio stronger while you apply. See [HOW-TO-FOLLOW-THE-ROADMAP.md](HOW-TO-FOLLOW-THE-ROADMAP.md) for stage-by-stage readiness checks.

## Learn Later

These are valuable, but not first-job requirements: advanced OS internals; distributed systems; multi-cloud; service mesh; Kubernetes Operators; eBPF; advanced GitOps; Platform Engineering; Internal Developer Platforms; advanced SRE and error budgets; advanced cloud security; FinOps; BGP; and complex microservices architecture.
