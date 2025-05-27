# Customer Churn Prediction: Evaluation and Predictions

## 📌 Table of Contents
- [Introduction](#introduction)
- [Pre-Processing Methods](#pre-processing-methods)
- [Balancing Methods](#balancing-methods)
- [Models Used](#models-used)
- [Findings and Conclusion](#findings-and-conclusion)

---

## 🏆 Introduction
Beta Bank is facing a **customer churn problem** that can be addressed through **research and machine learning**. Using a dataset of **10,000 customers**, I built a model to **predict which clients are at risk of leaving the bank**. The goal was to determine the most effective model for accurate churn prediction.

---

## 🔬 Pre-Processing Methods
To prepare the data for machine learning, I performed several **pre-processing steps**:
1. **Removed irrelevant columns** to streamline model training.
2. **Converted categorical data to numerical values** using **One-Hot Encoding**.
3. **Split the dataset** into **training, validation, and test sets**.
4. **Scaled the numerical data** to normalize feature distributions.

These steps ensured the data was properly formatted and optimized for machine learning models.

---

## 📊 Balancing Methods
Since the dataset had an **imbalance in churned vs. non-churned clients**, I tested two methods to improve model performance:
1. **Upsampling** - Increased the number of churn observations to balance the dataset.
2. **Class Weight Parameter** - Adjusted model weights to give higher importance to the underrepresented class.

**Findings:** The **upsampling method** produced higher **F1 scores**, suggesting it was the more effective approach for predicting churn.

---

## 🎯 Models Used
I trained and compared the performance of **three classification models**:
1. **Decision Tree**
2. **Logistic Regression**
3. **Random Forest**

Each model's performance was evaluated based on the **F1 score**, a balance between precision and recall.

---

## 🔍 Findings and Conclusion
The **Random Forest model** achieved the highest **F1 score**, making it the most effective choice for predicting customer churn.

### **F1 Scores:**
- **Decision Tree** = **0.721**
- **Logistic Regression** = **0.640**
- **Random Forest** = **0.732**

Since the **Random Forest model** provided the best balance of precision and recall, **Beta Bank should use this model** to identify at-risk clients.

### **Key Insights:**
- **Age** was the most important feature in predicting churn.
- **50% of customers who left** were between **46-60 years old**, and another **25%** were in the **61-75 age range**.

### **Recommendations:**
- Beta Bank should **investigate the needs** of clients aged **46-75**.
- Develop targeted **products and services** to retain this demographic.
- Conduct additional **customer surveys and market research** to enhance retention strategies.

🚀 **Future Work:** Exploring alternative feature engineering techniques, testing additional models, and optimizing hyperparameters may further improve churn predictions.

