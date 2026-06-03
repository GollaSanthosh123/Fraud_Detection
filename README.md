# Credit Risk Modeling and Loan Default Prediction

## Project Overview

This project develops an end-to-end Credit Risk Modeling system to predict the likelihood of loan default using customer demographic information, loan details, and credit bureau data.

The solution combines advanced feature engineering, statistical risk assessment techniques, machine learning modeling, and business intelligence visualization to help financial institutions make data-driven lending decisions and minimize credit losses.

---

## Business Problem

Financial institutions face significant risks when approving loans to customers with uncertain repayment behavior.

The objective of this project is to:

- Predict whether a customer is likely to default on a loan.
- Identify key factors influencing credit risk.
- Improve loan approval decisions.
- Reduce financial losses from high-risk borrowers.
- Support risk analysts through interactive dashboards and reports.

---

## Dataset

The project utilizes multiple datasets containing:

### Customer Information
- Age
- Gender
- Occupation
- Income
- Employment Status
- Marital Status

### Loan Information
- Loan Amount
- Interest Rate
- Loan Tenure
- Loan Type
- EMI Details

### Credit Bureau Information
- Existing Loans
- Credit History Length
- Delinquencies
- Credit Utilization
- Previous Defaults

### Target Variable
- Loan Default Status
  - 0 = Non-Default
  - 1 = Default

---

## Project Workflow

### 1. Data Collection

Collected and integrated customer, loan, and bureau datasets from multiple sources.

### 2. Data Cleaning

- Missing value treatment
- Duplicate removal
- Outlier detection
- Data validation checks
- Data type corrections

### 3. Exploratory Data Analysis (EDA)

Performed detailed analysis to understand:

- Default distribution
- Income vs Default Rate
- Loan Amount vs Risk
- Credit Score Analysis
- Correlation Analysis

#### Key Visualizations

- Histograms
- Boxplots
- Heatmaps
- Risk Distribution Charts
- Default Rate Analysis

---

### 4. Feature Engineering

Created risk-based features including:

- Debt-to-Income Ratio
- Credit Utilization Ratio
- Loan-to-Income Ratio
- Delinquency Count
- Average Credit Age

Applied:

- One-Hot Encoding
- Label Encoding
- Scaling and Normalization

---

### 5. Statistical Risk Analysis

Implemented industry-standard credit risk techniques.

#### Weight of Evidence (WOE)

Used to transform categorical variables into predictive numerical representations while preserving risk relationships.

#### Information Value (IV)

Measured predictive power of variables and assisted in feature selection.

| IV Range | Predictive Power |
|-----------|-----------------|
| < 0.02 | Not Useful |
| 0.02 - 0.10 | Weak |
| 0.10 - 0.30 | Medium |
| 0.30 - 0.50 | Strong |
| > 0.50 | Suspicious |

#### Kolmogorov-Smirnov (KS) Statistic

Evaluated the model's ability to distinguish between good and bad borrowers.

---

## Machine Learning Models

The following models were evaluated:

- Logistic Regression
- Random Forest
- XGBoost

### Final Model: XGBoost Classifier

Reasons for selection:

- Handles imbalanced datasets effectively
- Strong predictive performance
- Robust against overfitting
- Supports feature importance analysis
- Suitable for credit risk applications

---

## Hyperparameter Optimization

Used **Optuna** for automated hyperparameter tuning.

Optimized parameters:

- Learning Rate
- Max Depth
- Number of Estimators
- Subsample Ratio
- Column Sampling Ratio
- Regularization Parameters

---

## Model Performance

| Metric | Score |
|----------|----------|
| Accuracy | 85% - 90% |
| Precision | High |
| Recall | High |
| F1-Score | High |
| ROC-AUC | Excellent |
| KS Score | Strong |

---

## Technology Stack

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Optuna

### Dashboarding
- Streamlit

### Database
- MySQL

### Version Control
- Git
- GitHub

---

## Streamlit Dashboard Features

### Customer Risk Analysis
- Individual Risk Score
- Probability of Default
- Customer Profile Insights

### Portfolio Monitoring
- High Risk Customers
- Medium Risk Customers
- Low Risk Customers

### Business Insights
- Default Trends
- Feature Importance
- Risk Distribution

### Model Monitoring
- ROC Curve
- Confusion Matrix
- Accuracy Metrics
- KS Statistics

---

## Project Structure

```text
Credit-Risk-Modeling/
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── notebooks/
│   ├── EDA.ipynb
│   ├── Feature_Engineering.ipynb
│   ├── Model_Training.ipynb
│
├── src/
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   ├── model_training.py
│   ├── model_evaluation.py
│
├── models/
│   ├── xgboost_model.pkl
│
├── dashboard/
│   ├── app.py
│
├── outputs/
│   ├── figures/
│   ├── reports/
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/Credit-Risk-Modeling.git
```

### Navigate to Project Folder

```bash
cd Credit-Risk-Modeling
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Streamlit Dashboard

```bash
streamlit run dashboard/app.py
```

---

## Results

- Developed a complete credit risk prediction pipeline.
- Applied WOE, IV, and KS statistical techniques for risk assessment.
- Built and optimized an XGBoost model achieving approximately 85–90% prediction accuracy.
- Identified key drivers of loan default.
- Created an interactive Streamlit dashboard for business users and stakeholders.
- Enabled data-driven lending and risk management decisions.

---

## Future Enhancements

- SHAP Explainable AI Integration
- Real-Time Credit Scoring API
- AWS/Azure Deployment
- Automated Model Monitoring
- Portfolio Risk Forecasting
- MLOps Pipeline Integration

---

## Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Credit Risk Analytics
- WOE & IV Analysis
- KS Statistics
- Machine Learning
- Hyperparameter Tuning
- XGBoost
- Optuna
- Streamlit
- Business Intelligence
- Model Evaluation

---

## Author

### Golla Santhosh

**Data Analyst | Machine Learning Enthusiast**

- LinkedIn: https://www.linkedin.com/in/golla-santhosh-a06231300
- GitHub: https://github.com/GollaSanthosh123

---

⭐ If you found this project useful, consider giving it a star on GitHub.
