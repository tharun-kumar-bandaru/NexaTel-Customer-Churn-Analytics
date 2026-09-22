# 🧹 Phase 1 — Data Cleaning & Quality Check

## NexaTel Customer Churn Analytics

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)
![Status](https://img.shields.io/badge/Phase-1%20Completed-success)

---

## 📌 Overview

Phase 1 focuses on **Data Loading, Cleaning and Quality Check** for the NexaTel Customer Churn Analytics project.

The objective of this phase is to understand the structure and quality of the NexaTel dataset before performing exploratory analysis, KPI calculations, and dashboard development.

The project contains **24 interconnected tables** with approximately **757,000 records**. The `customers` table acts as the central table, with multiple operational tables connected through primary and foreign keys.

This phase establishes a reliable foundation for all subsequent analysis.

---

## 🎯 Objectives

The main objectives of Phase 1 are to:

- Load all 24 CSV datasets into Python.
- Profile every table.
- Analyze row and column counts.
- Inspect data types.
- Identify missing values.
- Calculate missing-value percentages.
- Detect duplicate records.
- Validate primary-key uniqueness.
- Validate date fields.
- Validate numeric fields.
- Detect billing anomalies.
- Identify data-usage outliers.
- Validate customer information.
- Verify referential integrity.
- Analyze subscription data quality.
- Analyze unresolved complaints.
- Compare findings against the provided data-quality issue log.

---

## 📂 Dataset Structure

The NexaTel database contains 24 interconnected tables.

| # | Table | Purpose |
|---|---|---|
| 1 | `customers` | Central customer profile and churn information |
| 2 | `subscriptions` | Customer subscription records |
| 3 | `plans` | Available telecom plans |
| 4 | `plan_history` | Plan upgrade and downgrade history |
| 5 | `contracts` | Customer contract information |
| 6 | `devices` | Customer device information |
| 7 | `billing` | Monthly customer invoices |
| 8 | `payments` | Payments made against invoices |
| 9 | `recharges` | Prepaid recharge transactions |
| 10 | `usage_voice` | Monthly voice usage |
| 11 | `usage_sms` | Monthly SMS usage |
| 12 | `usage_data` | Monthly mobile data usage |
| 13 | `network_quality` | Monthly network experience |
| 14 | `support_tickets` | Customer support interactions |
| 15 | `complaints` | Formal customer complaints |
| 16 | `customer_feedback` | CSAT and NPS feedback |
| 17 | `retention_campaigns` | Customer-level retention campaigns |
| 18 | `marketing_campaigns` | Marketing campaign definitions |
| 19 | `employees` | Support and sales employees |
| 20 | `stores` | Retail store information |
| 21 | `regions` | Operating regions |
| 22 | `cities` | City information |
| 23 | `states` | Indian states and union territories |
| 24 | `data_quality_issue_log` | Reference list of known data-quality issues |

---

## 🔍 Data Quality Checks

The following checks were performed during Phase 1.

### 1. Dataset Profiling

For each table, the following information was reviewed:

- Number of rows
- Number of columns
- Column names
- Data types
- Duplicate records
- Missing values

---

### 2. Missing-Value Analysis

Missing values were checked across every column.

The analysis identifies:

- Columns containing missing values
- Number of missing records
- Percentage of affected records
- Tables with the highest number of missing values

Missing values were not automatically treated as errors because some fields are legitimately nullable according to the data dictionary.

For example, `churn_date` can be blank for active customers.

---

### 3. Duplicate Detection

Duplicate records were checked across all tables.

Special attention was given to:

- Duplicate `customer_id` values in `customers`
- Duplicate `invoice_id` values in `billing`
- Duplicate complete rows

Primary-key uniqueness was treated as an important data-quality validation.

---

### 4. Date Validation

Date fields were validated using the expected:

```text
DD-MM-YYYY
