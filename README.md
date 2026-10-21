# Customer Churn Prediction Using Machine Learning

## Overview
This project focuses on predicting customer churn — identifying customers who may stop using a service. It uses machine learning to classify customers based on their likelihood of leaving and explores how prediction thresholds can be adjusted to reduce potential business costs.

## Objectives
- Analyze customer data and explore patterns associated with churn.
- Preprocess data for machine learning.
- Train and compare machine learning models.
- Evaluate the selected model using classification metrics.
- Tune the classification threshold based on estimated business costs.

## Dataset
The project uses the **Telco Customer Churn** dataset.

Dataset source: [Telco Customer Churn — Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

The dataset contains customer information and a churn label indicating whether a customer left the service.

## Methodology
1. Data loading and cleaning
2. Exploratory data analysis (EDA)
3. Data preprocessing
4. Training and comparing machine learning models
5. Hyperparameter tuning using GridSearchCV
6. Final test-set evaluation
7. Classification threshold tuning using estimated business costs

## Model Evaluation
The selected model in the notebook is a **HistGradientBoosting classifier**, optimized using GridSearchCV.

The notebook evaluates the model using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Average Precision (PR-AUC)
- Confusion matrix
- ROC and Precision–Recall curves

## Business-Cost-Based Threshold Tuning
The project examines different classification thresholds to minimize an estimated cost:

- False Negative (missed churn customer): $1,000
- False Positive (incorrect churn prediction): $50

The threshold analysis compares estimated financial cost, recall, and precision to identify a cost-minimizing threshold.

These cost values are assumptions used for the analysis, not verified real-world business costs.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

## Project File
- `Customer_churn_prediction.ipynb` — notebook containing the analysis, model evaluation, and threshold tuning.

## Conclusion
This project demonstrates a machine learning workflow for customer churn prediction, combining model evaluation with business-cost-based threshold analysis to support customer retention decisions.
