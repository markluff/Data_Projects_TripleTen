# Sprint 17: Customer Churn Prediction

## 📌 Table of Contents
- [Introduction](#introduction)
- [Process](#process)
- [Model Comparisons](#model-comparisons)
- [Conclusion & Recommendations](#conclusion--recommendations)

---

## 🏆 Introduction
Interconnect tasked me with creating a **predictive model** to identify customers most likely to **cancel their services**. The goal was to analyze customer data, handle class imbalance, and implement machine learning models to accurately predict churn.

---

## 🔬 Process
### Data Preparation
Interconnect provided **four different CSV files**, which required extensive **cleaning and merging**. The dataset included **begin and end date columns**, allowing me to calculate **contract length** and **churn status**. Customers **without an end date** were considered **active users**. After processing, the dataset contained **7,000 observations**, with **26.5% representing churned customers**.

### Handling Class Imbalance
Since the dataset was **imbalanced**, I employed **SMOTE (Synthetic Minority Over-sampling Technique)** to increase the number of churned customer samples. This strategy interpolates between existing observations to generate synthetic data, reducing the risk of overfitting while improving model performance.

### Feature Engineering & Encoding
Most of the dataset contained **categorical variables**, requiring **One-Hot Encoding** to convert them into numerical format for machine learning models.

---

## 📊 Model Comparisons
I implemented four different machine learning models and evaluated their **AUC-ROC scores**:

1. **Random Forest Classifier**: Achieved an AUC-ROC score of **0.86**. This model showed strong predictive power but was outperformed by others.
2. **Logistic Regression**: Performed the worst, achieving an AUC-ROC score of **0.81**. Due to its lower predictive accuracy, this model is **not recommended**.
3. **LightGBM (Gradient Boosting)**: **Top performer** with an AUC-ROC score of **0.90**. This model was not only accurate but also computationally efficient.
4. **XGBoost Classifier**: Delivered a solid performance with an **AUC-ROC score of 0.88**, making it another viable option.

---

## ✅ Conclusion & Recommendations
### 🔹 Best Model: **LightGBM**
Based on performance metrics, I recommend **Interconnect use the LightGBM model** for predicting customer churn. This model offers **high accuracy (AUC-ROC: 0.90)** and is computationally **efficient for large datasets**.

### 🔹 Key Insights
- **Most important churn indicators (LightGBM model)**:
  - **Contract Length**
  - **Monthly Charges**
  - **Total Charges**
- **XGBoost found another significant predictor**:
  - **Electronic Check Payment Method** accounted for **40% of predictive weight**. Further investigation into potential billing issues with e-check payments is advised.
- **Random Forest model insights**:
  - Additional factors such as **Fiber Optic Services** and **Total Charges** were important predictors of churn.

### 🔹 Next Steps for Interconnect
- **Investigate customer concerns** related to **contract length, pricing models, and payment methods**.
- **Optimize service offerings** for customers in high-risk churn categories.
- **Monitor and improve billing processes**, especially for **electronic check users**.

🚀 **Future Work:** Additional hyperparameter tuning and testing alternative ensemble models could further improve predictive accuracy.

