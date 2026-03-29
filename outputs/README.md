Customer Churn Prediction – Output Summary

Overview

This project focuses on predicting whether a customer will leave (churn) or stay using different machine learning models. Various visualizations and model results are stored in the output folder to help understand patterns and performance.

-> Output Files Explanation

**01_churn_distribution.png**
Shows how many customers stayed vs churned.
-Helps identify class imbalance in the dataset.

**02_income_vs_churn.png**
Compares income levels between churned and non-churned customers.
-Higher income customers tend to churn slightly more.

**03_purchases_vs_churn.png**
Shows purchase behavior for both groups.
-Customers with fewer purchases are more likely to churn.

**04_logistic_regression_confusion_matrix.png**
Displays prediction results of Logistic Regression.
-Shows correct vs incorrect predictions.

**05_logistic_regression_roc_curve.png**
ROC curve for Logistic Regression with AUC = 0.86.
-Indicates good model performance.

**06_model_comparison.png**
Compares accuracy of Logistic Regression and Random Forest.
-Logistic Regression performs slightly better.

**07_feature_importance.png**
Shows most important features affecting churn.
-Purchases, tenure, and income are key factors.

**08_rule_based_confusion_matrix.png**
Performance of a simple rule-based approach.
-Less accurate compared to ML models.

**09_model_accuracy_table.png**
Table showing accuracy of all models.
-Helps quick comparison.

**10_model_accuracy_comparison.png**
Visual comparison of model accuracies.
-Logistic Regression and Tuned RF are close.

**11_roc_curve_comparison.png**
ROC curves of multiple models (LR, RF, Tuned RF).
-All models perform similarly with AUC ≈ 0.86.

-> Key Inferences

* Dataset is slightly imbalanced (more non-churn customers).
* Customers with **low purchases and low tenure** are more likely to churn.
* **Income also plays a role**, but not as strong as purchases.
* Logistic Regression performed the best overall.
* Random Forest improved slightly after tuning but didn’t outperform LR significantly.
* ROC curves show that all models are **reliable and consistent**.

-> Conclusion

The model successfully predicts customer churn with good accuracy (~82%).
While Logistic Regression performs well as a baseline model, the key insight is that **advanced models like XGBoost and Random Forest provide competitive and slightly improved performance**.

* **XGBoost achieved the highest accuracy (~82%)**
* **Random Forest also performed well (~81%)**
* Logistic Regression remains useful for baseline comparison, but not the best final choice

These models are better at capturing complex patterns in customer behavior.

Therefore, **XGBoost is the best choice for deployment** due to:

* High accuracy
* Better handling of complex relationships
* Strong performance consistency

-> Final Note

This output folder provides both:
✔ Visual understanding of data
✔ Performance comparison of models


Overall, the project shows that **machine learning models like XGBoost can effectively identify at-risk customers**, helping businesses take proactive steps such as targeted offers, retention strategies, and personalized engagement to reduce churn.
