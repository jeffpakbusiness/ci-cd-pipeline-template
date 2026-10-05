# Product Brief: CI/CD Pipeline Template

## Problem
Developers starting a new Python project often skip automated testing and
style checks early on, or spend time manually configuring CI/CD for every
new repository. As a result, bugs and style issues go unnoticed until
later in development.

## Solution
A ready-to-use GitHub Actions workflow (`.github/workflows/ci.yml`) that
any Python project can copy in directly. It runs pytest and flake8
automatically on every push and pull request to `main`, so failures are
caught before code is merged.

## Target Users ("Builders")
Individual developers and small teams who want consistent code quality
without configuring CI/CD from scratch for every new project.

## Success Metrics
- Time to add CI to a new repository: copying one file rather than
  building a pipeline from scratch
- Frequency with which lint or test failures are caught by CI before
  merge, rather than after

## Out of Scope (for this version)
- Deployment/CD steps (this template covers CI only)
- Language support beyond Python
- Multi-OS test matrix
