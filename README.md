# Hospital Readmissions Analysis

## Overview
An end-to-end SQL, Python, and Power BI analysis of U.S. hospital readmission rates using CMS Hospital Readmissions Reduction Program (HRRP) data. The project investigates which states, hospitals, and medical conditions drive excess readmissions across 18,330 hospital-condition records.

**Business Question:** Which hospitals and conditions drive excess readmissions, and what patterns predict poor performance?

## Dataset
- **Source:** Centers for Medicare & Medicaid Services (CMS)
- **Link:** https://data.cms.gov/provider-data/dataset/9n3s-kdb3
- **Records:** 18,330 hospital-condition pairs
- **Conditions Tracked:** AMI, COPD, Heart Failure, Pneumonia, Hip/Knee, CABG
- **Performance Period:** July 2021 – June 2024

## Tools & Technologies
- Python (pandas, matplotlib, seaborn)
- SQL (SQLite)
- Jupyter Notebook
- Power BI (interactive dashboard)

## Key Findings
1. **Massachusetts, New Jersey, and Florida** are the worst performing states for excess readmissions nationally
2. **Hip/Knee replacements** have the highest proportion of High Risk hospitals at 23%, more than any other condition
3. **Oroville Hospital (CA)** and **Winchester Hospital (MA)** are the worst overall performers when averaged across multiple conditions
4. Massachusetts appears consistently across every analysis — state-level averages, rate gaps, and worst hospital rankings — suggesting a systemic issue rather than isolated poor performers
5. **COPD** has the most evenly distributed performance of any condition, with only 2.88% of hospitals classified as High Risk

## SQL Concepts Demonstrated
- Aggregations and GROUP BY
- Window functions (RANK, SUM OVER, PARTITION BY)
- Common Table Expressions (CTEs)
- CASE WHEN performance tier classification
- Multi-condition filtering and NULL handling

## How to Run
1. Download the dataset CSV from the link above
2. Clone this repository and open the notebook in Jupyter
3. Update the file path in the first cell to point to your downloaded CSV
4. Run all cells in order
