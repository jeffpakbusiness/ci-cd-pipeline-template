# Contributing

Thanks for considering a change to this template.

## Local setup

1. Fork and clone the repo.
2. Install the dependencies the pipeline uses:

   ```
   pip install pytest pytest-cov flake8
   ```

3. Run the same checks CI runs before you open a pull request:

   ```
   flake8 . --max-line-length=100
   pytest --cov=. --cov-report=term-missing
   ```

## Opening a pull request

1. Create a branch for your change.
2. Make sure flake8 and pytest both pass locally.
3. Open a pull request against main. The CI workflow runs the same checks automatically and must pass before merging.

## What to contribute

This repo is intentionally small, it's a template, not a full application. Improvements to the workflow file itself, clearer documentation, or a slightly more realistic example are more useful than expanding the sample code into something bigger.
