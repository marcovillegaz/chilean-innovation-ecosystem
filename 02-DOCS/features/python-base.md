# Feature: Python base (venv + src)

**Branch:** `feat/python-base` · **Lane:** FTD · **Date:** 2026-10-02

## Intent
Give the project an isolated Python environment and an installable `src/` package to build the OOP stakeholder model on.

## Scope
In: `.venv`, `pyproject.toml`, `src/stakeholders_map/`, smoke test, README setup, Python entries in `.gitignore`.
Out: domain classes, graph libraries, app framework, data sources.

## Checklist
- [x] Branch `feat/python-base`
- [x] venv created with Python 3.13 (`.venv`)
- [x] `pyproject.toml` (setuptools, src layout, dev extras: pytest, ruff)
- [x] `src/stakeholders_map/` with `__init__.py` and `__main__.py`
- [x] `tests/test_smoke.py`
- [x] `.gitignore` Python entries, README setup section
- [x] Editable install with dev extras

## Evidence
- `python -m stakeholders_map` → `stakeholders_map 0.1.0`
- `pytest -q` → `1 passed in 0.01s`
- `ruff check src tests` → `All checks passed!`
- `git status` does not list `.venv/` (ignored)

## Next step
`specify` (or `idea-refinement`): define stakeholders, relationships and what the app does for its user, before adding domain code.
