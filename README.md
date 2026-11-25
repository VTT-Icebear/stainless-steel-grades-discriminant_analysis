# Discriminant Analysis for Classifying Stainless Steel Grades

Classifying SS304, SS304L, SS316, SS316L from OES chemical composition
(C, Si, Mn, Cr, Mo, Ni) using LDA and QDA.
Vietnamese-German University, Data Analysis course.

## Main results
- Validation: spark-level LOOCV, leave-one-block-out CV (LOBO-CV), block-level hold-out
- LOBO-CV accuracy: LDA 82.88%, QDA 79.28% (LDA chosen)
- Mo separates the 304 and 316 families; most errors are SS316 vs SS316L

## Authors
Group 10: Dieu Ngoc Thien An, Vuong Thai Thinh, Nguyen Huu Tri, Vu Gia Bao

## Requirements
R packages: MASS, biotools, klaR, ggplot2

## How to Use

Follow these steps to reproduce the analysis and inspect the results:

### 1. Prepare the Data
1. Extract `data/dataset_for_analysis/DA dataset-20261125T092909Z-1-001.zip` into `data/dataset_for_analysis/` (or verify the file path referenced inside `src/analysis.R` and `src/analysis.ipynb`).
2. To inspect the OES CSV structure or run a quick check before using the full dataset, look at the sample files in `data/sample/`:
   - `261103-18.CSV`
   - `26260-1.CSV`
   - `26363-2.CSV`
   - `26723-1.CSV`

### 2. Run the R Script (`src/analysis.R`)
From the repository root directory, run the script via terminal:

```bash
Rscript src/analysis.R



