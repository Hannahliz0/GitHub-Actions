# GitHub-Actions
# CI/CD Pipeline Setup with GitHub Actions

This project implements a CI/CD pipeline using **GitHub Actions** for a full-stack application. The goal is to ensure quality checks are performed automatically and deployments occur seamlessly when the code is merged into the `main` branch.

---

## Features

1. **Continuous Integration (CI):**
   - Automatically triggers Cypress component tests when a Pull Request is made to the `develop` branch.
   - Displays test results on GitHub Actions for validation before merging.

2. **Continuous Deployment (CD):**
   - Automatically deploys the application to Render when code is merged from the `develop` branch to the `main` branch.

---

## Workflow Overview

### 1. **Branching Strategy:**
   - **Develop Branch:** For integrating new features. All feature updates must go through this branch via Pull Requests.
   - **Main Branch:** For production-ready code. Code is automatically deployed upon merging into this branch.

### 2. **GitHub Actions Workflows:**

#### Workflow 1: CI - Component Testing
   - **Trigger:** Pull Request to `develop` branch.
   - **Action:**
     1. Runs Cypress component tests to ensure code quality.
     2. Test results are displayed in the GitHub Actions tab.
   - **Outcome:** If tests pass, the code is approved for merging.

#### Workflow 2: CD - Automatic Deployment
   - **Trigger:** Code merge from `develop` to `main` branch.
   - **Action:**
     1. Automatically deploys the application to Render.
     2. Confirms successful deployment in the GitHub Actions tab.
   - **Outcome:** Updates are live on production.

---

## Collaborators

- Hannah Schmidt, Student
- Sabrin, Student
