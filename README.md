## Overview

An end-to-end customer churn analytics project analyzing telecommunications
customer data to identify factors associated with customer churn and translate
data-driven findings into actionable business insights.

The project combines Python, SQL, and Tableau to demonstrate data cleaning,
exploratory analysis, SQL analysis, and data
visualization.

## Business Objective

The goal of this analysis is to understand which customer characteristics and
service factors are associated with higher churn rates and identify areas where
businesses could focus customer retention efforts.

## Business Questions

1. Which contract type has the highest churn rate?
2. Does internet service type influence churn?
3. Which payment methods are associated with the highest churn?
4. Are customers with higher monthly charges more likely to churn?
5. Does customer tenure affect churn?

### 1. Data Cleaning

Cleaned the customer dataset by:

- Converting TotalCharges to a numeric data type
- Handling blank values
- Checking for duplicate records
- Verifying missing values
- Creating a cleaned dataset for analysis --> churn_cleaned.csv

### 2. Exploratory Data Analysis

Used Python and Pandas to explore customer demographics,
services, charges, tenure, and churn behavior.

### 3. SQL Analysis

Used SQL to answer the project's five core business questions
and calculate churn rates across customer segments.

### 4. Tableau Dashboard

Built an interactive dashboard to visualize:

- Total customers
- Churned Customers
- Overall churn rate
- Average monthly charges
- Average customer tenure
- Churn rate by contract type
- Churn rate by internet service
- Churn rate by payment method
- Monthly charges by churn status
- Churn rate by tenure group

## Key Findings

- Month-to-month customers showed the highest churn rate.
- Customers with shorter tenure demonstrated substantially higher churn.
- Customers who churned had higher average monthly charges than customers who remained.
- Fiber optic customers had higher churn than other internet service groups.
- Electronic check customers had the highest churn rate among payment methods.

These findings suggest that pricing, contract commitment, customer experience, and payment preferences all contribute to customer retention. To reduce churn, the company should prioritize converting customers to longer-term contracts, improving early customer engagement, reviewing pricing strategies for premium services, and encouraging enrollment in automatic payment methods.

## Dashboard

