# Platform Applications
A GitOps-driven Kubernetes application deployment repository for managing platform workloads across environments using ArgoCD, Helm, and Kubernetes manifests.
## Overview
platform-applications contains the application layer for the platform infrastructure.

This repository is responsible for:

- Managing Kubernetes application deployments
- Defining ArgoCD applications
- Organizing workloads by environment
- Managing Helm charts and Kubernetes manifests
- Enabling GitOps-based continuous delivery
- Supporting multi-environment deployments (dev, staging, production)

The infrastructure layer is managed separately in the platform-infrastructure repository.
# Tech Stack
This repository uses:

- Kubernetes
- ArgoCD
- Helm
- GitHub Actions
- Docker
- AWS EKS
- Prometheus & Grafana
# GitOps Workflow
The deployment workflow follows GitOps principles:

1. Developer pushes code changes
2. CI pipeline builds and publishes Docker images
3. Image tags are updated in this repository
4. ArgoCD detects repository changes
5. Kubernetes cluster syncs automatically
6. Application rollout is performed in EKS
# Environments
## Development

Used for:

- Feature validation
- Integration testing
- Internal QA
## Staging

Used for:

- Pre-production testing
- Release validation
- Performance checks
## Production

Used for:

- Live customer workloads
- High availability deployments
- Monitored production releases
# Prerequisites
Before using this repository, ensure you have:

- Kubernetes cluster access
- kubectl installed
- Helm installed
- ArgoCD configured
- AWS CLI configured
- Docker installed

  
