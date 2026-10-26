Odoo Project & PowerBI Analytics

## Project Summary  
A Python and Power BI data engineering and business intelligence project automating the extraction, transformation, and reporting of financial data (account.move) from a self-hosted Odoo ERP system. The pipeline extracts invoice records, calculates aging metrics, and visualizes cash flow risks and customer payment behavior across thousands of synthetic invoice transactions.

## Overview

This project bridges transactional ERP operations and executive business intelligence. Using Python (xmlrpc.client, pandas), the pipeline authenticates against Odoo's native XML-RPC web service API, extracts raw customer invoice records, dynamically calculates overdue days based on maturity dates, and structures the output into tabular formats for Power BI analytics. Key analytical capabilities include:

* **Overdue & Risk Tracking:** Quantifying aging parameters per invoice and categorizing records into actionable status buckets (On Track, Overdue by X days).
* **Customer Exposure Analysis:**  Identifying high-risk debtor accounts by aggregating total outstanding balances across major debtors (e.g., Acme Corporation, Azure Interior, AT Company).
* **Temporal Cash Flow Forecasting:** Visualizing monthly invoice due balances to highlight seasonal cash inflow patterns and potential liquidity bottlenecks.

## Data Architecture (Direct Integration Pipeline)

To optimize engineering effort and deliver immediate business value, the solution employs a lean, highly efficient integration architecture connecting directly to Odoo's operational data store:
* **Data Extraction:** Authenticates dynamically using Odoo's common and object XML-RPC endpoints to query the account.move model (filtering by move_type='out_invoice').
* **Transformation:** Utilizes Pandas to clean schema fields, standardize timestamp formats, map payment status markers, and calculate vector-based Days Overdue logic relative to execution dates.
* **Storage & Consumption:** Exports processed records directly to overdue_invoices_report.csv and feeds data directly into Power BI Desktop for interactive visual analytics.

## Tools & Technologies

* **Platform:** VS Code & Power BI
* **Languages:** Python (Pandas), DAX

## Key Odoo Analytics & Insights

Visual 1 (Pending): 
![Pending](Pending)
* **Pending:** Pending.
* **Pending:** Pending.

Visual 2 (Pending): 
![Pending](Pending)
* **Pending:** Pending.
* **Pending:** Pending:
  * **Pending:** Pending.
  * **Pending:** Pending.

Visual 3 (Pending):
![Pending](Pending)
* **Pending:** Pending.
* **Pending:** Pending.
* **Pending:** Pending.


