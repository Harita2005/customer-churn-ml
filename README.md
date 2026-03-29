 Customer Churn Prediction using Machine Learning

 Introduction

Customer retention is one of the biggest challenges for businesses today. Acquiring new customers is often more expensive than retaining existing ones, which makes churn prediction extremely valuable.

In this project, I built a complete machine learning pipeline to predict whether a customer is likely to churn. The goal is not just prediction, but also understanding **why customers leave**, so businesses can take proactive actions.

 Objective

The main objectives of this project are:

* To predict customer churn using multiple machine learning models
* To compare model performance and identify the best approach
* To extract meaningful insights that can help improve customer retention
* To explore both data-driven and rule-based decision-making


Dataset Description

The dataset consists of various customer-related attributes, including:

* **Tenure** – How long the customer has stayed
* **Monthly Charges** – Customer spending pattern
* **Total Charges** – Overall value of the customer
* **Contract Type / Membership** – Subscription behavior
* **Service Usage** – Features like Tech Support, Streaming, etc.

 Target Variable

* `Churn`

  * `1` → Customer will churn
  * `0` → Customer will stay

---

 Project Workflow

This project follows a structured ML pipeline:

 1. Data Preprocessing

* Handled missing values
* Converted categorical variables into numerical form
* Cleaned and standardized the dataset

2. Feature Engineering & Encoding

* Applied **One-Hot Encoding** for categorical features
* Ensured compatibility with ML models

3. Feature Selection

* Used **Random Forest feature importance**
* Selected only the most impactful features to reduce noise

4. Model Training

Trained multiple models to compare performance:

* Logistic Regression
* Random Forest
* Tuned Random Forest
* XGBoost

5. Model Evaluation

Evaluated each model using:

* Accuracy
* Precision, Recall, F1-score
* ROC-AUC
* Confusion Matrix

6. Hyperparameter Tuning

* Used **GridSearchCV** to optimize Random Forest
* Improved model generalization and performance

7. Rule-Based Approach

* Designed a simple logic-based model based on business understanding
* Example rules:

  * Low total charges + low monthly income → high churn risk
  * No contract → higher probability of churn

8. Model Comparison

* Compared all models to identify the best-performing one

 -> Models Used

 🔹 Logistic Regression

A simple and interpretable baseline model.
Helps understand feature influence but limited in capturing complex patterns.

 🔹 Random Forest

An ensemble model that handles non-linear relationships well.
Improved accuracy compared to Logistic Regression.

 🔹 Tuned Random Forest

Optimized using hyperparameter tuning.
Better performance and reduced overfitting.

🔹 XGBoost

A powerful boosting algorithm known for high performance.
Handles complex feature interactions effectively.

🔹 Rule-Based Model

A manually designed model based on domain knowledge.
Useful for explainability but less accurate than ML models.



 -> Model Performance (Example)

| Model               | Description        | Performance |
| ------------------- | ------------------ | ----------- |
| Logistic Regression | Baseline           | 82%         |
| Random Forest       | Ensemble           | 79%         |
| Tuned Random Forest | Optimized          | 82%         |
| XGBoost             | Boosting model     | 81%         |
| Rule-Based          | Heuristic approach | 45%        |

-> key Insights

From the analysis, a few important patterns emerged:

* Customers with **low total spending** are more likely to churn
* **Contract type** plays a major role in retention
* Customers without **support services** tend to leave more frequently
* Long-term customers are less likely to churn

 Final Conclusion

* Ensemble models like **Random Forest and XGBoost** clearly outperform simpler models
* Hyperparameter tuning significantly improves results
* Rule-based systems are easy to understand but lack predictive power

-> Best Performing Model

XGBoost / Tuned Random Forest  achieved the best balance of accuracy and ROC-AUC.

-> Project Structure

customer-churn-ml/
│
├── data/              # Raw dataset
├── notebooks/         # Jupyter notebooks with code
├── outputs/           # Graphs, plots, and evaluation results
├── README.md          # Project documentation

 -> Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn
* XGBoost
* Matplotlib, Seaborn

-> Outputs

The `outputs/` folder contains:

* Confusion matrices
* ROC curves
* Model comparison graphs
* Feature importance plots

These visualizations help in better understanding model performance and behavior.

 -> Future Improvements

* Handle class imbalance using **SMOTE**
* Perform deeper feature engineering
* Try advanced models like LightGBM
* Deploy the model using **Streamlit or Flask**
* Build a real-time churn prediction dashboard

-> Final Note

This project represents a complete end-to-end machine learning workflow — from raw data preprocessing to model evaluation and business insights.

It not only focuses on prediction but also on **understanding customer behavior**, making it highly relevant for real-world business applications.

