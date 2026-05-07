# Glioblastoma Transcriptomic Clustering
**An Unsupervised Machine Learning Pipeline for Biomarker Discovery in High-Dimensional RNA-seq Data**

Author: Santiago López Cervantes

---

## Project Overview
Welcome to the documentation for the Glioblastoma Subtype Analysis project. This repository details an end-to-end bioinformatics pipeline designed to address the clinical challenge of Glioblastoma (GBM) tumor heterogeneity. 

Using bulk RNA-sequencing data from The Cancer Genome Atlas (TCGA), this project implements unsupervised machine learning to mathematically isolate distinct molecular phenotypes and extract the specific genetic biomarkers driving their divergence.

### Core Objectives
1. **Dimensionality Reduction:** Process a high-dimensional transcriptomic matrix (~60,000 features) using log-normalization, variance filtering, and Principal Component Analysis (PCA).
2. **Unsupervised Clustering:** Implement and evaluate clustering algorithms (K-Means vs. Agglomerative Hierarchical) to determine the optimal molecular taxonomy of the cohort.
3. **Biomarker Discovery:** Execute non-parametric differential expression analysis (Mann-Whitney U) to isolate statistically significant, high-magnitude protein-coding drivers.
4. **Clinical Integration:** Map the mathematically derived transcriptomic clusters to real-world patient phenotype and survival data to prove prognostic relevance.

---
*Built with Python, Scikit-Learn, SciPy, and Pandas. Data provided by [TCGA UCSC Xena repository](https://xenabrowser.net/datapages/?cohort=GDC%20TCGA%20Glioblastoma%20(GBM)&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443).*