# Project 4 — Cloud deployment

## Goal

Deploy the application on one cloud provider (AWS examples: VPC, EC2, RDS, S3, IAM, ALB).

## Build

- Create VPC with public and private subnets across appropriate availability zones.
- Place an internet-facing load balancer in public subnets and app EC2 in private networking where practical.
- Put RDS PostgreSQL in private subnets; allow its port only from the app security group.
- Use S3 for a harmless uploaded/static object example.
- Give EC2 an IAM role with only required S3 access.
- Send logs/metrics to CloudWatch, add cost budget/tagging, and document cleanup.

## Acceptance test

A browser reaches the app through the load balancer; app reaches RDS; database is not publicly reachable. Record a simple architecture diagram and cost cleanup steps.

## Stretch

Add a second app instance and demonstrate load balancer health checks.
