# 📊 IBM Telco Customer Churn Analysis

##  Overview
This project analyzes customer churn behavior using the IBM Telco dataset. The goal is to identify key factors that influence customer attrition and provide data-driven insights to improve retention strategies.

The analysis focuses on customer demographics, service usage, and account information to uncover patterns associated with churn.

---

##  Objectives
- Analyze overall churn rate and customer distribution  
- Identify key drivers of churn (e.g., contract type, payment method, internet service)  
- Perform segmentation analysis across customer groups  
- Explore churn reasons for high-risk segments  
- Build a structured, end-to-end data pipeline to clean, transform, and prepare data for machine learning

---

##  Dataset
- Source: IBM Telco Customer Churn Dataset (Kaggle)  
- Size: ~7,000 customers  
- Features include:
  - Customer demographics (tenure, senior citizen status)  
  - Service usage (internet service, additional services)  
  - Account details (contract type, payment method, charges)  
  - Churn label and churn reason  

---

##  Data Preparation (ETL Pipeline)
A structured ETL workflow was implemented:

- **Extract:** Load raw customer data from CSV  
- **Transform:**
  - Clean column names and data types  
  - Handle missing values (e.g., `TotalCharges`)  
  - Encode categorical variables for analysis  
- **Load:**
  - Create an analysis-ready dataset for EDA  
  - Create a model-ready dataset for machine learning  

---

##  Exploratory Data Analysis

Key analyses performed:
- Overall churn rate calculation  
- Churn by:
  - Contract type  
  - Payment method  
  - Internet service type  
  - Additional services (Online Security, Tech Support)  
- Correlation analysis using encoded features  
- Customer segmentation using clustering  

---

##  Key Insights

- Customers with **month-to-month contracts** show significantly higher churn  
- **Fiber optic users** have the highest churn rate (>40%)  
- Customers using **electronic check** are more likely to churn  
- Lack of **additional services** (e.g., online security, tech support) is associated with higher churn  

###  Fiber Optic Churn Analysis
Further analysis revealed that churn among fiber optic customers is driven by:
- Customer service issues (support experience)  
- Competitive pressure (better pricing, speed, and data from competitors)  
- Perceived value vs cost  

---

##  Business Recommendations

- Improve customer support experience and response time  
- Offer competitive pricing and improve internet service performance  
- Increase adoption of additional services 
- Enhance network reliability and clearly communicate value  

---

##  Machine Learning (Logistic Regression)

A logistic regression model was developed to predict customer churn:

- Data standardization and preprocessing  
- Train-test split  
- Model training and prediction  
- Evaluation using:
  - Accuracy  
  - Precision / Recall  
  - F1-score  
  - Confusion matrix  

---

## 🛠️ Tools & Technologies
- Python (pandas, numpy)  
- Data visualization: seaborn, matplotlib  
- Machine learning: scikit-learn  
- Environment: Google Colab

---

## 👤 Author
Nathan Huynh  
Management Information Systems | Data Analytics  
