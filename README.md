# Customer Churn Analysis| End-to-End Data Analytics Project | SQL + Python + Machine Learning + Power BI

## Project Overview

Customer churn directly impacts business growth and profitability. Understanding why customers leave and predicting who is likely to churn allows companies to take proactive retention measures.

This project builds an end-to-end churn analysis pipeline combining SQL for data extraction, Python for machine learning, and Power BI for business intelligence visualization.

Customer data was queried and prepared using SQL, analyzed and modeled using Python, and the results were visualized in an interactive Power BI dashboard to uncover churn patterns and high-risk customer segments.

# Tools & Technologies

**SQL**
Data extraction and preparation

**Python (Pandas, Scikit-learn)**
Data preprocessing and machine learning

**Jupyter Notebook**
Model development and experimentation

**Power BI**
Interactive business intelligence dashboard

**Excel / CSV**
Data storage and data transfer between stages

# Project Workflow

## 1. Data Extraction (SQL)

Customer churn data was queried from the database using SQL.
The queries were used to create structured datasets used for analysis and modeling.

The SQL stage prepared two key datasets:

* **Churn Data** – historical customer information used to train the machine learning model
* **Join Data** – customer records used for generating churn predictions

These datasets formed the foundation of the analysis pipeline.

## 2. Data Preparation (Python)

The SQL outputs were imported into **Python using Pandas** for preprocessing.

Key steps included:

* Removing identifiers and leakage columns
* Cleaning and preparing features
* Encoding categorical variables
* Structuring the dataset for machine learning models

This ensured the data was ready for predictive modeling.

## 3. Machine Learning Model

A Random Forest Classifier was trained to predict customer churn.

Random Forest was chosen because it:

* Handles categorical and numerical features effectively
* Captures complex relationships in customer behavior
* Provides feature importance insights

The dataset was split into training and testing sets to evaluate the model’s predictive performance.

## 4. Model Evaluation

Model performance was assessed using:

* Confusion Matrix
* Classification Report

These metrics helped evaluate the model's ability to correctly identify customers who are likely to churn.

## 5. Churn Prediction

After training, the model was used to generate predictions for additional customer records.

A new variable was created: Customer_Status_Predicted

This identifies customers at risk of leaving and allows businesses to focus retention strategies on high-risk segments.

## 6. Power BI Dashboard

The final dataset containing churn predictions was loaded into **Power BI** to build an interactive dashboard.

The dashboard enables exploration of:

* Overall churn distribution
* Customer segments with higher churn risk
* Behavioral patterns linked to churn
* Key factors influencing customer retention

# Repository Structure

```
customer-churn-analysis
│
├── sql
│   └── churn_analysis.sql
│
├── notebooks
│   └── churn_prediction.ipynb
│
├── data
│   └── prediction_data.csv
│
├── dashboard
│   └── customer_churn_dashboard.pbix
│
└── README.md
```

# Project Outcome

This project demonstrates an **end-to-end data analytics workflow**, integrating:

* SQL for structured data extraction
* Python for predictive modeling
* Power BI for business insight visualization

The result is a pipeline capable of identifying churn patterns and predicting customer churn risk, enabling businesses to design more effective retention strategies.
