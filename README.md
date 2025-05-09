# Customer Churn Prediction

## Overview
This project explores customer churn in the telecom industry using classification models. The objective is to identify customers who are likely to churn so the company can take proactive retention measures. Two models were developed: a logistic regression model and a decision tree, with the latter tuned to improve performance.

## Business and Data Understanding
### Stakeholder Audience
The primary audience for this project includes business leaders, marketing analysts, and customer Service team. They are interested in understanding which customers are at risk of leaving and what patterns or customer characteristics contribute to churn.

### Dataset
The dataset used contains customer demographics, service plans, usage patterns, and customer service interactions. It was sourced from Kaggle and includes a target variable indicating whether a customer has churned.

Key features include:

- Contract type (I.e. month-to-month)
- Internet and phone service
- Monthly charges and total charges
- Number of customer service calls
- Tenure

## Modeling
Two models were developed for this problem:

### 1. Logistic Regression (Baseline)
A simple, interpretable model that establishes a baseline. 

### 2. Decision Tree
A decision tree model was trained in two forms:
- **Baseline Decision Tree** with  default parameters
- **Tuned Decision Tree** using `max_depth=5` to  reduce overfitting

All models were trained on an 80/20 train-test split and evaluated on the test set.

## Evaluation
The models were evaluated using accuracy, precision, recall, and ROC AUC.

### Logistic Regression
- Accuracy 86.1%
- Precision (Churn) 54%
- Recall (Churn) 26%
- ROC AUC 0.81

### Tuned Decision Tree
- Accuracy 91.8%
- Precision (Churn) 76%
- Recall (Churn) 63%
- ROC AUC  0.81

The tuned decision tree outperformed the logistic regression model, especially in recall, making it better suited for identifying churners.

## Conclusion
This project successfully used classification models to predict telecom customer churn. The decision tree classifier, particularly after tuning, provided the best results. It is recommended for use in business scenarios where interpretability and actionable retention strategies are needed.

Further improvements can include incorporating more customer behavior data for increased accuracy.
