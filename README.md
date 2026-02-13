# 🩸 Blood Donation Eligibility & Next 6-Month Donation Prediction

## 📌 Project Overview
- This Machine Learning project predicts whether a registered blood donor is likely to donate blood in the next 6 months.
- The prediction is based on demographic details, health data, and past donation history.
- The model helps blood banks identify high-probability donors and improve outreach planning.

## 📊 Dataset
- Source: Kaggle – Blood Donor Registry Dataset
- Rows: 30,000
- Columns: 27

### Dataset Contains
- Donor personal details
- Blood type and region
- Health indicators
- Donation history
- Eligibility and deferral information

### Target Variable
- `donated_next_6m`
  - 1 → Likely to donate
  - 0 → Not likely to donate

## 🎯 Problem Statement
- Build a classification model to predict whether a donor will donate blood in the next 6 months
- Use donor profile and past donation behavior
- Support better donor targeting and reduce failed outreach efforts

## 🧠 Project Type
- Binary Classification Problem

## 🔍 Workflow in Notebook
- Library import
- Dataset loading
- Basic data inspection (`head`, `tail`, `info`, `describe`)
- Missing value analysis
- Categorical and numerical exploration
- Correlation analysis
- Feature reduction (perfectly correlated columns removed)
- Outlier handling (IQR method where required)
- Encoding categorical features
- Feature scaling
- Train/Test split
- Model training
- Model evaluation

## ⚙️ Libraries Used
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## 🤖 Models Used
- Logistic Regression
- Decision Tree Classifier
- Gradient Boosting Classifier
- Tree-based machine learning models

## 📈 Evaluation Metrics
- Accuracy
- F1 Score
- Precision
- Classification report
- Statistical comparison tests (t-test between models)

## 🧹 Feature Engineering Notes
- Highly correlated column removed:
  - `years_since_first_donation` (perfect correlation)
- Engineered feature:
  - `donation_propensity_score` (optional baseline exclusion)
- Label Encoding applied to categorical features

## 💡 Real World Use Case
- Identify donors who are likely to donate
- Reduce donor rejection rates
- Plan targeted donation campaigns
- Maintain a stable blood supply
