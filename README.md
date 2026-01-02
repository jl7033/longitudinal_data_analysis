# Longitudinal Analyis of Primary Biliary Cirrhosis (PBC) and D-penicillamine treatment in Mayo Clinic Patients, 1974-1984

## Overview
This project analyzes health outcomes in patients with Primary Biliary Cirrhosis (PBC) in a longitudinal cohort of 312 Mayo Clinic patients from 1974-1984. The primary aim was to evaluate the effectiveness of D-penicillamine, a chelating compound used to eliminate copper-containing bile in the liver, on PBC through serum bilirubin levels over a ten-year period.

## Data
- **Source:** Mayo Clinic
- **Sample size:** 312 patients (158 treatment, 154 control), all of whom had PBC at the beginning of the study
- **Response Variable:** Serum Bilirubin (mg/dL)
- **Predictor Variables:** Biological indicators of liver disease (i.e. ascites, hepatomegaly, spider angiomas), blood clotting measures (i.e. platelet count), demographic data (i.e. age, sex)

## Methods
- Data access via **pbcseq** dataset in R (from the **survival** package)
- Exploratory data analysis using spaghetti plots and distribution of the response variable
- Linear mixed-effects (LME) model to measure the effect of D-penicillamine on serum bilirubin over time

## Results
- Serum bilirubin generally increased over time, indicating worse liver health, and was correlated with several other markers of liver damage
- D-penicillamine did not significantly affect patients' PBC severity over time
- Results align with a 2006 meta-analysis that determined that D-penicillamine does not decrease morbidity or mortality while increasing risk of adverse events; the treatment has largely been discontinued

Selected visualizations are available in the accompanying PDF report.

## Limitations and Future Work
- Analysis uses data from more than 40 years ago
- Serum bilirubin is not a perfect predictor of PBC severity
- Imputation for ~5% of observations for some predictor variables may have affected model estimates

## Reproducibility
All analyses were conducted in R. The R Markdown file contains code to download,
preprocess, and analyze the data using the **survival**, **nlme** and **ggplot2** packages.
