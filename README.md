
# RNA-Seq Differential Expression Analysis

## Overview

This project investigates differential gene expression in metastatic triple-negative breast cancer using publicly available RNA-seq data from GEO dataset GSE184717.

Using R, I developed an RNA-seq analysis workflow incorporating data preprocessing, principal component analysis (PCA), differential expression analysis with DESeq2, and statistical comparison with Benjamini-Hochberg-adjusted t-tests.

The objective was to identify genes differentially expressed between metastatic tumor and adjacent normal tissue samples and evaluate agreement between statistical methods.

## Tools and Technologies

- **Language:** R
- **Packages:** GEOquery, DESeq2, ggplot2, dplyr, knitr
- **Methods:** RNA-seq preprocessing, PCA, differential expression analysis, t-tests, Benjamini-Hochberg correction
- **Data Source:** NCBI GEO (GSE184717)

## Key Findings

- Analyzed RNA-seq data from 42 tissue samples, including 28 metastatic tumor biopsies and 14 adjacent normal tissue samples.
- PCA revealed that PC1 explained 60% of the total variance, primarily separating tumor and normal tissue samples.
- DESeq2 identified **14,829 significantly differentially expressed genes** (adjusted p-value < 0.05).
- Benjamini-Hochberg-adjusted t-tests identified **14,434 significant genes**, with **13,453 genes overlapping** between both methods.
- The substantial overlap demonstrated strong agreement between the two statistical approaches.

## Limitations

All 42 samples originated from a single patient, representing spatial pseudoreplicates rather than independent biological replicates. Therefore, the findings are patient-specific and require validation in larger, independent cohorts.

## Project Files

- `analysis.Rmd` - R Markdown source code and analysis workflow
- `index.html` - Full analysis report with code, visualizations, and results

## Data Source

[GEO Dataset GSE184717](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE184717)

---

**M.S. Bioinformatics | Brandeis University | July 2026**
