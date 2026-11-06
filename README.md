# Tarfi Cloud

### Infrastructure Automation & Application Delivery Platform

Tarfi Cloud is a hands-on cloud engineering project focused on designing,
provisioning, securing, automating, deploying, and monitoring application
infrastructure on AWS.

The project aims to demonstrate practical skills in cloud infrastructure,
Linux administration, Infrastructure as Code, containerization, CI/CD,
networking, security, and observability.

## Project Objectives

- Provision AWS infrastructure using Terraform.
- Design VPC networking with appropriate public and private subnets.
- Deploy a containerized application using Docker.
- Configure Nginx as a reverse proxy.
- Implement automated CI/CD using GitHub Actions.
- Authenticate GitHub Actions to AWS using OpenID Connect (OIDC).
- Configure DNS and HTTPS using Cloudflare.
- Monitor infrastructure and application health using Prometheus,
  Grafana, and Amazon CloudWatch.
- Implement security controls, backups, and recovery procedures.

## Planned Technology Stack

| Category | Technology |
|---|---|
| Cloud Provider | AWS |
| Infrastructure as Code | Terraform |
| Operating System | Ubuntu Linux |
| Application | Python, FastAPI |
| Containerization | Docker |
| Reverse Proxy | Nginx |
| CI/CD | GitHub Actions |
| Authentication | AWS IAM, OIDC |
| DNS and HTTPS | Cloudflare |
| Monitoring | Prometheus, Grafana |
| Logging | Amazon CloudWatch |
| Database | PostgreSQL |

## Architecture Overview

The planned platform will use AWS VPC networking to isolate application
and data components.

The application will run on an Ubuntu EC2 instance using Docker.
Nginx will handle reverse proxy traffic, while PostgreSQL will provide
persistent data storage.

Terraform will provision the infrastructure, and GitHub Actions will
automate application testing, image building, and deployment.

Cloudflare will manage DNS and provide the public-facing proxy and
HTTPS configuration.

Monitoring and logging will provide visibility into infrastructure
and application health.

The architecture will be implemented incrementally, with optional
services such as Amazon RDS and CloudFront evaluated against actual
requirements and cost.

## Repository Structure

```text
tarfi-cloud/
├── .github/
│   └── workflows/
├── app/
├── docker/
├── docs/
├── monitoring/
│   ├── grafana/
│   └── prometheus/
├── nginx/
├── scripts/
└── terraform/
    ├── environments/
    │   └── dev/
    └── modules/


Implementation Roadmap
- [ ] Development environment and project foundation
- [ ] AWS networking and infrastructure
- [ ] Linux server configuration and security hardening
- [ ] FastAPI application and Docker deployment
- [ ] Terraform infrastructure automation
- [ ] GitHub Actions CI/CD with AWS OIDC
- [ ] Cloudflare DNS and HTTPS
- [ ] Prometheus, Grafana, and CloudWatch monitoring
- [ ] Backup, recovery, and security testing
- [ ] Architecture documentation and demonstration
Project Documentation
- Architecture: docs/architecture.md
- Deployment: docs/deployment.md
- Troubleshooting: docs/troubleshooting.md
Project Status
In development.

This repository documents the design and implementation of Tarfi Cloud.
The roadmap and architecture describe planned functionality; individual
features will be marked complete only after implementation and testing.

Built as a practical cloud and DevOps engineering portfolio project.
