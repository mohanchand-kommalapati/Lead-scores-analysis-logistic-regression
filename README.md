#  Lead Scoring Analysis using Logistic Regression

## Project Overview
X Education is an online course provider catering to working professionals. Although the company generates a large volume of leads, only about 30% convert into paying customers, leading to inefficiencies in sales efforts.

The objective of this project is to build a Lead Scoring model that helps the sales team identify high-potential ("Hot") leads, so they can focus their time and resources more effectively and improve the overall conversion rate.

This project demonstrates an **end-to-end machine learning workflow** with a strong focus on **business impact**.

---

##  Business Problem
- Thousands of leads are generated daily from multiple channels
- Sales representatives currently treat all leads similarly
- Low conversion rate (~30%) results in wasted effort and cost
- Management aims to achieve a **target conversion rate of ~80%**

###  Goal
Build a Logistic Regression model that assigns a Lead Score (0–100) to each lead:
- High score → High probability of conversion (Hot Lead)
- Low score → Low probability of conversion (Cold Lead)

---

## Dataset Description
- ~9,000 historical lead records
- Target variable: **Converted**
  - `1` → Lead converted
  - `0` → Lead not converted

### Feature Types
- **Numerical**:  
  - Total Time Spent on Website  
  - Total Visits  
- **Categorical**:  
  - Lead Source  
  - Last Activity  
  - Specialization  
  - What is your current occupation  

 Many categorical features contain a `"Select"` category, which was treated as missing data.

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Logistic Regression
- Jupyter Notebook

---

## Approach & Methodology

### Data Cleaning
- Removed columns with high missing values
- Handled `"Select"` values as nulls
- Imputed missing values where appropriate

### Exploratory Data Analysis (EDA)
- Conversion rate analysis
- Relationship between features and target variable
- Insights into user behavior patterns

### Feature Engineering
- Created dummy variables for categorical features
- Scaled numerical variables
- Removed multicollinearity using **VIF analysis**

### Model Building
- Built a Logistic Regression model
- Used train-test split
- Iteratively refined features based on:
  - Statistical significance
  - Business relevance

### Model Evaluation
- Accuracy
- Precision & Recall
- ROC-AUC Score
- Confusion Matrix
- Probability threshold tuning

---

## Key Results & Insights
- Identified key drivers of lead conversion such as:
  - Time spent on website
  - Lead source
  - Last activity
- Achieved a model that can help:
  - Increase conversion rate close to **80%**
  - Reduce unnecessary calls to low-quality leads
- Lead score enables **data-driven prioritization** for the sales team

---

## Business Impact
By implementing this Lead Scoring model:
- Sales efficiency can be significantly improved
- Marketing spend can be optimized
- Conversion rates can increase without increasing lead volume
- Sales teams can focus on **quality over quantity**

---
Project Report (Recommended)
The complete project analysis with visualizations is available here:

- **http://mohanchand-kommalapati.github.io/Lead-scores-analysis-logistic-regression/**
Open the link in a browser for the best viewing experience.
Author

Mohan Chand Kommalapati

Data Science Learner
