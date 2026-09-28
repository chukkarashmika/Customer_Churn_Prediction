# Customer Churn Prediction

## Project Overview

This project uses machine learning to predict whether a customer is likely to churn based on customer information and service usage details.

The project includes data preprocessing, exploratory data analysis (EDA), feature selection, model training, and evaluation using Logistic Regression.

## Dataset

The dataset contains customer demographic information, service details, contract information, billing details, and churn status.

* Original records: 7,043
* Records after cleaning: 7,032
* Original features: 21
* Features after one-hot encoding: 30 input features

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook
* Joblib

## Project Workflow

1. Data loading
2. Data inspection
3. Data cleaning
4. Missing-value handling
5. Exploratory Data Analysis
6. Categorical variable encoding
7. Feature selection using SelectKBest
8. Train-test split
9. Feature scaling using StandardScaler
10. Logistic Regression model training
11. Model evaluation
12. Model saving and loading

## Exploratory Data Analysis

The following visualizations were created:

* Customer churn distribution
* Customer tenure distribution
* Monthly charges distribution
* Churn vs contract type
* Churn vs internet service
* ROC curve

## Machine Learning Model

A Logistic Regression classifier was used for customer churn prediction.

The pipeline consists of:

* SelectKBest with ANOVA F-test
* StandardScaler
* Logistic Regression

The dataset was divided into:

* Training data: 5,625 records
* Testing data: 1,407 records

Stratified splitting was used to maintain the churn class distribution.

## Model Performance

* Accuracy: **79.25%**
* ROC-AUC: **0.830**

The ROC curve was also used to evaluate the model's ability to distinguish between customers who churn and customers who do not churn.

## Project Structure

```text
Customer_Churn_Prediction/
│
├── Dataset/
│   └── customer_churn.csv
│
├── Images/
│   ├── churn_distribution.png
│   ├── tenure_distribution.png
│   ├── monthly_charges_distribution.png
│   ├── churn_contract.png
│   ├── churn_internet_service.png
│   └── roc_curve.png
│
├── models/
│   └── customer_churn_model.pkl
│
├── Notebooks/
│   └── Customer_Churn_Analysis.ipynb
│
└── README.md
```

## Conclusion

The project demonstrates how machine learning can be applied to customer churn prediction. The trained model achieved an accuracy of 79.25% and a ROC-AUC score of 0.830 on the test dataset.

The model can be used as a predictive analytics tool to identify customers who may be likely to churn and to support analysis of customer retention patterns.
