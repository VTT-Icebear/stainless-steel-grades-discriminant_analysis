# Discriminant Analysis for Classifying Stainless Steel Grades

Classifying SS304, SS304L, SS316, SS316L from OES chemical composition
(C, Si, Mn, Cr, Mo, Ni) using LDA and QDA.
Vietnamese-German University, Data Analysis course.

## Main results
- Validation: spark-level LOOCV, leave-one-block-out CV (LOBO-CV), block-level hold-out
- LOBO-CV accuracy: LDA 82.88%, QDA 79.28% (LDA chosen)
- Mo separates the 304 and 316 families; most errors are SS316 vs SS316L

## Files
- `report/` : final report (PDF)
- `R/` : R scripts

## Requirements
R packages: MASS, biotools, klaR, ggplot2

## Authors
Group 10: Dieu Ngoc Thien An, Vuong Thai Thinh, Nguyen Huu Tri, Vu Gia Bao
