
# Layoffs Analysis (2020–2023)

## Overview

This repository presents a structured analytics project built around global layoffs from March 2020 through March 2023. The project spans data ingestion, cleaning, transformation, and exploratory analysis using SQL and Tableau. While the summary below outlines the process, detailed findings and transformations have been documented separately for deeper context.

## Objective

To explore the patterns, timing, and concentration of workforce reductions across industries, countries, and company stages in a post-pandemic economic environment, using reliable and structured data workflows.

---

## Data Source

The primary dataset was obtained from Kaggle and consists of publicly reported layoff events across the globe. The data was originally unstructured and required comprehensive preprocessing before use in analysis.

- **Original dataset**: `layoffs.csv`
- **Cleaned dataset**: `layoffs_staging2.csv`

---

## Project Structure

### 1. Data Cleaning

The data cleaning process was conducted entirely in MySQL and included:

- Backup creation and raw data preservation
- Deduplication using row partition logic
- Standardization of inconsistent text values (company, industry, country)
- Format normalization for date fields
- Strategic null-value handling and imputation
- Removal of analytically irrelevant records

A detailed explanation of each transformation is available in the report below:

> [Data Cleaning Report](./Data%20Cleaning%20Report.pdf)

---

### 2. Exploratory Data Analysis (EDA)

Post-cleaning, the dataset was analyzed to reveal multi-dimensional trends, with a focus on:

- Temporal evolution of layoffs
- Country-wise and sector-specific distributions
- Funding-stage effects on layoff volume
- Company-level and event-driven observations

Key findings are synthesized in the following report:

> [EDA Insights Report](./Unified%20Layoffs%20EDA%20Insights%20Report.pdf)

---

## Visualizations

An interactive dashboard was created in Tableau to summarize major patterns and enable dynamic slicing of the data. A static preview of this dashboard is included here:

- Dashboard File: `Layoffs Analysis.twbx`
- Preview: `Layoff Dashboard.png`

---

## Repository Contents

| File | Description |
|------|-------------|
| `layoffs.csv` | Original raw dataset from Kaggle |
| `layoffs_staging2.csv` | Cleaned and processed dataset |
| `TEMP Project work.sql` | SQL script for cleaning operations |
| `Layoffs Analysis.twbx` | Tableau dashboard file |
| `Layoff Dashboard.png` | Static preview of the dashboard |
| `Data Cleaning Report.pdf` | Full documentation of SQL cleaning steps |
| `Unified Layoffs EDA Insights Report.pdf` | Analytical report from EDA process |

---

## Next Steps

The prepared dataset and insights may serve as a foundation for:

- Predictive modeling on employment trends
- Cross-industry impact assessments
- Strategic workforce planning tools

---
