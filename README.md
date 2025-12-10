# Customer Churn Analysis & Prediction (Python + Power BI)

This project focuses on analyzing customer behavior and predicting churn for a subscription-based service.  
The goal is to identify which customers are at high risk of leaving and understand the key drivers behind churn so that the business can take proactive retention actions.

---

## 🎯 Objectives

- Analyze historical customer data and identify patterns related to churn.
- Build a predictive model to classify customers as **"Churn"** or **"Not Churn"**.
- Visualize churn insights and key metrics using **Power BI**.
- Provide actionable recommendations to reduce churn and improve customer retention.

---

## 📂 Dataset

- **Rows (example):** ~7,000+ customers  
- **Target variable:** `Churn` (Yes/No)  
- **Example features:**
  - `gender`
  - `SeniorCitizen`
  - `tenure`
  - `MonthlyCharges`
  - `TotalCharges`
  - `Contract` (Month-to-month / One year / Two year)
  - `InternetService`
  - `OnlineSecurity`, `TechSupport`
  - `PaymentMethod`

> You can replace this section with the actual dataset source (e.g., Kaggle Telco Customer Churn dataset) if applicable.

---

## 🧹 Data Cleaning & Preprocessing

Key preprocessing steps:

- Handled missing values and invalid entries (e.g., blank `TotalCharges`).
- Converted categorical variables into numeric form (Label Encoding / One-Hot Encoding).
- Treated outliers where necessary using simple statistical checks.
- Scaled numerical features for model training (where helpful).
- Split data into **train** and **test** sets to evaluate model performance.

---

## 🔍 Exploratory Data Analysis (EDA)

Performed EDA in Python to understand:

- Churn rate across the customer base.
- Relationship between **contract type**, **tenure**, **monthly charges**, and churn.
- Service-related features that strongly correlate with churn (e.g., lack of `TechSupport` or `OnlineSecurity`).
- Visualizations used:
  - Bar charts (churn by contract type, payment method, internet service)
  - Histograms (tenure, monthly charges)
  - Correlation heatmap for numerical features

---

## 🤖 Modeling

**Goal:** Predict whether a customer is likely to churn.

Models experimented with:

- **Logistic Regression** (baseline model)
- **Random Forest Classifier** (improved performance)
- Other models like XGBoost

**Example metrics (update with your real results):**

- Accuracy: ~**85–88%**
- Precision/Recall/F1-score for the churn class
- Confusion matrix to understand model performance

Focus of the project is to **interpret results**, not just to maximize accuracy.

---

## 📊 Power BI Dashboard

An interactive **Power BI dashboard** was created to help stakeholders:

- View **overall churn rate** and trends.
- Filter customers by:
  - Contract type
  - Tenure band (e.g. 0–12, 13–24, 25+ months)
  - Payment method
  - Internet service type
- Analyze **key churn drivers**:
  - High churn in month-to-month contracts
  - Higher churn for customers with no `OnlineSecurity` or `TechSupport`
  - Churn patterns by monthly charges and tenure
- See **segment-wise breakdowns** to support targeted retention campaigns.



