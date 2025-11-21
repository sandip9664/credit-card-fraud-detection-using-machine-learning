# Credit Card Fraud Detection

This project aims to develop and evaluate machine learning models for credit card fraud detection using a highly imbalanced dataset. The primary goal is to maximize the detection of fraudulent transactions (high recall) while maintaining overall model performance.

## Project Overview

-   **Dataset**: Utilizes a dataset of credit card transactions featuring PCA-transformed `V` features, `Time`, `Amount`, and a binary `Class` target (0: non-fraud, 1: fraud).
-   **Challenge**: Addressed severe class imbalance (0.1727% fraudulent transactions).
-   **Preprocessing**: Data split with stratification, followed by feature scaling using `StandardScaler`.
-   **Models Evaluated**: Logistic Regression, Random Forest Classifier, and XGBoost Classifier were implemented. 
-   **Evaluation Metrics**: Prioritized Recall, Precision, F1-score, Confusion Matrix, and AUC-ROC score due to dataset imbalance.
-   **Hyperparameter Tuning**: `GridSearchCV` was applied to optimize the XGBoost model for `roc_auc`.

## Key Findings

-   **XGBoost Classifier** emerged as the most suitable model, demonstrating the best balance of high `Recall` for fraudulent transactions and a superior `AUC-ROC` score after hyperparameter tuning. This makes it effective in identifying fraud within this imbalanced financial dataset.

This project highlights practical approaches to tackling fraud detection with imbalanced data, emphasizing robust model evaluation and optimization.
