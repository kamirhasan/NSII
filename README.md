# National Skill Intelligence Index (NSII)
**A GATv2 + XGBoost Framework for AI-Displaced Worker Wage Capacity Prediction**

This repository contains all analytical code, figures, and summary results for the paper:

> Khan, A. H. (2025). The National Skill Intelligence Index (NSII): A Graph Attention Network
> and Machine Learning Framework for Predicting Wage Capacity of AI-Displaced Workers in the
> Midwest Manufacturing Corridor. *Expert Systems with Applications*.

## Repository Structure

| Folder | Contents |
|--------|----------|
| notebooks/ | Four Jupyter notebooks (Phases 1–4) |
| figures/ | Six publication-quality PNG figures (300 DPI) |
| results/ | CSV summary tables from all four phases |
| data/ | Data source documentation and crosswalks |

## Computational Environment

- Phases 1, 2, 4: Google Colaboratory (CPU runtime)
- Phase 3 (GNN + XGBoost): Kaggle Notebooks (NVIDIA Tesla T4 GPU, 15.6 GB VRAM)
- Python 3.12, PyTorch 2.1.0, PyTorch Geometric 2.5.0, XGBoost 3.2.0
- Full dependency list: requirements.txt

## Data Sources

All data are from US federal government sources:
- IPUMS CPS ASEC (ipums.org) — 2019–2024
- BLS OEWS (bls.gov/oes) — 2019–2024
- O*NET v29.0 (onetonline.org)
- HMDA (consumerfinance.gov) — 2019–2023
- FRED (fred.stlouisfed.org)
- Census LEHD QWI (lehd.ces.census.gov)

Raw data files are not redistributed (federal license). Processed outputs are in results/.

## Key Results

| Metric | Value |
|--------|-------|
| NSII range (31 occupations) | 280.7 – 655.1 |
| NSII × log(wage) Pearson r | 0.2819 (p < 10⁻⁸²) |
| XGBoost R² — NSII alone | 0.3661 |
| XGBoost R² — Full model | 0.5503 |
| GNN reconstruction r | 0.8461 |
| Workers analysed | 4,464 |

## Contact

Amir Hasan Khan | khan.295@wright.edu
Raj Soin College of Business, Wright State University, Dayton, Ohio, USA

