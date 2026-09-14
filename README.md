# ci-cd-pipeline-template

A ready-to-use GitHub Actions workflow that runs linting and tests on every
push and pull request to a Python project. Copy one file in, get CI running
in a couple of minutes.

## What it does

On every push or pull request to `main`, the workflow:

1. Checks out your code
2. Sets up Python 3.11
3. Installs `pytest` and `flake8`
4. Runs `flake8` (style/lint checks)
5. Runs `pytest` (tests)

If either step fails, the run is marked failed and shows up as a red X on the
commit/PR, so problems get caught before they merge instead of after.

## How to use this in your own project

1. Copy `.github/workflows/ci.yml` from this repo into the same path in yours.
2. Make sure your test files are discoverable by `pytest` (e.g. named
   `test_*.py`) and your source files pass `flake8` with a
   `--max-line-length=100` (adjust the flag in the workflow if you use a
   different limit).
3. Push. Check the "Actions" tab on GitHub to watch it run.

## Example project in this repo

`calculator.py` and `test_calculator.py` are a minimal example the pipeline
runs against, just to prove the workflow works end to end. They're not the
point — the workflow file is.

## Project management

See `PRODUCT_BRIEF.md` for the problem this solves, target users, and
success metrics.
