Health Insurance Cross-Sell Prediction

Project Overview
This project aims to build a classification model to predict whether a customer is interested in purchasing vehicle insurance provided by a company. The dataset used for this project was sourced from Kaggle and consists of approximately 400,000 rows and 12 columns.

Dataset Description
. Target Variable: Response (0 or 1) indicating whether a customer is interested in vehicle insurance.
. Independent Variables: Include features like Age, Gender, Driving License, Previously Insured, and more.
. Imbalance: The dataset was highly imbalanced, with the majority of responses being negative (0).

Project Workflow
Data Collection & Cleaning:

Collected the dataset from Kaggle.
Checked for null values and cleaned the dataset using Python's Pandas and Numpy libraries.
Exploratory Data Analysis (EDA):

Visualized the data to gain insights using Matplotlib and Seaborn.
Created new feature columns based on existing data.
Removed features that were not contributing significantly to the prediction.
Feature Engineering & Selection:

Conducted feature engineering to create meaningful features.
Performed hypothetical testing to ensure features' relevance.
Modeling:

Split the data into training and testing sets using train_test_split.
Addressed class imbalance using SMOTE (Synthetic Minority Over-sampling Technique).
Scaled numerical features using StandardScaler.
Implemented three different machine learning algorithms: Logistic Regression, Random Forest, and XGBoost.
Model Evaluation & Tuning:

Used cross-validation and hyperparameter tuning for each model.
Found that XGBoost performed the best with an ROC-AUC score of 84%.

Model Performance

Logistic Regression:

ROC-AUC: 0.7848
Precision, Recall, F1-Score: (Various metrics provided)

Random Forest:

ROC-AUC: 0.8032
Precision, Recall, F1-Score: (Various metrics provided)

XGBoost:

ROC-AUC: 0.8251
Precision, Recall, F1-Score: (Various metrics provided)

Conclusion

XGBoost was identified as the best-performing model with a mean ROC-AUC of 84%. The model effectively handles imbalanced data and provides robust predictions for the given problem.
