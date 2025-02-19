# hugo-mock-landing-page-autodeployed

# Hugo Mock Landing Page - Auto Deployed

This repository is a **Hugo static website** that is automatically deployed to GitHub Pages using **GitHub Actions**.

## 🌟 Continuous Deployment Setup

### 📌 How It Works
- Every time a change is pushed to the **main branch**, GitHub Actions runs the workflow.
- The workflow:
  1. Checks out the latest code.
  2. Installs Hugo.
  3. Builds the static site.
  4. Deploys the site to GitHub Pages.

### 🔧 GitHub Actions Workflow
The automation is handled by the following workflow file: .github/workflows/gh-pages-deployment.yaml

### 📝 Additional Notes
- The base URL in `config.toml` is set to match the deployed URL.
- Hugo version **0.144.1** is used in the workflow.
- GitHub Pages settings must have `gh-pages` as the deployment branch.

This project is part of **CIS 3500 - Software Engineering** at the University of Pennsylvania.



