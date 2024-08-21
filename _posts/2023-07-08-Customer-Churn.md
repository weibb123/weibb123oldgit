---
title: "Project Customer Churn"
date: 2023-07-08
categories:
  - Data Analytics
tags:
  - Data Science
---

## Context
![image](https://github.com/user-attachments/assets/dcf95087-b820-4b4d-a066-311414e56853)

Developed a fullstack application that predict customer's churn.

**Key lesson:** 
1. Customers who are likely to churn are those who have less remaining terms. Reason: subscriptions cost, not satisfying with product, altnerative good deals option

2. Look into customers who gave bad rating + remaining term is short, perhaps better off offer them

## Methods

1. Split data into train and testsets: Splitting dataset apart at early stage prevent data bias to avoid making assumptions about whole dataset.
2. Data preprocessing such as filling Null values with "missing" on categorical column, Imputator: average on numerical column
3. feature engineering: create unhappy customers column based on low remaining term + low net promotor rating
4. feature engineering: notice skew data distribution, perform log transform to approximate normal distribution
5. feature engineering: create new feature to decorrelate columns, ML model performs better with decorrelated features
6. Onehot encoding to encode categorical data
7. Notice that dataset is unbalanced, utilized scikitlearn to resample in order to achieve balanced dataset
8. ML pipeline: Search for hyperparameters, tested RFclassifier, XGBoost, GBclassifier, sgdclassifier, ridgeclassifier

code: [Notebook](https://github.com/weibb123/CustomerChurn)
