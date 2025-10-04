# try-copier-uv

[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/atloo1/try-copier-uv/ci.yaml)](https://github.com/atloo1/try-copier-uv/actions/workflows/ci.yaml?query=branch%3Amain)
[![Dynamic TOML Badge](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fatloo1%2Ftry-copier-uv%2Frefs%2Fheads%2Fmain%2Fpyproject.toml&query=%24.tool.poetry.dependencies.python&label=python)](https://github.com/atloo1/try-copier-uv/blob/main/pyproject.toml)
[![Dynamic TOML Badge](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fatloo1%2Ftry-copier-uv%2Frefs%2Fheads%2Fmain%2Fpyproject.toml&query=%24.tool.poetry.version&label=version)](https://github.com/atloo1/try-copier-uv/blob/main/pyproject.toml)
[![GitHub License](https://img.shields.io/github/license/atloo1/try-copier-uv)](https://github.com/atloo1/try-copier-uv/blob/main/LICENSE)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/atloo1/try-copier-uv)

[![Copier](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/copier-org/copier/master/img/badge/badge-grayscale-inverted-border-orange.json)](https://github.com/copier-org/copier)
[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
[![Renovate enabled](https://img.shields.io/badge/renovate-enabled-brightgreen.svg)](https://renovatebot.com/)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
[![uv](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/uv/main/assets/badge/v0.json)](https://github.com/astral-sh/uv)

Python project template managed by [copier](https://copier.readthedocs.io/en/stable/), supporting automated [1] package management via [uv](https://docs.astral.sh/uv), [2] dependency updates via [Renovate](https://github.com/renovatebot/renovate?tab=readme-ov-file#what-is-the-mend-renovate-cli), [3] testing via [pytest](https://github.com/pytest-dev/pytest), [4] linting via [mypy](https://github.com/python/mypy) & [ruff](https://github.com/astral-sh/ruff), & [5] CI/CD via [GitHub Actions](https://docs.github.com/en/actions/about-github-actions/understanding-github-actions#workflows) & [pre-commit](https://github.com/pre-commit/pre-commit)

## prerequisites

- [uv](https://docs.astral.sh/uv/getting-started/installation/)

```
uv tool install copier --with copier-template-extensions
```

## use

### template from this repo

#### remote

```
uv run copier copy https://github.com/atloo1/try-copier-uv/ path/to/destination --trust
```

#### local

```
uv run copier copy path/to/this/repo path/to/destination --trust
```

### update templated repo

```
uv run copier update
```

## develop

### first time setup

```
git clone https://github.com/atloo1/try-copier-uv.git
cd try-copier-uv/
uv run pre-commit install
```
