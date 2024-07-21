# Telecom Customer Churn Prediction

## Overview
The goal of this project is to predict customer churn in a telecommunications company using artificial neural network. The dataset includes various customer attributes, and the goal is to identify customers who are likely to leave the service.

## Dataset
- [The dataset](https://www.kaggle.com/datasets/yeanzc/telco-customer-churn-ibm-dataset/data)

The dataset Telco_customer_churn.xlsx contains information about telecom customers, including various demographic, account, and service-related features. 

## Data Preprocessing
- Handled missing values.
- Dropped irrelevant features.
- Encoded categorical features using one-hot encoding and binary encoding for binary features.
- Scaled numeric features to a range of 0 to 1.
- Used SMOTE to balance the dataset by generating synthetic samples for the minority class.

## Model Building
- Model Architecture: Built a Sequential neural network model with the following layers:
    - Dense layer with 100 units and ReLU activation
    - Dropout layer with 30% dropout rate
    - Dense layer with 50 units and ReLU activation
    - Dropout layer with 30% dropout rate
    - Dense layer with 20 units and ReLU activation
    - Dropout layer with 30% dropout rate
    - Output Dense layer with 1 unit and sigmoid activation
- Optimizer: Adam optimizer with learning rate 0.001
- Loss Function: Binary cross-entropy

## Evaluation
- Performance Metrics: The model's performance is evaluated using accuracy, precision, recall, F1 score, and confusion matrix.
- Threshold Adjustment: The threshold was adjusted to 0.4 to improve recall for the churn class.

## Libraries To run the notebook:
- pandas
- matplotlib
- seaborn
- scikit-learn
- tensorflow
- imblearn
