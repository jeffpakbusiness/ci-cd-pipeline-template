# ci-cd-pipeline-template

A ready-to-use GitHub Actions workflow that runs linting, tests, and a
coverage report on every push and pull request to a Python project. Copy
one file in, and CI is running within minutes.

## What It Does

On every push or pull request to `main`, the workflow:

1. Checks out the code
2. Sets up Python 3.11
3. Installs `pytest`, `pytest-cov`, and `flake8`
4. Runs `flake8` (style and lint checks)
5. Runs `pytest` with coverage (tests, plus a coverage report printed in the Actions log)

If either step fails, the run is marked failed and shows up as a red X on
the commit or pull request, so problems are caught before they merge
rather than after.

## How to Use This in Your Own Project

1. Copy `.github/workflows/ci.yml` from this repository into the same path in yours.
2. Confirm your test files are discoverable by `pytest` (for example, named
   `test_*.py`) and that your source files pass `flake8` with a
   `--max-line-length=100` setting (adjust the flag in the workflow if you
   use a different limit).
3. Push your changes, then check the "Actions" tab on GitHub to watch the
   workflow run.

## Example Project in This Repository

`calculator.py` and `test_calculator.py` are a minimal example the
pipeline runs against, included to demonstrate that the workflow functions
end to end. The example code is not the point; the workflow file is.

## Contributing

See `CONTRIBUTING.md` for local setup instructions and how to open a pull
request. Issue and pull request templates are included under `.github/` so
contributions follow a consistent format.

## Project Management

See `PRODUCT_BRIEF.md` for the problem this project solves, its target
users, and its success metrics.
