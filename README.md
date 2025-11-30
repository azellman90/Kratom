# NSDUH 2019 – Kratom Analysis (MIS581 Capstone Project)

Author: **Amy Zellman**  
Course: MIS581 – Capstone  
Institution: Colorado State University – Global Campus

## Overview

This repository contains the full analysis for a capstone project examining national-level predictors of kratom use (Mitragyna speciosa) using the 2019 National Survey on Drug Use and Health (NSDUH).

The project focuses on:

- Weighted national prevalence of lifetime kratom use
- Differences in prevalence by sex and race/ethnicity
- Associations between kratom use and:
  - Age
  - Sex
  - Income
  - Substance use disorder (SUD)
  - Nonmedical opioid use (`udpyopi`)
  - Lifetime heroin use (`herever`)
- An expanded survey-weighted logistic regression model with additional sociodemographic covariates
- Classification tree modeling (unweighted)
- ROC curve and AUC for model performance
- Principal component analysis (PCA) of recovery-related factors

All analyses are performed using R and the `survey` package to account for the complex NSDUH design.

## Files

- R Code
  - Data import
  - Variable renaming
  - Derived variable creation
  - Survey design specification
  - Weighted prevalence analysis
  - Logistic regression models
  - Classification tree
  - ROC/AUC
  - PCA

- `Screenshots/`  
  Folder containing screenshots of key analysis outputs (console and plots), as required by MIS581.

- Repository 
  Variable mapping from original NSDUH file (V1–V42) to cleaned variable names used in the script.

- Capstone Paper
  Final APA-formatted capstone report (paper).

- MIS581 Presentation  
  Slide deck for capstone presentation.

## How to Run

1. Install required R packages:

   ```r
   install.packages(c("dplyr", "survey", "ggplot2", "broom", "rpart", "pROC"))
