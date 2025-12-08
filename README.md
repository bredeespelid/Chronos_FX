# Chronos_FX

This repository contains Jupyter notebooks used for the **Chronos-based FX forecasting experiments** in a master’s thesis. The notebooks implement monthly and quarterly walk-forward evaluations for EUR/NOK, including price-only baselines, macro-enriched variants, panel/exogenous extensions, finetuned models, and multi-FX robustness checks.

## Purpose
- Benchmark **Chronos** forecasting models for **EUR/NOK level prediction**.
- Compare model families across:
  - Price-only inputs,
  - Macro-financial covariates,
  - Panel/exogenous extensions,
  - Finetuned Chronos variants,
  - Multi-FX experiments.
- Provide reproducible notebooks aligned with the thesis evaluation design.

## Repository Structure
- `data/` — raw and processed data files used by the notebooks.
- `src/` — Jupyter notebooks for modelling and evaluation.
- `requirements.txt` — pinned dependencies.
- `LICENSE` — MIT License.

## Notebooks
All notebooks are located in `src/` and correspond to the experiment blocks in the thesis.

### Price-Only Models (PO)
- **ChronosPriceMonthly.ipynb** — Chronos price-only model, monthly frequency.  
  Link: [`src/ChronosPriceMonthly.ipynb`](src/ChronosPriceMonthly.ipynb)

- **ChronosPriceQuarterly.ipynb** — Chronos price-only model, quarterly frequency.  
  Link: [`src/ChronosPriceQuarterly.ipynb`](src/ChronosPriceQuarterly.ipynb)

### Macro-Enriched Models (EN)
- **ChronosMacroMonthly.ipynb** — Chronos with selected macro-financial covariates, monthly frequency.  
  Link: [`src/ChronosMacroMonthly.ipynb`](src/ChronosMacroMonthly.ipynb)

- **ChronosMacroQuarterly.ipynb** — Chronos with selected macro-financial covariates, quarterly frequency.  
  Link: [`src/ChronosMacroQuarterly.ipynb`](src/ChronosMacroQuarterly.ipynb)

### Panel / Exogenous-Extended Models (EN-EX)
- **ChronosPanelMonthly.ipynb** — Chronos with panel/exogenous extensions, monthly frequency.  
  Link: [`src/ChronosPanelMonthly.ipynb`](src/ChronosPanelMonthly.ipynb)

- **ChronosPanelQuarterly.ipynb** — Chronos with panel/exogenous extensions, quarterly frequency.  
  Link: [`src/ChronosPanelQuarterly.ipynb`](src/ChronosPanelQuarterly.ipynb)

### Variable Importance / LOFO
- **ChronosVariableImportance.ipynb** — LOFO-style variable-importance analysis (monthly & quarterly).  
  Link: [`src/ChronosVariableImportance.ipynb`](src/ChronosVariableImportance.ipynb)

- **ChronosFinetuning.ipynb** — LOFO-guided finetuning / covariate-selection workflow.  
  Link: [`src/ChronosFinetuning.ipynb`](src/ChronosFinetuning.ipynb)

### Multi-FX Experiments
- **ChronosMultiFX.ipynb** — Multi-FX monthly & quarterly runs for robustness checks.  
  Link: [`src/ChronosMultiFX.ipynb`](src/ChronosMultiFX.ipynb)

## Quick Start
1. Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate   # Linux/macOS
# .\.venv\Scripts\Activate.ps1  # PowerShell (Windows)
