# Customer Churn Prediction

## Project Overview

Customer churn refers to customers discontinuing a company's service. This project aims to predict whether a telecom customer is likely to leave the service based on customer demographics, service usage, and billing information.

The solution helps businesses identify at-risk customers and take proactive retention measures.

---

## Problem Statement

Analyze customer data to predict which customers are likely to churn, enabling companies to improve customer retention strategies and reduce revenue loss.

---

## Dataset

**Dataset:** Telco Customer Churn Dataset

The dataset contains customer information such as:

* Demographic details
* Service subscriptions
* Contract information
* Billing information
* Customer churn status

**Target Variable:** `Churn Value`

* `1` → Customer churned
* `0` → Customer stayed

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* LightGBM
* Streamlit
* Joblib

---

## Project Workflow

1. Data Collection
2. Data Understanding and Exploration
3. Data Cleaning
4. Exploratory Data Analysis (EDA)
5. Feature Engineering
6. Data Preprocessing
7. Model Building
8. Model Evaluation
9. Model Deployment using Streamlit

---

## Data Preprocessing

* Removed unnecessary columns.
* Converted `Total Charges` to numeric values.
* Handled missing values.
* Applied One-Hot Encoding using `pd.get_dummies()`.
* Performed Train-Test Split.
* Handled class imbalance using SMOTE.

---

## Models Implemented

### Logistic Regression

Accuracy: **77.83%**

### Random Forest

Accuracy: **78.32%**

### LightGBM

Accuracy: **77.61%**

---

## Final Model Selection

The **Random Forest Classifier** achieved the highest accuracy and was selected as the final model.

**Final Accuracy:** 78.32%

---

## Key Insights

* Customers with month-to-month contracts are more likely to churn.
* Customers with shorter tenure tend to leave the service.
* Higher monthly charges are associated with increased churn.
* Customers using electronic check payments show higher churn rates.
* Fiber optic internet customers exhibit higher churn.

---

## Project Structure

```text
Customer-Churn-Prediction
│
├── Dataset/
│   └── Telco_customer_churn.xlsx
│
├── models/
│   ├── churn_model.pkl
│   └── model_columns.pkl
│
├── notebooks/
│   └── Customer_Churn_Prediction.ipynb
│
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/HARIPRIYAKS-ops/Customer-Churn-Prediction.git
cd Customer-Churn-Prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Streamlit Application

```bash
streamlit run app.py
```

---

## Future Enhancements

* Hyperparameter tuning for improved accuracy.
* Deployment on Streamlit Cloud.
* Integration with real-time customer data.
* Automated retention recommendation system.

---

