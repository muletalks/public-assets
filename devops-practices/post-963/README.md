# Mastering DevOps: Streamlining MuleSoft Projects with Reusable GitHub Actions

Welcome to the assets repository for our blog post on streamlining MuleSoft projects with reusable GitHub Actions. This repository contains a simple MuleSoft application and a globally reusable GitHub Actions workflow.

## Assets Overview

1. **Simple Hello World Mule Application**: A basic MuleSoft application that demonstrates the use of a GitHub Actions workflow for deployment to a DEV environment.
2. **Globally Reusable Workflow**: A workflow designed to be reusable across multiple MuleSoft projects, promoting the DRY (Don't Repeat Yourself) principle.

## Usage

### Simple Hello World Mule Application

This application comes with a predefined GitHub Actions workflow located at `.github/workflows/dev-workflow.yml`. This workflow triggers on pushes to the `develop` branch and allows manual dispatch with input parameters for worker type and count.

### Globally Reusable Workflow

Located at `.github/workflows/dev-reusable-workflow.yml`, this workflow is designed to be reusable across multiple MuleSoft projects. It abstracts the core logic of deploying a MuleSoft application to a DEV environment, allowing you to maintain a single source of truth for your deployment logic.

To use this workflow in another repository, reference it in your workflow file using the `uses` keyword:

```yaml
uses: muletalks/reusable-workflows/.github/workflows/dev-reusable-workflow.yml@master
```

## Prerequisites

- Ensure you have the following secrets set up in your GitHub repository:
  - `MULETALKS_DEPLOYER_PREPROD_CLIENT_ID`
  - `MULETALKS_DEPLOYER_PREPROD_CLIEN_SECRET`
  - `MULETALKS_ANYPOINT_PLATFORM_CLIENT_ID`
  - `MULETALKS_ANYPOINT_PLATFORM_CLIENT_SECRET`

These secrets are essential for the deployment process to the CloudHub DEV environment.

## Feedback and Contributions

Your feedback and contributions enrich our repository. Should you face any challenges or have innovative suggestions, don't hesitate to [open an issue](https://github.com/muletalks/public-assets/issues/new). Alternatively, you can [contact us directly on our website](https://muletalks.dev/contact/).


Happy coding and may the force of streamlined DevOps be with you!
