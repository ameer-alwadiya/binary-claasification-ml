Sure, here's a README file for your GitHub repository:

---

# Predicting the Biodegradability of Chemicals

This repository contains the code and data used in the study "Predicting the Biodegradability of Chemicals from QSAR data" by Ameer S. H. Alwadiya. The research explores the application of supervised machine learning models to predict the biodegradability of chemicals using Quantitative Structure-Activity Relationship (QSAR) data. 

## Table of Contents

- [Introduction](#introduction)
- [Data Processing](#data-processing)
- [Methodology](#methodology)
  - [Logistic Regression using sklearn](#logistic-regression-using-sklearn)
  - [Support Vector Classification (SVC) using sklearn](#support-vector-classification-svc-using-sklearn)
  - [Logistic Regression from Scratch](#logistic-regression-from-scratch)
- [Model Analysis](#model-analysis)
- [Conclusion and Recommendations](#conclusion-and-recommendations)
- [References](#references)
- [How to Run](#how-to-run)

## Introduction

In the face of escalating environmental challenges, the application of machine learning technologies has become imperative for devising effective solutions. This repository contains code for building predictive models to understand the biodegradability of chemicals—a crucial factor in preventing their harmful accumulation and environmental dispersion. 

## Data Processing

The dataset used contains information on QSAR and the biodegradability status of 1,055 chemicals. Each row in the dataset corresponds to a specific chemical, with 41 features and a label indicating biodegradability (1) or non-biodegradability (0). The data is pre-processed to remove redundant features and standardize the values using Z-score normalization.

## Methodology

### Logistic Regression using sklearn

A logistic regression model is employed using the scikit-learn library. The logistic function and cross-entropy loss are used for classification. Hyperparameters are tuned using Grid Search Cross-Validation.

### Support Vector Classification (SVC) using sklearn

Support Vector Classification involves finding a hyperplane that best separates the data into different classes. The RBF kernel function is used, and hyperparameters are tuned using Grid Search Cross-Validation.

### Logistic Regression from Scratch

A logistic regression model is implemented from scratch to gain a deeper understanding and customization for the specific task. The model uses gradient descent for optimization.

## Model Analysis

The data is split into training and testing sets (80% training, 20% testing). Model performance is evaluated using confusion matrices and ROC curves. The AUC scores are:
- Logistic Regression using sklearn: 0.939
- Support Vector Classification: 0.949
- Logistic Regression from Scratch: 0.946

## Conclusion and Recommendations

The Support Vector Classifier demonstrates the highest accuracy in predicting the biodegradability of chemicals. The custom logistic regression model also shows competitive performance, highlighting the importance of parameter tuning and algorithm selection.

## References

1. K. Mansouri, T. Ringsted, D. Ballabio, R. Todeschini, and V. Consonni, “Quantitative structure–activity relationship models for ready biodegradability of chemicals,” Journal of chemical information and modeling, vol. 53, no. 4, pp. 867–878, 2013

## How to Run

1. Clone the repository:
   ```
   git clone https://github.com/ameer-alwadiya/binary-classification-ml.git
   ```
2. Navigate to the directory:
   ```
   cd binary-classification-ml
   ```
3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
4. Open the Jupyter Notebook:
   ```
   jupyter notebook Predicting%20the%20Biodegradability%20of%20Chemicals.ipynb
   ```
5. Run the notebook cells to execute the code and reproduce the results.

---

Feel free to customize this README further to match the specifics of your project and repository structure.
