Dataset: `customer_churn.csv`

-> Overview

This dataset contains customer-related information used to predict whether a customer will **churn (leave)** or **stay** with a service. It is commonly used for classification problems in Machine Learning.

The dataset includes demographic details, service usage patterns, and billing information.

-> Dataset Features

Below are the key columns typically present in the dataset:

| Column Name        | Description                                                |
| ------------------ | ---------------------------------------------------------- |
| `customerID`       | Unique ID assigned to each customer                        |
| `gender`           | Customer gender (Male/Female)                              |
| `SeniorCitizen`    | Whether the customer is a senior citizen (0 = No, 1 = Yes) |
| `Partner`          | Whether the customer has a partner                         |
| `Dependents`       | Whether the customer has dependents                        |
| `tenure`           | Number of months the customer has stayed                   |
| `PhoneService`     | Whether the customer has phone service                     |
| `MultipleLines`    | Whether the customer has multiple lines                    |
| `InternetService`  | Type of internet service (DSL, Fiber, None)                |
| `OnlineSecurity`   | Whether online security is enabled                         |
| `OnlineBackup`     | Whether online backup is enabled                           |
| `DeviceProtection` | Whether device protection is enabled                       |
| `TechSupport`      | Whether tech support is enabled                            |
| `StreamingTV`      | Whether streaming TV is enabled                            |
| `StreamingMovies`  | Whether streaming movies is enabled                        |
| `Contract`         | Contract type (Month-to-month, One year, Two year)         |
| `PaperlessBilling` | Whether paperless billing is used                          |
| `PaymentMethod`    | Payment method used                                        |
| `MonthlyCharges`   | Monthly billing amount                                     |
| `TotalCharges`     | Total amount charged                                       |
| `Churn`            | Target variable (Yes = churn, No = stay)                   |

---

-> Target Variable

 **`Churn`**

  * `Yes` → Customer left the service
  * `No` → Customer stayed

This is a **binary classification problem**.

-> Use Cases

This dataset is used for:

* Customer churn prediction
* Retention strategy analysis
* Business decision-making
* Machine learning model training (Logistic Regression, Random Forest, XGBoost, etc.)








