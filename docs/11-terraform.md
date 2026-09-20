# 11 — Terraform

## Why it matters

Infrastructure as Code makes infrastructure repeatable, reviewable, and easier to recover.

## What to learn

Learn declarative configuration, provider, resource, variable, output, data source, module, `terraform init`, `plan`, `apply`, `destroy`, and state. State maps configuration to real infrastructure; protect it and use remote state for shared work.

## Practical examples

Always read a plan before apply. Keep state out of Git. Use `destroy` deliberately to remove a disposable lab after confirming its target.

## Short lab (30 minutes)

Write a small configuration that creates an S3 bucket or equivalent safe resource. Run `fmt`, `init`, `validate`, `plan`, `apply`, inspect output, then `destroy` it. First supply an invalid or missing variable, read the validation/plan error, fix it, and explain the change.

## Common mistakes

Skipping plans, committing state/secrets, manually changing Terraform-managed resources, or using one state file for unrelated systems.

## When to move on

- [ ] I can explain declarative IaC, provider, resource, variable, output, and state.
- [ ] I can review a plan, apply a small lab, and clean it up safely.

## Trusted resources

[Terraform introduction](https://developer.hashicorp.com/terraform/intro) · [Terraform core workflow](https://developer.hashicorp.com/terraform/intro/core-workflow) · [Terraform state](https://developer.hashicorp.com/terraform/language/state)
