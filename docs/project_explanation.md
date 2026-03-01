# Project Explanation
## Overview

This project simulates one year of financial activity for a professional services firm and analyzes revenue realization performance at both firm and client levels.
The model evaluates the full revenue lifecycle:
Billed Revenue (from time entries)
Adjusted Revenue (after write-offs/write-ups)
Collected Revenue (cash received)

The objective is to diagnose where revenue leakage occurs and determine whether the primary driver is pricing discipline or collection inefficiency.

## Data Flow

The project follows a relational data structure:

Practice Areas → Lawyers → Matters → Time Entries
Matters → Billing Adjustments
Matters → Collections

Time entries generate billed revenue.
Billing adjustments modify invoice value.
Collections reflect actual cash received.

This layered structure mirrors enterprise ERP systems used in professional services firms.

## Revenue Calculation Logic
1. Billed Revenue

Calculated as:

Hours Worked × Standard Hourly Rate
Rates are pulled dynamically from the lawyers table using lookup logic.

2. Adjusted Revenue

Calculated as:

Billed Revenue + Billing Adjustments

Write-offs are recorded as negative values.
Write-ups are recorded as positive values.

3. Collected Revenue

Summed from the collections table based on matter-level cash receipts.

## Realization Metrics
Billing Realization %

Adjusted Revenue ÷ Billed Revenue
Measures pricing discipline impact.

Collection Realization %

Collected Revenue ÷ Adjusted Revenue
Measures credit control effectiveness.

Overall Realization %

Collected Revenue ÷ Billed Revenue
Measures total revenue conversion efficiency.

## Client Risk Classification

Clients are classified based on overall realization:

≥ 85% → Healthy
70%–85% → Moderate Risk
< 70% → High Risk

This classification framework helps prioritize performance improvement efforts.

## Key Insight

The analysis demonstrated that collection inefficiencies were the dominant contributor to low realization rather than discounting behavior.
This distinction is critical for determining whether corrective action should focus on pricing strategy or operational credit control.
