# Customer Churn Analysis & Prediction (Telecom Industry)

Customer churn, or the loss of customers, can seriously affect a company's bottom line. It's essential for businesses to understand why customers are leaving and to actively work on strategies to keep them. 


This project focuses on **analyzing, understanding, and predicting customer churn** in a telecom company using **data analysis, visualization, clustering, and machine learning models**.  
The goal is to identify key factors that cause customers to leave and build predictive models to help improve customer retention.

---

## Project Overview

Customer churn has a major financial impact on telecom companies. In this project, we:

- Perform **data preprocessing and exploratory data analysis (EDA)**
- Identify **patterns and drivers of churn**
- Apply **customer segmentation using clustering**
- Build and evaluate **multiple machine learning models**
- Create an **interactive dashboard** for insights visualization

---

## Dataset

- **Dataset:** Telco Customer Churn Dataset  
- **Target Variable:** `Churn` (Yes / No)
- **Type:** Structured tabular data (categorical + numerical)
- **Key Features:**
  - Customer demographics (gender, senior citizen, dependents)
  - Services subscribed (Internet, phone, online security, tech support)
  - Contract and billing information
  - Monthly and total charges

---

## Technologies & Tools

- **Programming Language:** Python  
- **Libraries:**
  - Data Analysis: `pandas`, `numpy`
  - Visualization: `matplotlib`, `seaborn`, `plotly`
  - Machine Learning: `scikit-learn`
  - Dashboard: `Dash (Plotly)`
- **Environment:** Jupyter Notebook / VS Code

---

## Project Workflow

###  Data Preprocessing
- Removed duplicate records
- Dropped irrelevant columns (`customerID`)
- Converted `TotalCharges` to numerical
- Removed invalid records (`tenure = 0`)
- Encoded categorical variables
- Handled missing values

---

###  Exploratory Data Analysis (EDA)
Key findings from analysis and visualizations:

- **26.6% of customers churned**
- Customers with **Month-to-Month contracts** churn the most
- **Senior citizens** show a higher churn rate
- Customers **without dependents or partners** are more likely to churn
- **Electronic Check** users churn significantly more
- **Fiber optic internet users** have the highest churn rate
- Lack of **Online Security** and **Tech Support** strongly correlates with churn
- Higher **Monthly Charges** and **Total Charges** increase churn likelihood

---

###  Correlation Analysis
- Identified strong relationships between churn and:
  - Contract type
  - Monthly charges
  - Service subscriptions
  - Payment methods

---

###  Customer Segmentation (Clustering)
- Applied clustering techniques to segment customers
- Key insights:
  - **Clusters 0 and 3** show higher churn rates
  - High-risk clusters typically:
    - Use Month-to-Month contracts
    - Are more likely to be senior citizens
    - Lack online security
    - Use fiber optic internet

---

## Machine Learning Models

Multiple classification models were trained and evaluated:

- Logistic Regression
- Support Vector Classifier (SVC)
- Decision Tree Classifier
- Random Forest Classifier
- AdaBoost Classifier
- Gradient Boosting Classifier

### Best Performing Model
- **Random Forest Classifier**
- Achieved the highest overall performance and generalization
- Recommended for churn prediction deployment

---

## Model Evaluation
Models were compared using:
- Accuracy
- Precision
- Recall
- F1-Score

Random Forest demonstrated the best balance between performance and reliability.

---

## Interactive Dashboard

An **interactive dashboard** was built using **Plotly Dash** to:
- Visualize churn distribution
- Explore customer segments
- Analyze service usage and churn relationships
- Support data-driven decision making



