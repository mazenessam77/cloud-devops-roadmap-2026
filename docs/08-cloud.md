# 08 — Cloud

## Why it matters

Cloud is programmable rented infrastructure. Choose one provider first; AWS names are used here, but the concepts transfer.

## What to learn

Learn regions/AZs, shared responsibility, IAM users/roles/policies and least privilege, VPCs, subnets, routes, internet gateway, NAT, security groups, VMs, object/block storage, load balancers, managed databases, DNS, logs/metrics, secrets, and serverless basics. AWS examples: EC2, S3, VPC, IAM, RDS, Route 53, CloudWatch, Lambda.

## Practical examples

Use an IAM role instead of long-lived keys. Keep databases private and permit their port only from the application security group.

## Short lab (30 minutes)

In a sandbox/free-tier-aware account, create a VPC, EC2 instance, restrictive security group, and S3 bucket. Tag resources, set a budget alert, then record cleanup steps.

## Common mistakes

Using root credentials daily, public databases, wide-open SSH, and forgetting cost cleanup.

## When to move on

- [ ] I can explain a VPC, public/private subnet, IAM role, EC2, S3, RDS, and load balancer.
- [ ] I can deploy a small VM safely and find its logs.

## Trusted resources

[AWS Skill Builder](https://skillbuilder.aws/) · [AWS documentation](https://docs.aws.amazon.com/) · [AWS IAM best practices](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)
