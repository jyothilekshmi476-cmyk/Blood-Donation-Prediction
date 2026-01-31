🩸 Blood Donation Eligibility & Next 6-Month Donation Prediction
📌 Project Overview

This Machine Learning project predicts whether a registered blood donor is likely to donate blood in the next 6 months using demographic details, health data, and past donation history. The model helps blood banks identify high-probability donors and improve outreach planning.

📊 Dataset

Source: Kaggle – Blood Donor Registry Dataset
Rows: 30,000
Columns: 27

Contains:
Donor personal details
Blood type & region
Health indicators
Donation history
Eligibility & deferral information
Target Variable: donated_next_6m

1 → Likely to donate

0 → Not likely to donate

🎯 Problem Statement

To build a classification model that predicts whether a donor will donate blood in the next 6 months based on their profile and past donation behavior. This supports better donor targeting and reduces failed outreach efforts.

🧠 Project Type

Binary Classification Problem

🔍 Workflow in Notebook

Library import
Dataset loading
Basic data inspection (head, tail, info, describe)
Missing value analysis
Categorical & numerical exploration
Correlation analysis
Feature reduction (dropped perfectly correlated columns)
Outlier handling (IQR method where needed)
Encoding categorical features
Feature scaling
Train/Test split
Model training
Model evaluation

⚙️ Libraries Used

pandas
numpy
matplotlib
seaborn
scikit-learn

🤖 Models Used

logistic regression
Decision Tree Classifier
Gradient Boosting Classifier
Tree-based ML models for classification

📈 Evaluation Metrics

Accuracy
F1 Score
precision
Classification metrics

Statistical comparison tests (t-test used between models)

🧹 Feature Engineering Notes

Highly correlated column removed:

years_since_first_donation dropped due to perfect correlation

Engineered score (donation_propensity_score) noted as optional baseline exclusion
Label Encoding applied to categorical features

💡 Real World Use Case

This model can help:
Blood banks identify likely donors
Reduce donor rejection rates
Plan targeted donation campaigns
Maintain stable blood supply
