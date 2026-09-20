# Project 5 — Terraform

## Goal

Rebuild Project 4 reproducibly from Terraform.

## Build

- Create network/VPC, subnets/routes, VM/EC2, security groups, load balancer, and database.
- Use provider version constraints, variables, outputs, tags, and a small local module if helpful.
- Configure an appropriate protected remote backend before collaboration.
- Run `fmt`, `validate`, `plan`, and carefully reviewed `apply`.
- Keep state out of Git and document every cost-bearing resource.

## Acceptance test

Destroy a disposable environment and recreate it from clean code. Save a redacted plan summary and document how state is protected.

## Stretch

Use separate variables for dev and production-like environments; do not use workspaces as a substitute for thoughtful environment design.
