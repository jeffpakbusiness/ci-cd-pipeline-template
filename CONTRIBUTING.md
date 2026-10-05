# Contributing

Thank you for considering a change to this template.

## Local Setup

1. Fork and clone the repository.
2. Install the dependencies the pipeline uses:

   ```
   pip install pytest pytest-cov flake8
   ```

3. Run the same checks CI runs before opening a pull request:

   ```
   flake8 . --max-line-length=100
   pytest --cov=. --cov-report=term-missing
   ```

## Opening a Pull Request

1. Create a branch for your change.
2. Confirm that both flake8 and pytest pass locally.
3. Open a pull request against main. The CI workflow runs the same checks automatically and must pass before merging.

## What to Contribute

This repository is intentionally small; it is a template, not a full application. Improvements to the workflow file itself, clearer documentation, or a more realistic example are more valuable than expanding the sample code into something larger.
