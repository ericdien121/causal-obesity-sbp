# Causal Effect of Obesity on Systolic Blood Pressure
Author: Eric Dien

## Project Overview

This project estimates the causal effect of obesity on systolic blood pressure (SBP) using observational health data from the NHIS health screening dataset.

The analysis examines both:

- The **total causal effect** of obesity on SBP
- The **indirect pathway through waist circumference**

## Methods

The following causal inference methods were used:

- OLS regression adjustment
- Propensity score matching (PSM)
- Inverse probability weighting (IPW)
- Conditional average treatment effects (CATE) by age
- E-value sensitivity analysis

## Dataset

National Health Insurance Service (NHIS) Health Screening Dataset  
Available via Kaggle.

Working sample used in analysis: **4,402 individuals**

## Repository Structure
