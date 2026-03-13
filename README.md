# Causal Effect of Obesity on Systolic Blood Pressure

Prepared by Eric Dien

## Project Overview

This project estimates the causal effect of obesity on systolic blood pressure (SBP) using observational health data from the NHIS Health Screening Dataset.

The analysis evaluates both:

* The **total causal effect** of obesity on SBP
* The **indirect pathway through waist circumference**

## Methods

The following causal inference methods were implemented:

* OLS regression adjustment
* Propensity score matching (PSM)
* Inverse probability weighting (IPW)
* Conditional average treatment effects (CATE) by age
* E-value sensitivity analysis for unobserved confounding

## Dataset

**National Health Insurance Service (NHIS) Health Screening Dataset**

Available via Kaggle.

Working sample used in analysis: **4,402 individuals**

## How to Run

### Prerequisites

* R (version 4.2 or newer recommended)
* RStudio recommended

### 1. Clone the repository

```bash
git clone https://github.com/ericdien121/causal-obesity-sbp.git
cd causal-obesity-sbp
```

### 2. Install required packages

Run the following in R:

```r
install.packages(c("tidyverse", "MatchIt", "survey", "broom", "ggplot2"))
```

### 3. Add the dataset

Download the **NHIS Health Screening Dataset** from Kaggle and place the dataset file inside the project directory.
Update the file path in the R script if necessary.

### 4. Run the analysis

Run the main R script or R Markdown file used in the analysis.

Example:

```r
source("analysis.R")
```

or if using R Markdown:

```r
rmarkdown::render("analysis.Rmd")
```

## Output

The analysis produces:

* Estimated causal effect of obesity on systolic blood pressure
* Comparison of OLS, PSM, and IPW estimates
* Age-based treatment effect heterogeneity
* Sensitivity analysis results using the E-value

## Skills Demonstrated
- Causal inference
- Propensity score methods
- Observational data analysis
- R statistical programming
- Sensitivity analysis
