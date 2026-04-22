# GSE237290-Immune-Biomarker-Project

**Goal:** Reproduce and extend an immune gene expression–based prognostic score for early-stage basal-like breast cancer using the NanoString PanCancer Immune Panel (GSE237290).

## Data

- **Source:** NCBI GEO — GSE237290  
- **Organism:** Homo sapiens  
- **Platform:** GPL33583 — NanoString Human PanCancer Immune Panel  
- **Samples:** 57 primary tumor samples  
- **Endpoint:** Distant disease recurrence and disease-specific mortality

## Project structure

- `data/` — GEO series matrix and metadata (not tracked if large)
- `notebooks/`
  - `01_load_and_qc.ipynb`
  - `02_differential_expression.ipynb`
  - `03_prognostic_score.ipynb`
  - `04_survival_analysis.ipynb`
  - `05_ml_model.ipynb`
- `src/` — helper functions (data loading, plotting, modeling)
- `figures/` — exported plots for documentation
- `requirements.txt` — Python dependencies

## Plan

1. Load and quality control of NanoString expression data  
2. Differential expression between recurrence vs non-recurrence groups  
3. Construction of an immune-based prognostic score  
4. Survival analysis (Kaplan–Meier, risk stratification)  
5. Machine learning models to predict recurrence  
6. Biological interpretation of immune pathways

