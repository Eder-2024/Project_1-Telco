#
Telecom Customer Churn Analysis
Introduction
Ever heard the phrase "irreconcilable differences" in a divorce? Sounds fancy, but let’s be honest—someone just wasn’t happy! Now, imagine that happening in telecom. Customers don’t always say, "It’s not you, it’s me." They just leave—no goodbye, no closure.
So, our team asked the big question: Why do customers suddenly cancel their telecom services? Using real industry data, we analyzed key factors driving churn and developed actionable recommendations for the executive team.

Key Findings
📊 Customer Retention:
•	Out of 7,000+ customers, 27% churned while 73% stayed with the company.
💰 Customer Payment Behaviour:
•	The average monthly charge was $64.80, with some customers paying up to $118.75.
📅 Customer Tenure:
•	Customers stayed for an average of 32 months, ranging from 1 month to 72 months.
•	Longer tenures correlated with lower churn rates.
🛠 Data Quality:
•	The dataset was cleaned, missing values addressed, and irrelevant columns removed.

Business Recommendations
📜 1 – Secure Longer Contracts & Adjust Pricing
Encourage yearly plans with tiered pricing to improve retention and revenue.
✨ 2 – Bundle Additional Services
Offer value-added services (e.g., streaming, tech support) to increase stickiness.
👨‍👩‍👧‍👦 3 – Introduce Family & Senior Plans
Launch affordable family and senior citizen plans to drive multi-line subscriptions and loyalty.


Key Hypothesis Testing & Results
✅ H1: Higher Monthly Charges Increase Churn
•	Churned customers had an average monthly charge of $74 vs. $61 for retained customers.
•	Chi-Square test confirmed a significant correlation (p < 0.05).
✅ H2: Month-to-Month Contracts Have Higher Churn
•	Customers with monthly contracts churned significantly more than those on long-term contracts.
•	Pearson correlation (-0.95) supports this, though p > 0.05.
✅ H3: Longer Tenure Leads to Lower Churn
•	Customers with 60–72 months tenure had the lowest churn.
•	Chi-Square test confirmed a strong correlation.
❌ H4: Senior Citizens Are Less Likely to Churn (Rejected)
•	Senior citizens actually had a higher churn rate (41.68%) than non-seniors (23.65%).
•	Statistically significant (p < 0.001).
✅ H5: Customers with Dependents & Partners Have Lower Churn
•	Family-oriented customers churn less, though results were not statistically significant (p = 1.0).
✅ H6: More Additional Services = Lower Churn
•	Customers with 6+ additional services had the lowest churn (5.28%).
•	Chi-Square test confirmed strong correlation (p < 0.001).

Methods & Tools Used
•	Data Aggregation: groupby, value_counts
•	Visualizations: Pie Charts, Bar Charts, Stacked Columns
•	Statistical Tests: Chi-Square Test, Pearson Correlation
•	Feature Engineering: Tenure binning, Heatmaps
•	Tools: Python (Pandas, Matplotlib), Jupyter Notebook

Conclusion
By analysing churn drivers, we identified key strategies to improve retention. Longer contracts, bundled services, and family-friendly plans can significantly reduce churn and boost revenue. Let’s turn breakups into breakthroughs! 🚀

References
https://pandas.pydata.org/docs/reference/api/pandas.Series.value_counts.html
https://matplotlib.org/stable/gallery/images_contours_and_fields/image_annotated_heatmap.html
Bootcamp: UTOR-VIRT-DATA-PT-12-2024-U-LOLC-MTTHXpert Learning Assistant Chat+
ChatGPT for code debugging when stuck and for refinement

