# Kaggle ML Pipeline

A machine learning workflow for tabular classification, developed around Kaggle's [Predicting Smartphone Addiction](https://www.kaggle.com/competitions/playground-series-s6e8) competition. The task is to predict whether an individual is classified as addicted based on demographic, behavioral, and smartphone usage features, with **ROC AUC** as the evaluation metric.

The project covers exploratory data analysis, feature relationships and selection, and model development with cross-validation and hyperparameter optimization.

## Notebooks

The workflow is divided into three notebooks:

### 1. Data Visualization

Explores the training data through:

* Missing-value analysis
* Categorical feature distributions
* Numerical feature distributions
* Comparisons between the two target classes

### 2. Feature Correlation and Selection

Investigates relationships between features and their relevance to the target.

The notebook includes:

* Pearson and Spearman correlation analysis
* Mutual information
* Feature clustering with K-Means
* Permutation importance
* Pairwise feature evaluation
* Feature engineering and selection

### 3. Model

Develops and evaluates the classification model using the selected features.

The notebook includes:

* Stratified cross-validation
* XGBoost classification
* Optuna hyperparameter optimization
* Early stopping
* ROC AUC evaluation
* Analysis of Optuna trials and parameter importance

## Project Structure

```text
kaggle-ml-pipeline/
├── notebooks/
│   ├── data_visualization.ipynb
│   ├── feature_correlation_selection.ipynb
│   └── model.ipynb
├── requirements.txt
└── README.md
```

## Purpose

The repository has two main purposes:

1. Provide a practical example of a structured workflow for tabular classification.
2. Provide a simple, ready-to-use methodology that can serve as a baseline for similar machine learning tasks.
