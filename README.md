# Telecom Customer Churn Analysis  

## **Introduction**  
Ever heard the phrase *"irreconcilable differences"* in a divorce? I am sure you have as this is the common excuse used, but let’s be honest—someone just wasn’t happy!  

Now, imagine that happening in telecom. Customers don’t always say, *"It’s not you, it’s me."* They just leave—no goodbye, no closure.  

So, our team asked the big question:  
**Why do customers suddenly cancel their telecom services?**  

Using real industry data, we analyzed key factors driving churn and developed actionable recommendations for the Board.  

---

## **Key Findings**  

📊 **Customer Retention:**  
- Out of **7,000+ customers**, **27% churned**, while **73% retained** with the company.

![ChurnDistribution](https://github.com/Eder-2024/Project_1-Telco/blob/main/Plot/ChurnDistribution.png) 

💰 **Customer Payment Behavior:** 
- The **average monthly charge** was **$64.80**, with some customers paying up to **$118.75**.  

📅 **Customer Tenure:**  
- Customers stayed for an average of **32 months**, ranging from **1 month to 72 months**.  
- **Longer tenures correlated with lower churn rates.**  

🛠 **Data Quality:**  
- The dataset was cleaned, missing values addressed, and irrelevant columns removed.  

---

## **Business Recommendations**  

📜 **1 – Secure Longer Contracts & Adjust Pricing**  
Encourage **yearly plans** with tiered pricing to improve retention and revenue.  

✨ **2 – Bundle Additional Services**  
Offer **value-added services** (e.g., streaming, tech support) to increase retention.  

👨‍👩‍👧‍👦 **3 – Introduce Family & Senior Plans**  
Launch **affordable family and senior citizen plans** to drive multi-line subscriptions and loyalty.  

---

## **Key Hypothesis Testing & Results**  

✅ **H1: Higher Monthly Charges Increase Churn**  
- Churned customers had an **average monthly charge of $74** vs. **$61 for retained customers**.  
- **Chi-Square test confirmed** a significant correlation (p < 0.05).  

✅ **H2: Month-to-Month Contracts Have Higher Churn**  
- Churn rate:   **monthly contract - 42.7% , one year contract - 11.2%,  two year contract -2.8%**. 
- Customers with **monthly contracts churned significantly more** than those on **long-term contracts**.
- **Pearson correlation (-0.95) supports this, though p > 0.05.**  

![Contract Type Churn Rate](https://github.com/Eder-2024/Project_1-Telco/blob/main/Plot/Contract%20Type%20Churn%20Rate.png)

✅ **H3: Longer Tenure Leads to Lower Churn**  
- Customers with **60–72 months tenure had the lowest churn**.  
- **Chi-Square test confirmed a strong correlation.**

![Tenure vs. Churn](https://github.com/Eder-2024/Project_1-Telco/blob/main/Plot/Tenure%20vs%20Churn.png)

❌ **H4: Senior Citizens Are Less Likely to Churn (Rejected)**  
- **Senior citizens actually had a higher churn rate (41.68%)** than non-seniors (23.65%).  
- **Statistically significant (p < 0.001).**

![Churn Proportion for Non-Senior Citizens](https://github.com/Eder-2024/Project_1-Telco/blob/main/Plot/Churn%20Proportion%20for%20Non-Senior%20Citizens.png)

![Churn Proportion for Senior Citizens](https://github.com/Eder-2024/Project_1-Telco/blob/main/Plot/Churn%20Proportion%20for%20Senior%20Citizens.png)

![Churn Proportion Bar](https://github.com/Eder-2024/Project_1-Telco/blob/main/Plot/Churn%20Proportion%20Bar.png)

✅ **H5: Customers with Dependents & Partners Have Lower Churn**  
-   Churn rate for **customers with family** is 19.9% compared to 34.2% **without family**.
- **Family-oriented customers churn less**, though results were **not statistically significant** (p = 1.0).


![Family Churn Rate](https://github.com/Eder-2024/Project_1-Telco/blob/main/Plot/Family%20Churn%20Rate.png) 

✅ **H6: More Additional Services = Lower Churn**  
- Customers with **6+ additional services had the lowest churn (5.28%)**.  
- **Chi-Square test confirmed strong correlation (p < 0.001).**  

![Number of Additional ervices vs. Churn](https://github.com/Eder-2024/Project_1-Telco/blob/main/Plot/Number%20of%20Additional%20Services%20vs%20Churn.png)
---

## **🌟Additional Analysis - Bonus** 
We conducted a correlation heatmap analysis of monthly charges, total charges, and tenure. 
The results revealed a positive correlation, indicating that as monthly charges and tenure increase, total charges also rise.



![Correlation Heatmap of Numerical Features](https://github.com/Eder-2024/Project_1-Telco/blob/main/Plot/Correlation%20Heatmap%20of%20Numerical%20Features.png)

---

## **🔍Conclusion**  

By analyzing churn drivers, we identified key strategies to improve retention.  
**Longer contracts, bundled services, and family-friendly plans** can significantly reduce churn and boost revenue.  

Let’s turn **breakups into breakthroughs!** 🚀  

---


📝 **NOTE**: While the findings provide valuable insights, the dataset of over 7,000 customers may not fully represent the broader customer base. It doesn’t account for factors like geography, income, or service plans, and the analysis is based on a specific time period, making it less generalizable. Additionally, customer behavior may fluctuate over time, and external factors such as market conditions or competition are not considered, which could impact churn in ways not reflected in the data.

---

## **🔧Methods & Tools Used**  

- **Data Aggregation:** `groupby`, `value_counts`  
- **Visualizations:** Pie Charts, Bar Charts, Stacked Columns  
- **Statistical Tests:** Chi-Square Test, Pearson Correlation  
- **Feature Engineering:** Tenure binning, Heatmaps  
- **Tools:** Python (Pandas, Matplotlib), Jupyter Notebook  

---

## **💻Installation guide and usage instructions**
```
#Clone the repository
git clone https://github.com/Eder-2024/Project_1-Telco.git

#Launch in Jupyter Notebook
jupyter Main_Code Main_Code.ipynb
```

---

## **📚References** 
- [Telco Customer Churn Dataset on Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)  
- [Pandas value_counts Documentation](https://pandas.pydata.org/docs/reference/api/pandas.Series.value_counts.html)  
- [Matplotlib Annotated Heatmap Example](https://matplotlib.org/stable/gallery/images_contours_and_fields/image_annotated_heatmap.html)  
- Bootcamp: UTOR-VIRT-DATA-PT-12-2024-U-LOLC-MTTH Xpert Learning Assistant Chat+ 
- ChatGPT for code debugging when 

---

## **👥Collaborators**
1.	Demilade Adenuga (In charge of coding, developing visualizations, and writing summaries)
2.	Geraldine Valencia (In charge of coding and generating visualizations)
3.	Eder Ortiz (In charge of coding, data cleaning, and generating visualizations)

---

 ## **🛡️License**
 Data files © Original Authors - BlastChar


