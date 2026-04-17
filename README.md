# hospital-readmissions-analysis
## Query 1 - State-Level Readmission Performance
## Aggregates average excess readmission ratio by state to identify geographic patterns.
## A ratio above 1.0 means a state is readmitting more patients than expected.
## Query 2 - Worst Performing Conditions Nationally
## Compares all 6 conditions by average excess readmission ratio to determine
## which medical conditions drive the most avoidable readmissions across the country.
## Query 3 - Hospital Rankings Within Each State
## Uses a RANK() window function partitioned by state to rank every hospital
## relative to others in the same state, allowing fair geographic comparisons.
## Query 4 - Hospital Performance Tier Classification
## Uses CASE WHEN to bucket hospitals into performance tiers based on their
## excess readmission ratio, translating raw numbers into actionable risk categories.
## Query 5 - Worst Overall Hospitals Across Multiple Conditions
## Uses a CTE to first calculate each hospital's average ratio across all conditions,
## then filters to only hospitals tracked on 3+ conditions for statistical reliability.
## Query 6 - Gap Between Predicted and Expected Readmission Rates
## Measures how far hospitals deviate from expected performance by state and condition.
## Larger gaps indicate states where hospitals are most consistently underperforming.
## Query 7 - Performance Tier Distribution by Condition
## Uses a window function inside an aggregation to calculate what percentage of
## hospitals fall into each risk tier per condition, revealing which conditions
## have the most systemic performance problems across the entire hospital system.
