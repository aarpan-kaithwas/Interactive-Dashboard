# Customer Retention & Revenue Risk — Interactive Dashboard 

An interactive data visualization dashboard built for **Task 5 (Interactive Dashboard Development)** of the **VirtualWorks Data Analytics Internship**. The dashboard analyzes customer churn behavior, monthly recurring revenue (MRR) exposure, and subscriber lifecycle trends across **7,043 telecom customer records** (`Telco-Customer-Churn.csv`).

---

* **Interactive Notebook:** `Interactive_Dashboard.ipynb`
* **Dataset:** `Telco-Customer-Churn.csv`

---

## Dashboard Design Principles Applied
This dashboard follows core data visualization best practices to ensure clarity at a glance:
1. **Top-Left KPI Hierarchy:** Places primary metrics (**Churn Rate**, **Monthly Revenue Lost**, and **Average Tenure**) at the top with rounded numbers and baseline comparisons.
2. **High Data-Ink Ratio:** Uses a clean white template (`plotly_white`) with gridlines and visual clutter removed so data values stand out immediately.
3. **High-Clarity Chart Selection:** Uses vertical/horizontal bar charts and a continuous tenure line chart rather than pie or area charts for accurate visual comparison.
4. **Native Interactive Filtering:** Includes an embedded dropdown selector (`Contract | Internet Service`) that dynamically updates all KPI cards and charts in real time.

---

## Key Metrics & Findings (Overall Baseline)
* **Overall Churn Rate:** **26.5%** (1,869 of 7,043 customers)
* **Monthly Revenue Lost:** **$139,131** in churned subscriber MRR
* **Average Customer Tenure:** **32.4 months**

### Actionable Business Insights
1. **Month-to-Month Contract Risk:** Month-to-month subscribers churn at **42.7%**, compared to **11.3%** for one-year and **2.8%** for two-year contracts. Offering targeted 1-year upgrade incentives during the first 6 months addresses the largest retention driver.
2. **Early Lifecycle Drop-Off:** Churn peaks during the first **1–5 months** of tenure and stabilizes after month 24, making proactive onboarding check-ins during the first 90 days critical.
3. **Payment Friction & Fiber Optic Segment:** Customers paying via **Electronic Check** (**45.3%** churn) and **Fiber Optic** internet users (**41.9%** churn) carry the highest revenue exposure and should be prioritized for auto-pay enrollment and service quality outreach.

---

## Project Structure
```text
├── Interactive_Dashboard.ipynb   # Data cleaning, interactive Plotly dashboard, and insights
├── Telco-Customer-Churn.csv      # Raw customer churn dataset (7,043 rows, 21 columns)
└── README.md                     # Project documentation and findings
