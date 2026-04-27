# Credit Card Fraud Detection
This project applied machine learning approaches for detecting fraudulent credit card transactions in highly imbalanced datasets.

## Models Used
- Random Forest
- XGBoost (My Contribution)
- Autoencoder

## Contribution (XGBoost)
Implementing and evaluating the XGBoost model, including:
- Data preprocessing and feature engineering
- Model training and tuning
- Performance evaluation using recall and F1-score

## 📊 Model Performance Comparison

| Dataset | Model | Recall (Fraud) | F1 Score (Fraud) | ROC-AUC | Key Insight |
|--------|------|---------------|------------------|--------|------------|
| Synthetic (Raw) | Random Forest | 0.01 | 0.01 | 0.975 | Failed fraud detection |
| Synthetic (Raw) | XGBoost | 0.45 | 0.61 | 0.724 | Limited performance |
| Synthetic (Raw) | Autoencoder | 0.63 | 0.04 | 0.714 | Low precision |
| Cleaned Dataset | Random Forest | 0.02 | 0.04 | 0.987 | |
| Cleaned Dataset | XGBoost | 0.47 | 0.62 | 0.733 | Slight improvement |
| Cleaned Dataset | Autoencoder | 0.59 | 0.03 | 0.695 | |
| Feature Engineered | Random Forest | 0.64 | 0.77 | 0.988 | Improved |
| Feature Engineered | XGBoost | 0.82 | 0.88 | 0.908 | Best performance |
| Feature Engineered | Autoencoder | 0.60 | 0.03 | 0.701 | |
| European Dataset | Random Forest | 0.71 | 0.82 | 0.933 | Strong |
| European Dataset | XGBoost | 0.83 | 0.89 | 0.915 | Best overall |
| European Dataset | Autoencoder | 0.56 | 0.63 | 0.941 | |

**Key results:** Feature engineering significantly improves fraud detection performance, and XGBoost consistently achieved the best results.
