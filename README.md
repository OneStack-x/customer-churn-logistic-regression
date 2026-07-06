# Customer Churn Prediction using Logistic Regression

## Overview

This project predicts whether a telecom customer will churn using a Logistic Regression model.

The project covers the complete machine learning workflow, from data preprocessing to model evaluation using the IBM Telco Customer Churn dataset.

---

## Dataset

- IBM Telco Customer Churn Dataset
- 7,043 customer records
- Binary classification problem
- Target variable: **Churn**

---

## Project Workflow

### 1. Data Loading

- Loaded the dataset using `kagglehub`
- Read the CSV file with pandas

### 2. Data Exploration

Performed basic exploration using:

- Dataset shape
- Column names
- Data types
- Summary statistics
- Missing values
- Duplicate rows
- Class distribution

### 3. Data Cleaning

- Removed the `customerID` column
- Converted `TotalCharges` to numeric
- Removed rows containing missing values
- Encoded the target variable:
  - No → 0
  - Yes → 1

### 4. Exploratory Data Analysis (EDA)

Created visualizations for:

- Customer churn distribution
- Contract type vs churn
- Correlation matrix

### 5. Data Preprocessing

- Separated features and target
- Applied One-Hot Encoding using `pd.get_dummies()`
- Split the dataset into training and testing sets
- Standardized numerical features using `StandardScaler`

### 6. Model Training

Trained a Logistic Regression model using:

- `random_state=42`
- `max_iter=10000`

### 7. Model Evaluation

Evaluated the model using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC Curve

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- scikit-learn
- kagglehub

---

## Repository Contents

```
customer_churn_logistic_regression.ipynb
README.md
```

---

## Future Improvements

- Hyperparameter tuning with GridSearchCV
- Cross-validation
- Feature importance analysis
- Save the trained model using Joblib
- Deploy the model with FastAPI or Streamlit

---
