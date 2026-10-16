# SIRL — Appendix B data

Data for Appendix B, Tables B.1–B.15, of **SIRL: Safety-Internalizing Reinforcement Learning via Invertible Log-Barrier Mapping**.

This release follows the 2026-10-16 manuscript packaged as `SIRL_MinimalSubmission_20261016_r40`. Values are taken from the existing manuscript source data; no new experiments were run.

## Contents

| Table | File | Rows |
|---|---|---:|
| B.1 | [data/B01_navigation_outcomes.csv](data/B01_navigation_outcomes.csv) | 10 |
| B.2 | [data/B02_comparison_off_summary.csv](data/B02_comparison_off_summary.csv) | 3 |
| B.3 | [data/B03_comparison_off_by_seed.csv](data/B03_comparison_off_by_seed.csv) | 15 |
| B.4 | [data/B04_ablation_off_summary.csv](data/B04_ablation_off_summary.csv) | 5 |
| B.5 | [data/B05_ablation_off_by_seed.csv](data/B05_ablation_off_by_seed.csv) | 25 |
| B.6 | [data/B06_correction_rate_summary.csv](data/B06_correction_rate_summary.csv) | 5 |
| B.7 | [data/B07_correction_rate_by_seed.csv](data/B07_correction_rate_by_seed.csv) | 25 |
| B.8 | [data/B08_correction_magnitude_summary.csv](data/B08_correction_magnitude_summary.csv) | 5 |
| B.9 | [data/B09_correction_magnitude_by_seed.csv](data/B09_correction_magnitude_by_seed.csv) | 25 |
| B.10 | [data/B10_SAC_learning_success.csv](data/B10_SAC_learning_success.csv) | 18 |
| B.11 | [data/B11_SAC_learning_collision.csv](data/B11_SAC_learning_collision.csv) | 18 |
| B.12 | [data/B12_SRad_learning_success.csv](data/B12_SRad_learning_success.csv) | 18 |
| B.13 | [data/B13_SRad_learning_collision.csv](data/B13_SRad_learning_collision.csv) | 18 |
| B.14 | [data/B14_SIRL_learning_success.csv](data/B14_SIRL_learning_success.csv) | 18 |
| B.15 | [data/B15_SIRL_learning_collision.csv](data/B15_SIRL_learning_collision.csv) | 18 |

`data/learning_curve_counts_and_denominators.csv` provides only the counts and denominators underlying B.10–B.15. `table_index.json` maps files to appendix labels. `data_dictionary.json` defines variables and units.

## Measurement and precision

CSV files preserve the full-precision source values for the reported table cells. All cells were checked against the displayed rounding in Appendix B. Percent columns use 0–100, not 0–1. Summary columns are five-seed means and sample standard deviations. Quantiles are calculated within each seed before seed-level aggregation.

Seeds are 42, 217, 1250, 612 and 19031228. Endpoint experiments use 1,800,000 physical training transitions and 500 common development scenarios per seed. Learning windows cover 100,000 transitions each. SRad OFF retains only its fixed action limiter. See `data_dictionary.json` for metric definitions.

## Scope

This repository contains only Appendix B data and documentation. It excludes source code, models, keys, manuscript/PDF files, other appendices, unreported metrics, LD-SG implementation records, factorial-contrast data from Appendix D, and machine-specific source paths.

## Citation

Haoqi Wang, Yujie Cui, and Bo Li. SIRL: Safety-Internalizing Reinforcement Learning via Invertible Log-Barrier Mapping. Appendix B dataset, 2026. No article DOI or acceptance status is asserted.

## Reuse terms

The data in this repository are licensed under the Creative Commons Attribution 4.0 International license (CC BY 4.0). Credit Haoqi Wang, Yujie Cui, and Bo Li, link to the license, and indicate changes when reusing the data. See LICENSE.txt.
