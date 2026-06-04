# NovaSuite Revenue Leakage Analysis

## Project Overview

This project analyzes a fictional B2B SaaS company, **NovaSuite**, to identify areas where the business may be losing revenue and uncover opportunities to improve customer retention.

The project simulates a real-world business scenario in which a Data Analyst is tasked with investigating revenue leakage, customer churn risk, and operational inefficiencies using Python for data preparation and Power BI for business intelligence reporting.

---

## Business Problem

NovaSuite is a subscription-based software company experiencing steady customer growth, but leadership suspects that revenue is being lost through billing inefficiencies, customer inactivity, and churn.

The objective of this project is to:

* Clean and validate customer subscription data
* Identify potential revenue leakage points
* Prepare the dataset for business analysis
* Build an interactive Power BI dashboard
* Provide actionable business recommendations

---

## Dataset Information

The dataset contains customer-level subscription information, including:

* Customer details
* Subscription plans
* Monthly Recurring Revenue (MRR)
* Annual Recurring Revenue (ARR)
* Billing cycles
* Payment status
* Product usage metrics
* Customer satisfaction scores (NPS)
* Support ticket activity
* Login activity
* Churn information

The dataset was intentionally created with data quality issues to simulate real-world business data.

Examples include:

* Duplicate records
* Missing values
* Inconsistent plan names
* Inconsistent region naming conventions
* Mixed date formats
* Inconsistent currency formatting

---

## Tools Used

### Python

Used for:

* Data cleaning
* Data validation
* Feature engineering
* Data quality checks

Libraries:

* Pandas
* NumPy
* Jupyter Notebook

### Power BI

Used for:

* Interactive dashboards
* Revenue leakage analysis
* Customer health monitoring
* Executive reporting

---

## Data Cleaning Process

The following data quality issues were identified and resolved:

### Duplicate Records

* Removed duplicate customer records

### Missing Values

Handled missing values in:

* Industry
* Acquisition Channel
* Sales Rep

### Standardization

Standardized:

* Subscription plans
* Regions
* Date formats
* Revenue fields

### Revenue Validation

Validated that:

ARR = MRR × 12

to identify potential revenue inconsistencies.

---

## Feature Engineering

The following analytical fields were created:

### Days Since Login

Measures customer engagement by calculating the number of days since a customer's most recent login.

### Is_Churned

Flags customers who have churned.

### Low_Utilization_Flag

Identifies customers using less than 50% of purchased seats.

### High_Support_Flag

Identifies customers with high support ticket volumes.

### Inactive_60_Days_Flag

Flags customers who have not logged in within the last 60 days.

---

## Analysis Objectives

The analysis focuses on answering the following business questions:

### Revenue Leakage

* Are failed payments being recovered effectively?
* Are seat overages being billed correctly?
* Are annual discounts being applied consistently?

### Customer Health

* Which customers are at risk of churn?
* Does low product utilization increase churn risk?
* Does inactivity correlate with churn?
* Do support ticket volumes indicate customer dissatisfaction?

---

## Key Deliverables

* Cleaned dataset
* Python data cleaning notebook
* Power BI dashboard
* Business recommendations
* Revenue leakage analysis

---

## Repository Structure

```text
NovaSuite-Revenue-Leakage-Analysis/
│
├── data/
│   ├── NovaSuite_SaaS_Raw_Dataset.xlsx
│   └── NovaSuite_SaaS_Cleaned.xlsx
│
├── notebooks/
│   └── nova_suite.ipynb
│
├── dashboard/
│   └── NovaSuite_Dashboard.pbix
│
├── screenshots/
│   └── dashboard_images
│
└── README.md
```

---

## Future Enhancements

* Churn prediction modeling
* Customer segmentation analysis
* Revenue forecasting
* Automated data quality monitoring

---

## Author

Lilian Cheuno
