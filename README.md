# Shock and No Shift: Impact of the Expulsion Initiative on Foreign Crime Rates in Switzerland

> **Key Finding**: Our difference-in-differences analysis reveals no statistically significant impact of Switzerland's 2016 expulsion law on violent crime rates among foreign residents.

## 🔍 Research Question
**Did the implementation of Switzerland's 2016 expulsion law for foreign criminals reduce violent crime rates among foreign residents?** 

This project empirically evaluates the impact of the constitutional amendment (Art. 121) and Criminal Code Art. 66a implementation on foreign crime rates using canton-level data from 2010-2023.

## 📜 Key Publications
- [Federal Constitution Amendment (Art. 121)](https://www.fedlex.admin.ch/eli/cc/1999/404/en#art_121)
- [Criminal Code Art. 66a](https://www.fedlex.admin.ch/eli/cc/54/757_781_799/en#art_66a)

## 📊 Methodology
We employ a **difference-in-differences (DiD)** design comparing foreign residents (treatment group) to Swiss nationals (control group) with multiple robustness checks:

```mermaid
graph LR
A[DiD Design] --> B[Fixed Effects]
A --> C[Parallel Trends Validation]
A --> D[Wild Cluster Bootstrap]
A --> E[Placebo Tests]
A --> F[Box-Cox Transformation]
A --> G[Canton-level Heterogeneity Analysis]
