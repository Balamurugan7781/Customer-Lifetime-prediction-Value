# Customer-Lifetime-prediction-Value
Designed for the purpose of finding out the targeted customers for the bank to reduce their marketing cost


## Overview

This project develops a machine learning system to predict whether bank customers are likely to subscribe to a term deposit product based on historical marketing campaign data.

The solution helps financial institutions:
- Improve customer targeting
- Reduce marketing costs
- Increase conversion rates
- Enhance customer lifetime value (CLV)
- Optimize marketing ROI

The project includes:
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Imbalanced Classification Handling
- Model Comparison & Evaluation
- Business Impact Analysis
- Flask API Deployment

## Business Problem

Traditional bank marketing campaigns contact all customers without prioritization, resulting in:
- High marketing costs
- Low conversion efficiency
- Poor resource allocation

The objective of this project is to build a predictive machine learning model capable of identifying customers who are most likely to subscribe to a term deposit product.

By targeting high-potential customers, the bank can:
- Improve marketing efficiency
- Reduce operational costs
- Increase conversion rates
- Improve long-term customer value

## Dataset Information

- Source: UCI Bank Marketing Dataset
- Records: 41,188 customers
- Target Variable: Subscription to term deposit (`yes/no`)

### Features Include:
- Age
- Job
- Marital status
- Education
- Contact type
- Campaign information
- Previous marketing interactions
- Economic indicators

## Tech Stack

### Languages
- Python

### Libraries
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn
- Matplotlib
- Seaborn
- XGBoost

### Deployment
- Flask API
- Pickle

### Tools
- Jupyter Notebook
- GitHub

## Machine Learning Wokflow

1. Data Cleaning
2. Exploratory Data Analysis (EDA)
3. Feature Engineering
4. Handling Imbalanced Data
5. Model Training
6. Hyperparameter Tuning
7. Model Evaluation
8. Business Impact Analysis
9. Model Deployment using Flask API

## Imbalanced Data Handling

The dataset was highly imbalanced, where positive subscription cases represented a minority class.

To address this issue:
- Random Oversampling was implemented
- Class weights were applied
- Evaluation focused on:
  - F1 Score
  - AUC-PR
  - AUC-ROC
  - Precision
  - Recall

This improved the model’s ability to identify potential subscribers effectively.

## Models Evaluated

The following machine learning models were tested:

- Logistic Regression
- Random Forest
- Decision Tree
- Gradient Boosting Machine (GBM)
- XGBoost
- Support Vector Machine (SVM)
- KNN
- Naive Bayes

A total of 22 models were evaluated with different imbalance-handling strategies.

## Final Selected Model

### Gradient Boosting Machine (GBM) + Random Oversampling

The final selected model achieved strong performance on imbalanced classification metrics:

| Metric | Score |
|---|---|
| Precision | 44.5% |
| Recall | 86.4% |
| AUC-PR | 0.582 |
| F1 Score | Strong Balanced Performance |

The model was selected because it provided the best balance between identifying potential subscribers and minimizing marketing waste.

## Business Impact

### Marketing Cost Reduction
- Traditional Campaign Cost: $82,376
- Targeted Campaign Cost: $17,982
- Cost Reduction: 78.18%

### ROI Improvement
- Without Model ROI: 463%
- With Predictive Model ROI: 2127%

### Customer Targeting
- Predicted high-potential subscribers: 8,991
- Correctly identified subscribers: ~4,004

The predictive system enables highly targeted marketing campaigns, improving customer acquisition efficiency and maximizing Customer Lifetime Value (CLV).

## Flask API Deployment

The trained model was deployed using Flask API.

### API Workflow
1. Upload CSV containing customer features
2. API processes the data
3. Model generates predictions
4. Predictions are returned as JSON response

This enables real-time prediction capability for integration into banking systems.

## Installation

```bash
git clone https://github.com/Balamurugan7781/customer-lifetime-prediction-Value.git

cd customer-lifetime-prediction-Value

pip install -r requirements.txt
```



---

## Future Improvements

This makes the project look mature.

```markdown
## Future Improvements

- Deploy using Docker
- Cloud deployment using AWS/GCP
- Real-time prediction pipeline
- SHAP explainability integration
- Customer segmentation integration
- Streamlit dashboard
- Automated retraining pipeline
```

## Results

ROC Curve for Gradient Boosting Machine Model (GBM)
<img width="574" height="421" alt="image" src="https://github.com/user-attachments/assets/d594698c-a6cb-42bd-9863-d981e51bc7ca" />

PR curve for Gradient Boosting Machine Model (GBM)
<img width="572" height="370" alt="image" src="https://github.com/user-attachments/assets/ba679e62-c788-4548-aed0-a21477672cd7" />


## Badges
![Python](https://img.shields.io/badge/Python-3.10-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![Flask](https://img.shields.io/badge/Flask-API-black)
![License](https://img.shields.io/badge/License-MIT-green)


