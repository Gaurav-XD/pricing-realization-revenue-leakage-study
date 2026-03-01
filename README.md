# Pricing Realization & Revenue Leakage Study
## Client-Level Financial Performance Diagnostic for Professional Services
## Executive Summary

This project analyzes one year of simulated law firm financial data to diagnose realization performance and identify the root causes of revenue leakage.

## The study evaluates the complete revenue lifecycle:

Billed Revenue → Adjusted Revenue → Collected Revenue
The objective is to determine whether financial performance gaps are driven by pricing discounts or operational collection inefficiencies.

## Business Context

In professional services firms, revenue leakage may occur at multiple stages:
Pricing adjustments (write-offs / write-ups)
Client discounting behavior
Delayed or incomplete collections
Weak credit control governance
Without structured analysis, firms may incorrectly assume pricing strategy is the issue when operational inefficiencies are the primary driver.
This model provides a diagnostic framework to isolate and quantify leakage.

## Data Architecture

The project follows an enterprise-style relational design similar to ERP systems used in professional services firms.
Dimension Tables
Practice Areas
Lawyers (standard rate & cost structure)
Clients
Matters
Fact Tables
Time Entries (revenue generation)
Billing Adjustments (write-offs / write-ups)
Collections (cash realization)
This structure ensures scalability and mirrors real-world financial systems.

## Key Performance Indicators (KPIs)

The model calculates:
Total Billed Revenue
Total Adjusted Revenue
Total Collected Revenue
Billing Realization %
Collection Realization %
Overall Realization %
Discount Loss %
Collection Gap %

## Client Risk Classification

Core Findings

Overall realization: ~54.7%
4 out of 5 clients classified as High Risk
Primary revenue leakage driver: Collection inefficiency
Discount impact present but not dominant
Revenue leakage appears systemic rather than isolated

The analysis indicates that strengthening collection governance may improve profitability more effectively than pricing adjustments alone.

## Executive KPI Snapshot
<img width="1882" height="545" alt="kpi_summary" src="https://github.com/user-attachments/assets/e56388b7-5cfe-450b-8945-7305f5351781" />


## Client-Level Diagnostic Table
<img width="1485" height="253" alt="client_realization_table" src="https://github.com/user-attachments/assets/e38bad31-773b-4fdf-8d33-e913629d40b1" />


## Realization vs Target Benchmark (85%)
Clients are benchmarked against an 85% realization threshold to evaluate performance risk.

<img width="1107" height="372" alt="client_realization_chart" src="https://github.com/user-attachments/assets/222ee5df-d339-4f7e-ab2e-15f88c34ec42" />



## Strategic Recommendations

Implement structured client-level realization monitoring.
Introduce escalation triggers for accounts below 70%.
Strengthen collection follow-up processes.
Separate pricing discipline reviews from credit control governance.

## Tools & Techniques Used

Microsoft Excel
Relational data modeling principles
SUMIF and VLOOKUP logic
Financial KPI diagnostics
Risk classification framework

## Professional Relevance

This project demonstrates applied pricing analytics and revenue leakage diagnostics within a professional services environment.
It reflects the type of financial performance evaluation conducted by pricing and commercial finance teams to support margin governance and operational decision-making.

## What This Project Demonstrates

Pricing analytics capability
Realization diagnostics
Margin leakage identification

Enterprise-style data structuring

Executive-level insight communication
