---
layout: page
title: Skills
permalink: /tech
---


{% for sk in site.skills %}
  <h2>{{ sk.name }}</h2>
  <p>{{ sk.content | markdownify }}</p>
{% endfor %}


## Cloud Platforms & Administration
- AWS
- GCP
- Azure
- Proxmox
- OpenStack

## Infrastructure as Code & Orchestration
- Terraform
- Terragrunt
- Ansible
- SaltStack
- Puppet
- Docker
- containerd
- Kubernetes (GKE, OpenShift)
- Kustomize
- ArgoCD

## CI/CD & GitOps
- GitHub Actions
- GitLab CI
- Argo Workflows
- Argo Events
- Atlantis (Terraform GitOps model)

## Scripting & Programming
- Bash scripting
- Python

## Systems & User Management
- Linux server administration
- Windows server administration
- Okta (Identity Provider)
- JumpCloud
- Azure AD / Entra ID
- Keycloak

## Identity, Access & Security
- IAM (Cloud provider level)
- Privileged Access Management (PAM)
- SSO (Single Sign-On) integration
- VPN (IPSEC, WireGuard)
- TLS / Certificate management
- Employee lifecycle workflows
- Security hardening practices

## Monitoring, Logging & SIEM
- Prometheus
- Grafana
- Zabbix
- Datadog
- New Relic
- Graylog
- Splunk
- Sumo Logic
- CrowdStrike Falcon (SIEM)

## Security & Compliance
- ISO 27001
- SOC 2
- PCI-DSS
- NIST
- CIS Benchmarks
- Security auditing & compliance reporting

## Cloud FinOps & Operations
- Cloud cost optimization
- Monitoring & alerting
- Infrastructure automation
- Resource provisioning & cleanup workflows
