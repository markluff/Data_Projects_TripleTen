# Used Car Value Prediction: Evaluation and Predictions

## 📌 Table of Contents
- [Introduction](#introduction)
- [Process](#process)
- [Conclusion](#conclusion)

---

## 🏆 Introduction
Rusty Bargain requested a quality model to **predict the value of used cars** efficiently while ensuring **fast training and prediction times**. The goal of this project was to develop an accurate, yet computationally efficient, predictive model for used car pricing.

---

## 🔬 Process
I conducted **Exploratory Data Analysis (EDA)** on the provided `car_data.csv` file to clean and prepare it for machine learning. The dataset contained unnecessary columns, which were removed to streamline the model-building process. Additionally, I engineered key features such as **vehicle age** and **listing duration** to improve model performance. Data with inconsistent or incorrect values was also filtered out.

Once the dataset was prepared, I split it into **training (75%) and testing (25%)** sets. Then, I compared the performance of seven different machine learning regression models:
1. **Decision Tree**
2. **Random Forest**
3. **Linear Regression**
4. **Gradient Boosting**
5. **XGBoost**
6. **CatBoost**
7. **LightGBM**

The goal was to find the model with the **lowest RMSE** while also considering training and prediction speed. The **LightGBM model** proved to be the most efficient, ranking **second-best in RMSE (after CatBoost)** and **second-fastest in training and prediction times (after Decision Tree)**.

While **CatBoost** achieved the lowest RMSE (**1534**), it required significantly more time for hyperparameter tuning and training. In contrast, **LightGBM** was able to **tune faster** and still produce nearly as accurate predictions as CatBoost.

---

## 📊 Conclusion
I recommend that **Rusty Bargain** use the **LightGBM** model for predicting used car values. This model provides the best balance between **accuracy and efficiency**, making it ideal for real-time application needs.

🚀 **Future Work:** Further tuning of LightGBM, integrating additional feature engineering techniques, and exploring ensemble methods could enhance predictive performance even more.

