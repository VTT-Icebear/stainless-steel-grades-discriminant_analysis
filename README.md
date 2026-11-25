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


## Repository Structure

```text
.
├── data/
│   ├── dataset_for_analysis/
│   │   └── DA dataset-20261125T092909Z-1-001.zip   # Full dataset archive for analysis
│   └── sample/                                       # Sample OES CSV files for quick inspection/testing
│       ├── 261103-18.CSV
│       ├── 26260-1.CSV
│       ├── 26363-2.CSV
│       └── 26723-1.CSV
├── report/
│   └── Project_Outline_LDA_LaTeX_Report.pdf          # Project outline / report
├── slides/
│   └── CE1.pdf                                       # Presentation slides
└── src/
    ├── analysis.R                                    # R script for data analysis, modeling, and evaluation
    └── analysis.ipynb
