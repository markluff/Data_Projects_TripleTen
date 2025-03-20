# Gold Recovery Process: Evaluation and Predictions

## 📌 Table of Contents
- [Introduction](#introduction)
- [Process](#process)
- [Conclusion](#conclusion)

---

## 🏆 Introduction
Zyfra is looking to create a predictive model that will help a gold mining and refinement company develop more efficient processes. In this project, I explore the provided data in three datasets to ensure its usability for machine learning. I then prepare it for analysis. Once the data is fully ready, I use three different regression models to find optimized solutions for the gold mining company.

---

## 🔬 Process
The data came in three different files: **Training, Test, and Full**. The Test set did not include all the columns that the Training and Full sets did. To address this, I used the **Date** column as a functional ID for each observation and matched the corresponding dates from the Full set to extract the missing columns. Once I had a complete dataset, I cleaned the data and verified that the calculated columns were correctly computed.

After the data was cleaned, I wrote a function to calculate the **sMAPE score** for each prediction. Then, I used the training dataset to build three machine learning regression models:
1. **Random Forest**
2. **Linear Regression**
3. **Decision Tree**

Once the models were built, I found that the sMAPE on the Training set was below **10%** for all models. After effectively training each model, I applied them to the test set to determine which model performed best in predicting the **Rougher and Final Output Recovery of Gold**.

To ensure that the best model outperformed random chance, I also conducted a **sanity check**, setting the prediction value equal to the mean for the entire column. This test demonstrated that both the **Random Forest Regressor** and the **Decision Tree Regressor** were more effective at predicting the quantity of gold recovered.

As a final step, I analyzed the **feature importance** of the Random Forest model to identify the most critical variables for accurate predictions.

---

## 📊 Conclusion
The **Random Forest model** outperformed the other two models, achieving a final **sMAPE value of 8.9%**, whereas the sanity check yielded an sMAPE of **10.2%**. This **1.3% improvement** indicates that the **Random Forest model** is the best choice for future predictions.

However, this model is computationally intensive. If a **faster** model is required, the **Decision Tree model** offers a good alternative, outperforming the sanity check by nearly **1%**, with an sMAPE of **9.3%**. The **Decision Tree model** would be a better option if the company needs quicker predictions.

Finally, the most important features for building effective models were **final.output.tail_au** and **rougher.input.feed_au**. This suggests that early and late gold readings in the ore and solution provide the best indicators of ore quality. To optimize processes, the company should focus on improving efficiencies at these two points.

🚀 **Future Work:** Further model optimization, feature engineering, and testing alternative machine learning approaches could help refine predictions even further.

