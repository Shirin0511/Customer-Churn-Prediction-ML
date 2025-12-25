# Customer Churn Prediction  
## Machine Learning Classification with Explainability (SHAP)


## Project Overview
This project was built to predict whether a customer is likely to churn and, more importantly, to explain **why** a customer is predicted to churn using **SHAP (SHapley Additive exPlanations)**.

The outcome enables **data-driven retention strategies** rather than relying on black-box predictions.

## Problem Statement
- Identify customers at high risk of churn  
- Handle imbalanced classification  
- Move beyond accuracy to business-relevant metrics  
- Provide model explainability to support actionable decision-making  


## Solution Highlights
- Built two classification models: **Logistic Regression** and **Random Forest**
- Addressed class imbalance
- Evaluated models using robust performance metrics
- Applied **SHAP explainability** for global and local insights
- Converted model predictions into **business-level insights**


## Machine Learning Workflow

### 1. Data Understanding & Cleaning
- Analysed customer demographics, service usage, and billing information  
- Handled missing values and corrected data types  
- Removed inconsistencies affecting model performance  

### 2. Exploratory Data Analysis (EDA)
- Identified churn patterns across:
  - Contract type  
  - Tenure  
  - Monthly charges  
  - Payment methods  
- Visualized churn vs non-churn customer behaviour  

### 3. Feature Engineering & Preprocessing
- One-hot encoded categorical variables  
- Scaled numerical features where required  
- Prepared model-ready datasets  

### 4. Model Training
Implemented and compared:
- **Logistic Regression** (baseline, interpretable)  
- **Random Forest Classifier** (non-linear, high performance)  

### 5. Hyperparameter Tuning
- Used **GridSearchCV**
- Optimized models for **recall** and **ROC-AUC** to reduce false negatives  


## Model Evaluation
Models were evaluated using metrics suitable for imbalanced datasets:
- ROC-AUC  
- Precision  
- Recall  
- F1-Score  
- Confusion Matrix  

### Key Insight
The **Random Forest model** achieved stronger generalization and recall, making it more suitable for churn prediction where missing a churner is costly.


## Model Explainability with SHAP
To ensure transparency and trust:
- **Global explainability**: Identified top churn-driving features  
- **Local explainability**: Explained individual customer predictions  

Visualizations included:
- Feature importance  
- Direction of impact  
- Customer-level decision paths  

### Business Value
Stakeholders can understand **why** a customer is at risk and take targeted retention actions.


## Key Insights
- Customers on **month-to-month contracts** are significantly more likely to churn  
- **High monthly charges combined with low tenure** strongly correlate with churn  
- Contract length and payment method are major churn drivers  


## Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- SHAP  

---
