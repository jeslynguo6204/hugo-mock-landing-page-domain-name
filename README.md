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

✅ Recent Update: Scraping Latest Multimedia Story
📌 Changes Made
Updated Target Page:

Previously, the scraper extracted the main front-page headline from the homepage.
Now, it navigates to https://www.thedp.com/multimedia to find the most recent photo gallery or video story.
Modified Scraper Logic:

The scraper searches for a <div> with the class "featured-media", which contains the latest multimedia article.
Inside this section, it extracts the <a> tag with the headline text.
Added Robustness & Compliance:

Introduced a User-Agent header to prevent blocks by the website.
Ensured robots.txt compliance by implementing a 10-second delay between requests.

This project is part of **CIS 3500 - Software Engineering** at the University of Pennsylvania.



