# Telecom Churn Analysis Project

## Overview

This project focuses on analyzing telecom customer churn, a critical issue for service providers. The dataset, sourced from [provide dataset source if applicable], contains information about customers' attributes and their churn status. The goal is to gain insights through exploratory data analysis (EDA) and build machine learning models for predicting customer churn.

The project is structured into two main phases:

### 1. Exploratory Data Analysis (EDA)

The first phase involves exploring and understanding the dataset:

- **Data Cleaning:** Handled missing values and converted data types for analysis.
- **Univariate Analysis:** Examined distributions and counts of individual features.
- **Bivariate Analysis:** Explored relationships between features and their impact on churn.
- **Visualization:** Utilized various plots to visualize patterns and trends in the data.

Key findings from EDA:

- Customer churn is influenced by factors such as contract type, monthly charges, and total charges.
- The dataset initially had missing values, mainly in the 'TotalCharges' column, which were addressed through data cleaning.
- The 'Random Forest' model was selected for its superior performance in predicting churn based on the EDA insights.

### 2. Model Building

The second phase focuses on building and evaluating machine learning models:

- **Decision Tree Classifier:** Achieved an accuracy of 78.4% on the test set.
- **Random Forest Classifier:** Attained an accuracy of 77.8% on the test set, with detailed classification metrics.
- **Logistic Regression:** Achieved an accuracy of 79.0%, with a warning about convergence.

**Final Model Selection:** The Random Forest model with SMOTEENN for handling imbalanced data was chosen as the final model due to its accuracy of 90.3% on the test set.

### Results

- **Decision Tree Classifier:**
  - Accuracy: 78.4%
  - Confusion Matrix: [[401, 43], [51, 487]]

- **Random Forest Classifier:**
  - Accuracy: 77.8%
  - Detailed Classification Report:
    - Precision: 81% (Churn=0), 64% (Churn=1)
    - Recall: 92% (Churn=0), 39% (Churn=1)
    - F1-score: 86% (Churn=0), 49% (Churn=1)

- **Logistic Regression:**
  - Accuracy: 79.0%
  - Warning: ConvergenceWarning (consider increasing iterations or scaling data)

- **Final Model (Random Forest with SMOTEENN):**
  - Accuracy: 90.3%
  - Confusion Matrix: [[394, 55], [39, 482]]

## Next Steps

- Address the `ConvergenceWarning` in the Logistic Regression model training by following the suggestions provided in the warning.
- Ensure consistency in variable names for better code readability.
- Include visualizations for better presentation of results.
- Consider hyperparameter tuning for further model improvement.

## Author

Nanditha Nambiar

