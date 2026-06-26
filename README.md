# Predicting Employment Outcomes among Young Adults

### Machine Learning Analysis Using the PSID Transition into Adulthood Supplement (PSID-TAS)

## Overview

This project investigates the factors that predict employment outcomes among young adults in the United States using data from the **Panel Study of Income Dynamics Transition into Adulthood Supplement (PSID-TAS)**.

The study compares the predictive performance of **educational attainment**, **psychological well-being**, and **economic hardship** across multiple statistical and machine learning methods. Rather than relying on a single model, the project evaluates whether the same conclusions are supported across traditional econometric models and modern machine learning approaches.

The project was completed as part of an undergraduate research project at the **University of Washington**.

---

## Research Question

> **Which characteristics best predict employment outcomes among young adults?**

Specifically, the project examines whether

* Educational attainment
* Psychological well-being
* Financial hardship
* Previous employment experience
* Family background

provide meaningful information for predicting employment status.

---

## Dataset

**Source**

Panel Study of Income Dynamics (PSID)

Transition into Adulthood Supplement (TAS)

**Sample**

* 2,434 young adults
* United States nationally representative survey
* Cross-sectional 2023 data
* Longitudinal information from 2021 used for additional analyses

The original PSID data are not included in this repository because they are distributed under a restricted data agreement.

---

## Methods

The project compares several statistical and machine learning models.

### Statistical Models

* Logistic Regression
* Linear Probability Model (OLS)

### Machine Learning Models

* Decision Tree (CART)
* Random Forest
* LASSO Regression
* Support Vector Machine (SVM)
* Double Machine Learning (DoubleML)

These methods were used to compare predictive performance, evaluate variable importance, and identify robust predictors of employment.

---

## Key Findings

The results consistently indicate that:

* Educational attainment is the strongest predictor of employment.
* College attendance and years of education appear among the most important variables across nearly all models.
* Psychological well-being contributes relatively little predictive information once education is taken into account.
* Economic hardship (measured using 2021 SNAP participation) predicts a higher probability of unemployment in 2023.
* Previous employment status and responsibility-related behaviors remain important predictors in longitudinal models.

Across logistic regression, random forests, LASSO, SVM, and Double Machine Learning, educational variables consistently outperform well-being measures.

---

## Repository Structure

```
PSID-Employment-Prediction
│
├── README.md
├── Project Report Natalie.pdf
│
├── code
│   ├── Education&Wellbeing.Rmd
│   ├── dml.Rmd
│   └── FoodInsecurity_Unemployment.R
│
├── figures
│   ├── logistic_regression.png
│   ├── decision_tree.png
│   ├── random_forest.png
│   ├── lasso.png
│   └── svm.png
│
└── data
    └── Data description only (PSID data not included)
```

---

## Programming Languages

* R
* R Markdown

---

## Main Packages

* tidyverse
* glm
* rpart
* randomForest
* glmnet
* e1071
* DoubleML
* mlr3
* ranger

---

## Skills Demonstrated

* Data Cleaning
* Feature Engineering
* Predictive Modeling
* Machine Learning
* Statistical Modeling
* Variable Selection
* Model Comparison
* Causal Machine Learning
* Data Visualization
* Reproducible Research using R Markdown

---

## Results

The final report summarizes:

* Descriptive statistics
* Logistic regression
* Decision tree analysis
* Random forest variable importance
* LASSO regularization
* Support Vector Machine evaluation
* Double Machine Learning estimation
* Discussion and policy implications

---

## Future Improvements

Potential extensions include

* XGBoost
* LightGBM
* SHAP value interpretation
* Hyperparameter tuning
* Cross-validation optimization
* Additional longitudinal analyses

---
