# financial-fraud-detection
Machine learning analysis and fraud detection using Kaggle financial transactions dataset
## Dataset
This project uses the Financial Fraud Dataset from Kaggle.

Due to licensing, the dataset is not included in this repository.
You can download it here: https://www.kaggle.com/datasets/umitka/synthetic-financial-fraud-dataset
## Objective
- Identify fraudulent transactions in a large, imbalanced financial dataset.
- Apply feature engineering and machine learning to flag fraud.
- Evaluate using ROC-AUC and Precision–Recall curves.

---

## Key Steps
1. **Data Cleaning & Exploration**
   - Handle missing values and duplicates
   - Analyze distribution of fraud vs non-fraud
2. **Feature Engineering**
   - Amount-to-balance ratio
   - Destination balance change
3. **Modeling**
   - Random Forest Classifier
   - Train/Test split
4. **Evaluation**
   - Precision, Recall, F1-score
   - ROC-AUC curve
   - Precision–Recall curve
5. **Business Insights**
   - Fraud concentrated in `TRANSFER` and `CASH_OUT` transactions
   - Balance inconsistencies indicate fraudulent behavior

---

## Results
- **ROC-AUC:** 0.9988
- **Average Precision (AP):** 0.9976
- Near-perfect classification due to clear patterns in synthetic dataset.

### Key Insights
- Fraud is rare but highly predictable with engineered features.
- Balance inconsistencies and abnormal amounts are strong fraud indicators.
- The model can guide real-world fraud monitoring systems.

---

## Tools & Libraries
- Python 3.14.1
- Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- Google Colab for development

---
- Test with real-world datasets to ensure robustness
- Implement SHAP for explainability
- Develop a dashboard for real-time fraud monitoring
