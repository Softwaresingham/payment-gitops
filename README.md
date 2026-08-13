# Payment Service GitOps Repository

GitOps manifests for the Payment Service.

## Environments

- DEV
- QA
- PRE-PROD
- PROD

## Deployment Model

```text
ECR
  |
  v
Argo Image Updater
  |
  v
DEV
  |
  v
Kargo
  |
  +--> QA
  |
  +--> PRE-PROD
  |
  +--> PROD
