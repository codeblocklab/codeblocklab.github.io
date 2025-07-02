---
layout: post
title: Static Website Hosting on AWS with S3, CloudFront, HTTPS, and ACM Certificates
categories: aws
tags: aws
project: 1
---

Static website hosting on AWS with S3, CloudFront, and ACM for secure, global HTTPS delivery

<!--more-->

We provide a secure, scalable, and cost-effective static website hosting solution entirely on AWS. The architecture uses **Amazon S3** for storing and serving frontend assets, **CloudFront** for global content delivery, and **AWS Certificate Manager (ACM)** for managing HTTPS certificates.

## Scope of the Solution

### Amazon S3 Configuration

- Static website hosting using S3 buckets with public or restricted (CloudFront-only) access.  
- Bucket versioning, custom error documents, and SPA routing support.  
- Fine-grained bucket policies and optional encryption at rest (SSE-S3 or SSE-KMS).

### AWS CloudFront Integration

- Global CDN distribution with caching, compression, and origin protection.  
- Integration with S3 using Origin Access Control (OAC) or Origin Access Identity (OAI).  
- Caching strategies with cache behaviors and TTL configurations.  
- Optional WAF integration for traffic filtering and security rules.

### HTTPS with AWS Certificate Manager (ACM)

- Automated SSL/TLS certificate provisioning for custom domains via ACM.  
- DNS validation using Route 53 or external DNS providers.  
- HTTPS enforced for all users via CloudFront.  
- Auto-renewal of certificates without manual intervention.

### Automation with Terraform

- Infrastructure provisioning using modular Terraform code: S3, CloudFront, ACM, Route 53.  
- Optional use of Terragrunt for environment-specific overrides.  
- CI/CD pipelines to deploy frontend assets to S3 (e.g., GitHub Actions or CodePipeline).

### Monitoring & Security

- Access logging enabled on S3 and CloudFront.  
- CloudWatch metrics and alarms for traffic, errors, and performance.  
- IAM roles and least-privilege access for deployment pipelines and certificate management.

## Benefits

- Fully serverless and cost-efficient static site hosting on AWS  
- Global availability and performance via CloudFront  
- HTTPS and custom domain support with automatic certificate management  
- Easily repeatable and auditable infrastructure using Terraform

## Technologies Used

- AWS S3  
- AWS CloudFront  
- AWS Certificate Manager (ACM)  
- AWS Route 53 (optional)  
- AWS WAF (optional)  
- Terraform / Terragrunt  
- GitHub Actions / AWS CodePipeline  
- AWS CloudWatch
