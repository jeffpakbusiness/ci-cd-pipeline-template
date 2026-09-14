# Product Brief: CI/CD Pipeline Template

## Problem
Developers starting a new Python project often skip automated testing and style
checks early on, or spend time manually wiring up CI from scratch for every new
repo. Bugs and style drift creep in before anyone notices.

## Solution
A ready-to-use GitHub Actions workflow (`.github/workflows/ci.yml`) that any
Python project can copy in. It automatically runs pytest and flake8 on every
push and pull request to `main`, catching failures before they merge.

## Target Users ("Builders")
Individual developers and small teams who want consistent code quality without
hand-configuring CI/CD for every new project.

## Success Metrics
- Time to add CI to a new repo: copy one file instead of configuring a pipeline
  from scratch
- Share of pushes/PRs where lint or test failures are caught by CI before merge,
  rather than after

## Out of Scope (for this version)
- Deployment/CD steps (this template covers CI only)
- Language support beyond Python
- Multi-OS test matrix
