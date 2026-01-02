# Longitudinal Analysis of PBC Treatment Outcomes

## Overview
This project analyzes longitudinal health outcomes in a cohort of 312 Mayo Clinic patients
diagnosed with Primary Biliary Cirrhosis (PBC) between 1974 and 1984. The primary goal is
to evaluate the effectiveness of D-penicillamine treatment on disease progression using
repeated serum bilirubin measurements collected over a ten-year period.

A longitudinal modeling framework is used to account for within-patient correlation and
unequal follow-up times.

## Data
- **Source:** Mayo Clinic (pbcseq dataset, R `survival` package)
- **Sample size:** 312 patients (158 treated, 154 controls)
- **Response variable:** Serum bilirubin (mg/dL)
- **Predictors:** Clinical indicators of liver disease, blood clotting measures,
  and demographic variables (age, sex)

## Methods
- Data preprocessing and exploration in R
- Exploratory analysis using spaghetti plots and response distributions
- Linear mixed-effects models to estimate treatment effects over time while accounting
  for patient-specific trajectories

## Results
- Serum bilirubin levels generally increased over time, consistent with progressive
  liver deterioration, and were associated with multiple clinical markers
- No statistically significant effect of D-penicillamine on bilirubin trajectories
  was observed
- Findings are consistent with prior evidence indicating limited clinical benefit
  and increased risk of adverse outcomes, contributing to the discontinuation of
  the treatment in practice

Selected visualizations are available in the accompanying PDF report.

## Limitations and Future Work
- Data reflect clinical practice from over 40 years ago
- Serum bilirubin is an imperfect proxy for overall disease severity
- Approximately 5% of predictor values required imputation, which may influence estimates

## Reproducibility
All analyses were conducted in R. The R Markdown file contains code to download,
preprocess, and analyze the data using the `survival`, `nlme`, and `ggplot2` packages.
