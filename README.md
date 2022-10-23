# Welcome
This is me taking notes on GitHub while learning `Helm`. I will probably be going to need this document when I forget how it works. If you find something useful, be my guest. I will try to update this whenever I study.

## Intro
- Helm the best way to find, share and use software built for **Kubernetes**
- Helm is a **package manager** for Kubernetes
- It helps you to manage Kubernetes applications
- Helm Charts help you define, install, and upgrade even the most complex Kubernetes application
- Helm is maintained by the **CNCF - The Cloud Native Computing Foundation** (together with Kubernetes, fluentd, linkerd etc.)

## Setup
You can install `Helm` with the following [Helm Installation Document](https://helm.sh/docs/intro/install/) 

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

## Creating Custom Helm Charts
It is the recommended way to deploy custom applications on Kubernetes. Packaging the app, allows us deploy the app in 1 command instead of using `kubectl create/apply`.

To create the files necessary for a new chart, you can enter the command: `helm create mychart`. This will create a path named `mychart` and insert **yaml** files under the folder like shown below:

- mychart/
  - Chart.yaml
  - values.yaml
  - templates/
    - deployment.yaml
    - service.yaml

