#  Credit Risk Scoring Project

## Overview

This project focuses on building a machine learning model to predict whether a bank customer is likely to default on a loan.

The goal is to help financial institutions make better lending decisions and reduce financial risk.

---

## Business Problem

Banks need to decide:

> “Should we approve this loan or not?”

Incorrect decisions can lead to:

* Financial losses (if customer defaults)
* Missed opportunities (rejecting good customers)

This project aims to **identify high-risk customers** using data-driven methods.

---

## Dataset

* German Credit Dataset
* Contains information about:

  * Age
  * Job
  * Housing
  * Savings & Checking accounts
  * Credit amount
  * Loan duration
  * Purpose

---

## Data Cleaning

* Removed unnecessary index column
* Handled missing values by introducing `no_account`
* Standardized column names
* Created and cleaned target variable (`Risk`)

---

## Exploratory Data Analysis (EDA)

Key insights:

* Longer loan durations are associated with higher risk
* Customers with low or no savings show higher default probability
* Renters tend to have higher risk compared to homeowners
* Higher credit amounts increase default likelihood

---

## Feature Engineering

Created meaningful features:

* Loan-to-Age ratio
* Monthly payment (credit amount / duration)
* Account ownership indicators
* Housing stability score

---

## Model

* Logistic Regression

### Evaluation Metrics:

* Precision
* Recall
* F1-score

---

## Key Findings

* Financial pressure (high monthly payments) increases risk
* Lack of savings is a strong predictor of default
* Loan duration is one of the most influential factors

---

## Business Impact

This model can help banks:

* Reduce default risk
* Improve loan approval decisions
* Better understand customer risk profiles

---

## Tech Stack

* Python 3.13
* pandas
* numpy
* seaborn
* matplotlib
* scikit-learn

---

## Project Structure

```
credit-risk-scoring/
│
├── data/
├── notebooks/
│   ├── 01_eda.ipynb
│   └── 02_modeling.ipynb
├── src/
└── README.md
```

---

## Future Improvements

* Try Random Forest / XGBoost
* Hyperparameter tuning
* Deploy as a web app (Streamlit)

---

## Author

Muhammad Sodiq
