# Fraud-Detection

This project focuses on identifying fraudulent activities and predicting key financial metrics using advanced Machine Learning techniques. By combining **Classification** and **Regression** models, the system not only flags suspicious transactions but also provides quantitative insights into fraud-related data.

## 📌 Project Overview
Fraud remains one of the most significant challenges in financial ecosystems. This project aims to minimize financial losses and protect brand reputation by building a robust pipeline that covers everything from raw data processing to high-performance predictive modeling.

### Key Objectives:
- **Classification:** Identify whether a transaction is "Fraud" or "Legit".
- **Regression:** Predict continuous variables related to transactions (e.g., amount or risk scores).
- **Feature Engineering:** Enhance model performance through domain-specific data transformations.

---

## 🛠 Tech Stack & Workflow

### 1. Exploratory Data Analysis (EDA)
 **Missing Value Handling:** Systematic treatment of null values to maintain data integrity.
 **Statistical Analysis:** * Detailed statistics for `transaction_amount`.
     **Normality Tests:** Assessing `device_change_30d` distribution.
     **Categorical Tests:** Statistical testing for categorical feature significance.

### 2. Data Preprocessing & Feature Engineering
* **Encoding:** Applied `OneHotEncoding`, `OrdinalEncoding`, and `LabelEncoding` based on feature characteristics.
* **Scaling:** Data normalization and standardization for distance-based models (SVM, KNN).
* **Feature Engineering:** Creation of new features and hyperparameter optimization to boost model sensitivity.

### 3. Modeling Framework
We implemented a wide range of algorithms to compare performance across different architectural approaches:

#### **Classification Models:**
* Logistic Regression (Baseline & Scaled)
* Support Vector Machines (SVM)
* Decision Tree Classifier
* Random Forest Classifier
* K-Nearest Neighbors (KNN)

#### **Regression Models:**
* Linear Regression
* Decision Tree & Random Forest Regressors
* Gradient Boosting (XGBoost, LightGBM)

---

## 📊 Performance Results

After extensive testing and hyperparameter tuning, the following models demonstrated the highest performance:

### **Classification Results (Fraud Identification)**
| Model | Accuracy |
| :--- | :--- |
| **Random Forest Classifier** | **93%** |
| **Decision Tree Classifier** | **92%** |

### **Regression Results (Value Prediction)**
| Model | R-squared ($R^2$) |
| :--- | :--- |
| **Linear Regression** | **0.80** |
| **XGBoost Regressor** | **0.79** |
| **LightGBM Regressor** | **0.78** |

---

## 🚀 Conclusion
The **Random Forest Classifier** is the recommended model for real-time fraud detection due to its high accuracy (93%). For estimating continuous transaction metrics, **Linear Regression** provided the most reliable $R^2$ score (0.80), followed closely by boosting algorithms.
