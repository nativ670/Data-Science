# OkCupid Gender Prediction

## Project Overview

This project aims to predict the gender of OkCupid users from San Francisco by analyzing both **categorical variables** and **open-text responses**, ignoring specific physical attributes ("fair-game").

We are particularly interested in understanding differences in response patterns between men and women, both in **closed-ended questions** and in **writing style** of open-ended prompts. This study may reveal behavioral and stylistic patterns associated with gender and provide insights into user engagement on digital platforms.

The dataset contains responses from **59,946 users**, including:

* Categorical variables
* Open-text responses
* Numerical feature: age (income treated as categorical)

---

## Analysis Levels

We conduct analysis at two levels:

1. **Closed data only** (categorical variables)
2. **Open-text data only**

---

## Modeling Approach

We compare **two types of models** for each scenario:

### Logistic Regression

* Classic linear model
* Simple and interpretable
* May struggle with non-linear interactions

### Gradient Boosting Trees (GBT)

* Ensemble of decision trees
* Captures non-linear relationships
* Strong predictive performance
* Less interpretable and requires careful hyperparameter tuning

### Common Methodology

* Data split consistently into **training, validation, and test sets**
* Identical **preprocessing pipelines** for both models
* Feature selection and **L2 regularization** to prevent overfitting
* Analysis of **feature importance** and parameter estimates
* Exploration of methods for integrating **open-text responses** into structured models

---

## Goals

* Evaluate which model achieves **higher predictive accuracy**
* Assess **explanatory power** of features
* Understand model performance across **age groups** and **writing styles**
* Compare **interpretability vs predictive performance**

---

## Skills & Techniques

* Python / R for data analysis
* Feature engineering and preprocessing
* Logistic Regression & Gradient Boosting Trees
* Text analysis / NLP for open-text responses
* Model evaluation and regularization

---

## Dataset

* https://www.kaggle.com/datasets/andrewmvd/okcupid-profiles
* 59,946 user profiles from San Francisco
* Includes categorical, numerical, and textual data

---

## Usage

1. Preprocess categorical and textual data
2. Split into training, validation, and test sets
3. Fit Logistic Regression and GBT models
4. Evaluate model performance and feature importance
5. Compare predictive accuracy and interpretability
