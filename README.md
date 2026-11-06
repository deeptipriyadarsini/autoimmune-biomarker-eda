# Autoimmune Biomarker EDA

Exploratory data analysis and cleaning of a rheumatic and autoimmune disease lab biomarker dataset, done as Assignment 2 for the Data Exploration module at TU Dublin.

## Domain

Clinical rheumatology/immunology — lab serology data used to help diagnose rheumatic and autoimmune diseases from biomarker test results.

## Purpose

To explore how lab biomarkers can support early detection of rheumatic and autoimmune disease.

## Dataset

- **Source**: Abd, Mahdi & Jahani (2025), *Rheumatic and Autoimmune Diseases Dataset*, Harvard Dataverse, [doi.org/10.7910/DVN/VM4OR3](https://doi.org/10.7910/DVN/VM4OR3) (CC BY 4.0).
- **Original file**: 12,085 records, 15 columns (clean, unmodified, read-only).
- **Modified file** (`Rheumatic and Autoimmune Disease Dataset_modified.xlsx` / `.csv`): 12,140 records, 16 columns — duplicate rows, outliers, inconsistent date/time values, and categorical inconsistencies were intentionally introduced for the purposes of this assignment.

## Contents

| File | Description |
|---|---|
| `A00083343_assignment2.ipynb` | Main analysis notebook: dataset overview, data quality checks, cleaning, and exploratory analysis |
| `Rheumatic and Autoimmune Disease Dataset_modified.xlsx` | Modified dataset used in the notebook |
| `Rheumatic and Autoimmune Disease Dataset_modified.csv` | CSV version of the same dataset |

## Approach

1. **Dataset overview & inspection** — shape, column types, mixed data types, missing values, categorical inconsistencies (e.g. gender case variants, serology result encodings).
2. **Data cleaning & preparation** — missing numeric lab values imputed with median (per-disease baselines vary and right-skewed distributions make median a more realistic center); missing categorical lab values filled as `'Unknown'` rather than dropped, since not every test is run for every disease.
