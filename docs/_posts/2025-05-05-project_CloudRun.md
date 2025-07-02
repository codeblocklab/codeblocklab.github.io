---
layout: post
title: Automated Infrastructure Deployment for Cloud Run with Cloud Armor and Secrets Manager
categories: gcp
tags: gcp
project: 1
---

GCP serverless provisioning with Cloud Run, Cloud Armor, Secret Manager, and Terraform automation.

<!--more-->

We provide infrastructure provisioning and deployment automation in GCP for serverless workloads using Cloud Run. Our solution includes secure traffic protection with Cloud Armor, centralized secret management with Secret Manager, and Infrastructure as Code using Terraform for repeatable, compliant environments.

## Scope of the Solution

### Cloud Run Deployment

- Automated provisioning of Cloud Run services with Terraform.  
- Configuration of service revisions, concurrency, memory, and autoscaling.  
- Setup of custom domains, HTTPS, and traffic splitting between revisions (for blue/green or canary deployments).

### Cloud Armor Integration

- Configuration of Cloud Armor security policies to protect Cloud Run from common threats (e.g., SQL injection, XSS, DDoS).  
- Implementation of IP allow/deny lists, rate limiting, and geo-based access control.  
- Logging and alerting on denied requests for audit and incident response.

### Secret Management

- Secure injection of secrets from GCP Secret Manager into Cloud Run services as environment variables.  
- Versioned secret access with IAM-controlled policies and audit logs.  
- Optional encryption key management via Cloud KMS for enhanced security.

### Infrastructure as Code & Automation

- Use of Terraform (optionally Terragrunt) to manage services, IAM roles, secrets, and policies.  
- Environment-specific configuration (dev/staging/prod) with reusable modules.  
- CI/CD pipeline integration for infrastructure promotion (GitHub Actions, GitLab CI, Cloud Build).

## Benefits

- Secure and scalable serverless workloads deployed with IaC best practices  
- Centralized secret storage and strict IAM control  
- Layered security with WAF rules and access policies via Cloud Armor  
- Fully automated provisioning and deployment process with version control

## Technologies Used

- Google Cloud Run  
- Google Cloud Armor  
- Google Secret Manager  
- Google Cloud IAM  
- Terraform / Terragrunt  
- GitHub Actions / GitLab CI / Cloud Build  
- Cloud KMS (optional)
