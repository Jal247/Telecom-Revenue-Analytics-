# Telecom-Revenue-Analytics
End-to-end analytics pipeline investigating telecom subscriber churn and revenue protection. Features diagnostic data validation, automated python cleansing, and executive performance dashboards.

# Telecom Revenue & Subscriber Churn Analytics Pipeline

## Business Scenario & Problem Statement
In the telecommunications sector, sustaining subscriber revenue requires a tight balance between managing customer churn and maintaining backend data integrity. In this enterprise simulation, a telecom provider is experiencing unexplained revenue fluctuations alongside a baseline customer churn rate. 

The core challenge is a classic diagnostic problem: **Is the revenue drop strictly due to customer attrition, or are backend billing logic gaps causing systemic revenue leakage?**

This project approaches the problem by treating data analytics as an end-to-end pipeline. It moves from raw, unverified transactional records to a structured, validated data model, culminating in an executive-facing Business Intelligence solution.

---

## Project Objectives & Core KPIs
To address the business problem, the analytics pipeline is designed to deliver:
*   **Data Integrity Auditing:** Identify and log database anomalies, missing transactional values, and calculation logic failures within billing records.
*   **Automated Data Engineering:** Build a reproducible Python pipeline to clean, transform, and segment customer profiles.
*   **Executive Business Intelligence:** Architect an interactive multi-page dashboard tracking key performance indicators (KPIs).

### Primary Metrics Tracked:
1.  **Churn Rate (%)**: Total customers lost within a specific period divided by the total active subscriber base.
2.  **Monthly Recurring Revenue (MRR) at Risk**: Total monthly billings tied to subscribers flagged with high churn propensity.
3.  **Data Logic Discrepancy Rate (%)**: Percentage of customer billing records where calculated lifetime values do not mathematically match recorded metrics.
4.  **Year-over-Year (YoY) / Month-over-Month (MoM) Churn Trends**.

---

## Repository Architecture
The pipeline is strictly segmented into modular environments to maintain clean code and professional project hygiene:

```text
telecom-revenue-analytics/
│
├── .gitignore               # Excludes system cache, local environments, and temporary files
├── README.md                # Project overview, strategic business framework, and takeaways
│
├── documentation/           # Agile requirement mapping, user stories, and data dictionaries
│
├── data/                    # Data architecture layer
│   ├── raw_data/            # Source landing zone for the uncleaned dataset
│   └── cleaned_data/        # Processed target layer exported by the automated pipeline
│
├── sql_scripts/             # Week 1: Anomaly detection, CTEs, and query architecture
│
├── python_pipelines/        # Week 2: Pandas script for profiling, cleaning, and segmentation
│
└── bi_dashboards/           # Week 3: Power BI / Tableau files and executive UI screenshots
