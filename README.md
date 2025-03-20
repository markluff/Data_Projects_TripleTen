# Data Projects: TripleTen Repository

## 📌 Table of Contents
- [Introduction](#introduction)
- [Projects](#projects)
  - [Sprint 8: Bank Customer Churn Prediction](#sprint-8-bank-customer-churn-prediction)
  - [Sprint 10: Gold Recovery Process Prediction](#sprint-10-gold-recovery-process-prediction)
  - [Sprint 12: Used Car Value Prediction](#sprint-12-used-car-value-prediction)
  - [Sprint 17: Subscription Churn Prediction](#sprint-17-subscription-churn-prediction)
- [Technologies Used](#technologies-used)
- [How to Use This Repository](#how-to-use-this-repository)
- [Future Improvements](#future-improvements)

---

## 🚀 Introduction
This repository contains various machine learning projects completed as part of my data science training at TripleTen. Each project explores different machine learning techniques and predictive modeling approaches to solve real-world business problems. The projects cover classification, regression, feature engineering, and model evaluation strategies.

---

## 📊 Projects

### Sprint 8: Bank Customer Churn Prediction
**Objective:** Predict which customers are likely to leave Beta Bank using machine learning models.

- **Key Techniques:**
  - Data preprocessing: feature selection, encoding, and scaling
  - Handling class imbalance with SMOTE and class weights
  - Model comparison: Decision Tree, Logistic Regression, and Random Forest
  - Feature importance analysis
- **Best Model:** Random Forest (F1 Score = 0.732)
- 📂 [Project Link](./Sprint8)

---

### Sprint 10: Gold Recovery Process Prediction
**Objective:** Optimize the efficiency of gold recovery processes by predicting metal recovery rates.

- **Key Techniques:**
  - Data merging and cleaning
  - Regression modeling: Random Forest, Linear Regression, and Decision Tree
  - sMAPE metric for model evaluation
  - Feature importance analysis
- **Best Model:** Random Forest (sMAPE = 8.9%)
- 📂 [Project Link](./Sprint10)

---

### Sprint 12: Used Car Value Prediction
**Objective:** Build a machine learning model to predict the value of used cars efficiently.

- **Key Techniques:**
  - Exploratory Data Analysis (EDA)
  - Feature engineering and data cleaning
  - Regression modeling: Decision Tree, Random Forest, Linear Regression, Gradient Boosting, XGBoost, CatBoost, and LightGBM
  - Model evaluation using RMSE
- **Best Model:** LightGBM (Balanced accuracy and speed)
- 📂 [Project Link](./Sprint12)

---

### Sprint 17: Subscription Churn Prediction
**Objective:** Predict which customers are likely to cancel their subscription for Interconnect.

- **Key Techniques:**
  - Data cleaning and merging from multiple CSV files
  - Handling class imbalance using SMOTE
  - Model comparison: Random Forest, Logistic Regression, LightGBM, and XGBoost
  - Feature importance analysis
- **Best Model:** LightGBM (AUC-ROC = 0.90)
- 📂 [Project Link](./Sprint17)

---

## 🛠️ Technologies Used
- Python (pandas, numpy, scikit-learn, matplotlib, seaborn)
- Machine Learning Models: Random Forest, Decision Tree, Logistic Regression, Gradient Boosting, XGBoost, LightGBM, CatBoost
- Feature Engineering and Data Preprocessing
- Model Evaluation Metrics: F1 Score, sMAPE, RMSE, AUC-ROC

---

## 📂 How to Use This Repository
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Data_Projects_TripleTen.git
   ```
2. Navigate to the desired project folder:
   ```bash
   cd Data_Projects_TripleTen/SprintXX
   ```
3. Run the project notebook or script following the provided instructions.

---

## 🔍 Future Improvements
- Further optimization of models through hyperparameter tuning
- Exploration of deep learning models where applicable
- Deployment of models using Flask or FastAPI for real-world applications

---

Thank you for checking out my work! Feel free to reach out for collaboration or suggestions. 🚀
