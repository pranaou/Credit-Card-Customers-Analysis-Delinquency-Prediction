# Credit Card Customers Analysis & Delinquency Prediction

## Overview

This project analyzes credit card customer data to provide insights into customer demographics, transaction behaviors, and revenue distribution. Additionally, it predicts delinquent accounts using machine learning models.

The project includes:

1. **Credit Card Customers Analysis Report**: A Power BI dashboard summarizing key metrics and customer demographics.
2. **Delinquency Prediction Model Performance and Outcome**: Machine learning model evaluation for predicting delinquent accounts.

## Power BI Dashboard

### Overview of the Data

- **Total Income, Transactions, and Revenue**: Key financial metrics.
- **Revenue Distribution by Customer Occupation**: Revenue contributions by occupation.
- **Revenue Analysis by Education Level Over Time**: Revenue trends by education level.
- **Income Distribution by Marital Status and Gender**: Income distribution segmented by marital status and gender.
- **Interest Earned by Expense Type**: Interest earned across different expense types.
- **Revenue Analysis by State**: Revenue distribution across states.
- **Revenue Analysis by Age Group and Gender**: Revenue distribution by age group and gender.

### Prediction Analysis

- **Comparison of Delinquent and Non-Delinquent Account Predictions**: Model predictions across card categories.
- **Model Accuracy Comparison**: Accuracy comparison of Random Forest, XGBoost, and Logistic Regression models.
- **AUC-ROC Score Comparison by Model**: AUC-ROC scores for each model.
- **Average Probability Distribution Across Predictive Models**: Probability distribution for predicting delinquent accounts.

## Machine Learning Model Development

### Data Preparation and Feature Selection

- Merging `credit_card.csv` and `customers.csv` on `Client_Num`.
- Selected features: `Income`, `Credit_Limit`, `Total_Revolving_Bal`, `Avg_Utilization_Ratio`, `Customer_Age`.
- Categorical variables encoded using one-hot encoding.
- Dataset split into training and testing sets.

### Model Training

- **Random Forest Classifier**
- **Logistic Regression**
- **XGBoost Classifier**

Each model is saved as a `.pkl` file for future predictions.

### Model Prediction and Evaluation

- Predictions made with Logistic Regression, Random Forest, and XGBoost models.
- Accuracy and AUC-ROC scores calculated for each model.
- Results saved to `predictions.csv`, `model_accuracies.csv`, and `model_auc_roc_scores.csv`.

## Usage

1. **Power BI Dashboard**: Open the Power BI dashboard to explore the data analysis and model performance visualizations.
2. **Python Scripts**: Run the provided Python scripts for model training, prediction, and evaluation.
3. **Model Files**: Use the trained model files for predictions on new data.

## Conclusion

This project provides insights into credit card customer behavior and risk prediction using machine learning. The results and models can be used for decision-making related to customer management and risk assessment.
