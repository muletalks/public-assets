# Mastering DevOps: Streamlining MuleSoft Projects with Reusable GitHub Actions

Welcome to the assets repository for our comprehensive guide on centralizing MuleSoft projects using GitHub Actions. This repository houses both a rudimentary MuleSoft application and a globally reusable GitHub Actions workflow, serving as practical references for the concepts discussed in the blog post.

## Assets Overview

1. **Hello World Mule Application**: A foundational MuleSoft application that showcases the integration of a GitHub Actions workflow for deployment to a DEV environment.
2. **Globally Reusable Workflow**: A simplified reusable workflow intended for universal applicability across diverse MuleSoft projects, championing the DRY (Don't Repeat Yourself) principle.

## Usage

### Hello World Mule Application

This application is equipped with a pre-configured GitHub Actions workflow located at `.github/workflows/dev-workflow.yml`. This workflow triggers on pushes to the `develop` branch and supports manual dispatch, complete with input parameters to specify worker type and count.

### Globally Reusable Workflow

Located at `.github/workflows/dev-reusable-workflow.yml`, this workflow is architected for broad reusability across a spectrum of MuleSoft projects. It encapsulates the quintessential logic for deploying a MuleSoft application to a DEV environment, ensuring you have a consistent and centralized deployment logic.

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
