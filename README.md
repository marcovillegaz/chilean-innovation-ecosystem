# chilean-innovation-ecosystem

Stakeholder map of the Chilean innovation ecosystem, modelled with OOP to expose
relevant interactions and relationships, growing into an app.

## Setup (Windows / PowerShell)

```powershell
py -3.13 -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -e ".[dev]"
```

## Run and test

```powershell
python -m stakeholders_map
pytest
ruff check src tests
```
