# docswarm

Minimal Python package scaffold for publishing `docswarm` to PyPI.

## Local development

```bash
python -m venv .venv
. .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -e .
```

## Build distributions

```bash
python -m pip install --upgrade pip
python -m pip install build
python -m build
```

## Publish workflow

Publishing is configured in `.github/workflows/workflow.yml` using PyPI Trusted Publishing.
Create a git tag like `v0.1.0` and push it to trigger publication.