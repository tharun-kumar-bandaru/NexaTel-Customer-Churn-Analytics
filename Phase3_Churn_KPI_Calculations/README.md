# Phase 3: Churn KPI Calculations 

## NexaTel Customer Churn Analytics 

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?logo=numpy)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)


---

## Project Overview

This repository contains **Phase 3 of the NexaTel Customer Churn Analytics Project**, focused on calculating key business KPIs required to understand customer retention, churn, recurring revenue, customer value, and service performance.

The analysis uses the same **24-table NexaTel telecom dataset** used throughout Phases 1 and 2.

The objective of Phase 3 is to transform the cleaned and explored data from the previous phases into **business-focused Key Performance Indicators (KPIs)** that can support management decision-making and the final Power BI dashboard.

The Phase 3 analysis covers:

- Customer Churn Rate
- Customer Retention Rate
- Average Revenue Per User (ARPU)
- Customer Lifetime Value (CLV)
- Revenue Lost to Churn
- Monthly Recurring Revenue (MRR)
- First Contact Resolution (FCR)
- Average Resolution Time
- Contract Renewal Rate
- Average Customer Tenure
- Cohort Retention Analysis

---

# Objectives

The major objectives of Phase 3 are:

1. Calculate the monthly customer churn rate.
2. Measure customer retention performance.
3. Calculate recurring revenue and ARPU.
4. Estimate customer lifetime value.
5. Quantify revenue exposed to customer churn.
6. Measure customer support effectiveness.
7. Calculate contract renewal performance.
8. Measure average customer tenure.
9. Compare KPI performance against project benchmarks.
10. Prepare structured outputs for Phase 4 Power BI dashboard development.
11. Perform optional cohort retention analysis.

---

# Business Context

NexaTel Digital Services is a simulated Indian telecom and digital-services operator serving customers across multiple product lines.

The company operates across:

- Prepaid Mobile
- Postpaid Mobile
- 4G
- 5G
- Fiber Broadband
- Enterprise Connectivity
- IoT Solutions
- Smart Home
- OTT Bundles

The management team wants to understand:

- How many customers are leaving each month?
- What percentage of customers are retained?
- How much recurring revenue does the company generate?
- How valuable are customers over their lifetime?
- How much revenue is lost because of churn?
- How effectively are customer support issues resolved?
- How many contracts are successfully renewed?
- How long do customers typically remain with NexaTel?

Phase 3 converts these business questions into measurable KPIs.

---

# Dataset

The NexaTel project contains **24 interconnected CSV tables** representing approximately **757,000 records** across customer, subscription, billing, support, usage, network, contract, and other operational data.

Important tables used in Phase 3 include:

| Table | Purpose |
|---|---|
| `customers.csv` | Customer profile, segment, plan, tenure and churn status |
| `subscriptions.csv` | Subscription and recurring charge information |
| `plans.csv` | Plan catalogue and monthly charges |
| `billing.csv` | Monthly billing and recurring revenue information |
| `support_tickets.csv` | Customer support and resolution information |
| `contracts.csv` | Contract and renewal information |

The project specification requires KPI calculations to be traceable to the underlying data rather than using hardcoded values. :contentReference[oaicite:0]{index=0}

---

# Technologies Used

### Programming Language
- Python 3.x

### Libraries
- Pandas
- NumPy

### Development Environment
- Jupyter Notebook

### Analysis Techniques
- Data aggregation
- Filtering
- Date-based analysis
- GroupBy operations
- KPI calculations
- Customer-level analysis
- Cohort analysis
- Business benchmarking
