# Shock and No Shift: Impact of the Expulsion Initiative on Foreign Crime Rates in Switzerland

**Authors:** Souhil Khiat, Simon Schmidt-Ginzkey, Martin Sinishta, Tommaso Spreij, Timon van Engen  
**Affiliation:** HEC Lausanne, Faculty of Business & Economics, University of Lausanne  
**Date:** June 2025

---

## Project Overview

This repository contains all code, data, plots, and the full LaTeX source for the paper:

> **Shock and No Shift: Impact of the Expulsion Initiative on Foreign Crime Rates in Switzerland**  
> _The findings are data-driven and do not reflect any normative stance._

On October 1<sup>st</sup>, 2016, Switzerland’s “Pour le renvoi des étrangers criminels” initiative (expulsion of foreign criminals) took effect. Using canton-level data from 2010–2023, we implement a Difference-in-Differences (DiD) framework comparing violent‐crime rates among foreign residents vs. Swiss nationals. We find no statistically significant effect of the expulsion law on foreign‐resident violent crime.

Key contributions:

- First empirical evaluation of Switzerland’s 2016 expulsion law.  
- Panel data (26 cantons × 2 residency groups × 14 years = 728 cells).  
- Robustness checks: parallel‐trend tests, event-study, alternative transformations (Box–Cox, log, linear), placebo reforms, canton heterogeneity, wild-bootstrap inference.  

---

## Repository Structure

Below is a high-level view of the folder structure. Each main folder and its contents are described in detail.

```text
├── data
│   ├── raw
│   │   ├── crimes_subject_to_law_raw.xlsx
│   │   ├── crimes_subject_to_law_raw_by_…xlsx
│   │   ├── population_raw.xlsx
│   │   └── population_raw_by_canton.xlsx
│   └── processed
│       ├── crimes_subject_to_law_cleaned.csv
│       └── crimes_subject_to_law_cleaned_by_canton.csv
├── plots
│   ├── BoxCoxProfile.png
│   ├── BoxCoxProfile_with_CI.png
│   ├── crime_rate_transformations.png
│   ├── did_graph.png
│   ├── did_graph_boxcox.png
│   ├── did_graph_linlin.png
│   ├── did_graph_loglin.png
│   ├── foreigner_year_interaction.png
│   ├── foreigner_year_interaction_linear.png
│   ├── pre_2017_trend_linlin.png
│   ├── pre_2017_trend_loglin.png
│   ├── pre_2017_trend_loglin.png
│   └── keepgit  ← (empty placeholder to ensure Git tracks this folder)
├── script
│   ├── 01_data_cleaning.ipynb
│   ├── 02_parallel_trends_test_comparison.ipynb
│   ├── 02_parallel_trends_test_comparison_alt.ipynb
│   ├── 03_did_BC_optimal.ipynb
│   ├── 03_did_linear.ipynb
│   ├── 03_did_log.ipynb
│   └── README.md  ← (this file)
├── main.tex  ← LaTeX source for the paper
└── references.bib  ← BibLaTeX bibliography file
