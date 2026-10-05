# Product Brief: CI/CD Pipeline Template

## Problem
When people start a new Python project, they usually skip automated testing
and style checks early on, or they waste time wiring up CI from scratch every
time. Bugs and style issues creep in before anyone catches them.

## Solution
A ready-to-use GitHub Actions workflow (`.github/workflows/ci.yml`) that any
Python project can copy in. It runs pytest and flake8 automatically on every
push and pull request to `main`, so failures get caught before they merge.

## Target Users ("Builders")
Individual developers and small teams who want consistent code quality
without hand-configuring CI/CD every time they start something new.

## Success Metrics
- Time to add CI to a new repo: copy one file instead of building a pipeline
  from scratch
- How often lint or test failures get caught by CI before merge, instead of
  after

## Out of Scope (for this version)
- Deployment/CD steps (this template is CI only)
- Language support beyond Python
- Multi-OS test matrix
