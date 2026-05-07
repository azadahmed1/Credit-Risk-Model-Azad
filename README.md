# Credit-Risk-Model-Azad

Project Overview

This project focuses on building an end-to-end Machine Learning solution for predicting loan default risk using customer, loan, and bureau datasets. The objective was to develop a highly reliable classification model that can identify high-risk customers while meeting business requirements for recall.

The project includes:

Data preprocessing
Feature engineering
Feature selection using WOE/IV and VIF
Handling class imbalance
Model training and evaluation
Threshold optimization
Model deployment using Streamlit
Business Problem

Financial institutions face significant losses due to loan defaults. The objective of this project was to build a predictive system capable of identifying potential defaulters with high recall so that risky applications can be flagged early.

Dataset Information

The project used three separate datasets:

Customer Data
Loan Data
Bureau Data

After merging the datasets:

Total Records: 50,000+
Target Variable: Default (Yes/No)
Project Workflow
1. Data Preprocessing
Merged multiple datasets using Pandas
Performed train-test split before preprocessing to avoid data leakage
Handled missing values using mode imputation
Removed duplicate entries
Treated outliers using business thresholds
Standardized inconsistent categorical values
2. Exploratory Data Analysis
Boxplots for outlier visualization
Histograms for distribution analysis
KDE plots for business insights
Target distribution analysis for imbalance detection
3. Feature Engineering

Created business-driven features such as:

Loan-to-Income Ratio
Delinquency Ratio
Average DPD per Delinquency
4. Feature Selection
Variance Inflation Factor (VIF)
Weight of Evidence (WOE)
Information Value (IV)
5. Models Used
Logistic Regression
Random Forest Classifier
XGBoost Classifier
6. Imbalance Handling
Random Under Sampling
SMOTE Oversampling
7. Hyperparameter Optimization
Optuna
Threshold Tuning using predicted probabilities
Model Performance
Final Selected Model: Logistic Regression
Key Results
Recall Achieved: 94%
Business Requirement: 90% Recall
Strong ROC-AUC Performance
Effective Rank Ordering and KS Statistics
Business Impact
83% of default cases captured in top decile
Improved risk identification capability
Better precision after threshold optimization
Deployment

The final model and scaler were exported using Joblib and deployed using Streamlit.

Streamlit Application

Lauki Finance: Credit Risk Modelling · Streamlit
GitHub Repository

azadahmed1/Credit-Risk-Model-Azad: Credit Risk Model prediction project

Tech Stack
Python
Pandas
NumPy
Scikit-learn
XGBoost
Optuna
Matplotlib
Seaborn
Streamlit
Key Learnings
Importance of handling class imbalance
Business-focused evaluation metrics
Threshold optimization for recall improvement
Feature engineering in financial risk modeling
End-to-end ML deployment workflow
Author

Azad Ahmed Machine Learning Engineer
