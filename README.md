# Welcome
This is me taking notes on GitHub while learning `Helm`. I will probably be going to need this document when I forget how it works. If you find something useful, be my guest. I will try to update this whenever I study.

## Intro
- Helm the best way to find, share and use software built for **Kubernetes**
- Helm is a **package manager** for Kubernetes
- It helps you to manage Kubernetes applications
- Helm Charts help you define, install, and upgrade even the most complex Kubernetes application
- Helm is maintained by the **CNCF - The Cloud Native Computing Foundation** (together with Kubernetes, fluentd, linkerd etc.)

## Setup
- Download helm client
- Run helm init

## Common Commands
```
# Install tiller on the cluster
helm init

# Remove tiller from the cluster
helm reset

# Install a helm chart
helm install

# Search for a chart
helm search

# List releases (installed charts)
helm list

# Upgrade a release
helm upgrade

# Rollback a release to previous version
helm rollback
```
