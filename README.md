# Credit Card Fraud Detection - XGBoost
This project applies machine learning techniques to detect fraudulent credit card transactions in an imbalanced datasets.

## Models Used
- Random Forest
- XGBoost (My Contribution)
- Autoencoder

## Contribution for XGBoost
Implementing and evaluating the XGBoost model, including:
- Data preprocessing and feature engineering
- Model training and tuning
- Performance evaluation using recall and F1-score

## 📊 Model Performance Comparison

| Dataset | Model | Recall (Fraud) | F1 Score (Fraud) | ROC-AUC | Key Insight |
|--------|------|---------------|------------------|--------|------------|
| Synthetic (Raw) | Random Forest | 0.01 | 0.01 | 0.975 | High accuracy but failed to detect fraud |
| Synthetic (Raw) | XGBoost | 0.45 | 0.61 | 0.724 | Better fraud detection but still limited |
| Synthetic (Raw) | Autoencoder | 0.63 | 0.04 | 0.714 | Detected fraud but very low precision |
| Cleaned Dataset | Random Forest | 0.02 | 0.04 | 0.987 | Slight improvement but still weak |
| Cleaned Dataset | XGBoost | 0.47 | 0.62 | 0.733 | Minor improvement after cleaning |
| Cleaned Dataset | Autoencoder | 0.59 | 0.03 | 0.695 | Slight improvement but still unstable |
| Feature Engineered | Random Forest | 0.64 | 0.77 | 0.988 | Significant improvement with better features |
| Feature Engineered | XGBoost | 0.82 | 0.88 | 0.908 | Best overall performance |
| Feature Engineered | Autoencoder | 0.60 | 0.03 | 0.701 | Still limited performance |
| European Dataset | Random Forest | 0.71 | 0.82 | 0.933 | Strong performance on real dataset |
| European Dataset | XGBoost | 0.83 | 0.89 | 0.915 | Best fraud detection overall |
| European Dataset | Autoencoder | 0.56 | 0.63 | 0.941 | Balanced but weaker than XGBoost |
