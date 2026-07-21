# docswarm

`docswarm` is a Python package scaffold published to PyPI. The repository currently ships the packaging, build, and trusted-publishing plumbing; the package module itself is intentionally minimal while the public API is worked out.

## Status

Early scaffold. The `docswarm` distribution builds and publishes, but exposes only a `__version__` attribute for now. Treat the `0.1.x` line as a placeholder until a real module surface lands.

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

## License

Licensed under the [MIT License](LICENSE).
