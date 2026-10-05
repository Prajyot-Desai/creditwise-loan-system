# CreditWise Loan System

An end-to-end supervised machine learning project for predicting whether a loan application will be approved or rejected.

This project compares three classification algorithms:
- Logistic Regression
- K-Nearest Neighbours (KNN)
- Naive Bayes

The workflow includes data preprocessing, exploratory data analysis (EDA), feature encoding, feature engineering, feature scaling, model training, and evaluation using Precision, Recall, F1 Score, and Accuracy.


## Objective

The objective of this project is to build a binary classification system that predicts whether a loan application will be approved based on applicant and loan-related features.

The project also compares the performance of Logistic Regression, KNN, and Naive Bayes using standard classification metrics.


## Dataset

The dataset contains information about loan applicants and their financial and demographic characteristics.

### Key Features

- Applicant Income
- Coapplicant Income
- Credit Score
- DTI Ratio
- Savings
- Loan Amount
- Loan Term
- Education Level
- Employment Status
- Marital Status
- Property Area
- Loan Purpose
- And other applicant-related features

### Target Variable

**Loan_Approved** — indicates whether the loan application was approved or not.


## Machine Learning Workflow

- Data preprocessing and missing value handling
- Exploratory Data Analysis (EDA)
- Categorical feature encoding
- Feature scaling using StandardScaler
- Model training using Logistic Regression, KNN, and Naive Bayes
- Model evaluation using Accuracy, Precision, Recall, and F1 Score
- Feature engineering and model comparison


## Model Results

| Model               | Accuracy | Precision | Recall | F1 Score |

| Logistic Regression | 86.5%    | 78.3%     | 77.0%  | 77.7%    |

| KNN                 | 76.0%    | 62.7%     | 52.5%  | 57.1%    |

| Naive Bayes         | 86.5%    | 80.4%     | 73.8%  | 76.9%    |

**Best model based on Precision:** Naive Bayes


## Feature Engineering

Additional features were created by squaring `DTI_Ratio` and `Credit_Score` to capture possible non-linear relationships.

The models were retrained after feature engineering and their performance was compared again.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure

```text
creditwise-loan-system/
├── creditwise_loan_prediction.ipynb
├── loan_approval_data.csv
├── README.md
└── .gitignore
```
