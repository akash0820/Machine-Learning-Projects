# Customer Churn Prediction and Behavior Analysis

## Introduction

Customer churn is a critical challenge for streaming services, impacting profitability and growth. This project uses machine learning to predict churn and understand customer behavior, enabling actionable strategies for retention and revenue optimization.

## Data Description

### Dataset: 5,000 records, 12 features.
### Features:
Demographics: Age, Gender, Region.
Behavioral: Monthly Spend, Satisfaction Score, Last Activity.
Operational: Payment Method, Support Tickets Raised.
### Target Variables:
Churned: Binary indicator (1 = Yes, 0 = No).
Monthly Spend: Continuous variable.
### Challenges:
Missing Values: Age (500), Satisfaction Score (500).
Imbalanced Churn Distribution: ~30% churned customers.

## Problem Statement

Predict customers likely to churn.
Analyze factors influencing churn and spending behavior.
Provide actionable insights for improving retention and customer engagement.

## Approach and Methodology

### Regression Models:
Linear Regression: Baseline for predicting spending.
Random Forest Regressor: Non-linear relationships and feature importance.
### Classification Models:
Logistic Regression: Interpretable binary classification.
Random Forest Classifier: Highest performance for churn prediction.
K-Nearest Neighbors (KNN): Captures neighborhood-based patterns.

## Results and Performance

### Regression:
R2 for Linear Regression: 0.934.
Random Forest Regressor identified key spending predictors: Satisfaction Score, Discount Offered.
### Classification:
Random Forest Classifier: Accuracy 83%, AUC 0.88.
Key churn predictors: Satisfaction Score, Last Activity.
### Insights:
Discounts can lead to higher churn if not strategically applied.
Low satisfaction scores strongly correlate with churn.

## Business Impact

Targeted Retention: Identify at-risk customers and personalize retention strategies.
Customer Segmentation: Segment customers based on predicted spend and churn likelihood.
Process Optimization: Optimize customer support based on ticket patterns.

## Challenges and Limitations

### Missing Data:
Age and Satisfaction Score required imputation.
Recommendation: Improve data collection processes to ensure completeness.
### Class Imbalance:
Resampling techniques were employed to address imbalance in churn data.
Recommendation: Explore additional techniques like SMOTE or weighted models.

## How to Use

### Prerequisites
Python 3.7+ with the following libraries:
pandas, numpy, scikit-learn, matplotlib, seaborn.

## Directory Structure
```
├── data/
│   ├── Streaming.csv                  # Raw dataset
├── notebooks/
│   ├── Streaming.ipynb                # Python Code
├── Documents/
│   ├── Streaming-final.pptx           # Presentation 
│   ├── Final Report- ML-Group10.pdf   # Report
├── README.md                          # Project README
```
## Future Work

Incorporate time-series analysis for customer engagement trends.
Explore additional features like device usage and content preferences.
Deploy models in production to generate real-time predictions.

## Authors and Acknowledgments

Akash Anand, Arjun Sreekumar, Ayantika Chatterjee, Taranjeet Kamboj.
Special thanks to the Streaming Service Dataset for providing the data.
