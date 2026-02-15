
# Customer Segmentation Using RFM Analysis

## Project Overview
This project applies RFM (Recency, Frequency, Monetary) analysis to an online retail dataset in order to segment customers based on purchasing behavior. The objective is to transform transactional data into actionable customer insights for business decision-making.

---

# Data Cleaning & Preparation

The dataset was cleaned to ensure accurate behavioral analysis:

- Removed transactions with missing `CustomerID`
- Excluded returned/cancelled orders (negative quantities)
- Filtered invalid price entries
- Created a new feature: `TotalPrice = Quantity × UnitPrice`

This preprocessing ensured the analysis reflects valid and meaningful purchasing activity.

---

# Exploratory Data Analysis (EDA)

## Distribution of Recency
A histogram of Recency shows a wide spread of customer inactivity levels. 
Some customers purchased recently, while others have been inactive for a long period.

**Insight:** Recency clearly distinguishes active customers from inactive ones, making it a strong predictor of engagement.

---

## Distribution of Frequency
The Frequency distribution is right-skewed. 
Most customers purchase only a few times, while a small percentage make repeated purchases.

**Insight:** Customer engagement is concentrated among a limited group of repeat buyers.

---

## Distribution of Monetary Value
Monetary value is heavily right-skewed.
A small group of customers contributes a disproportionately large share of total revenue.

**Insight:** Revenue concentration follows a Pareto-like pattern common in retail businesses.

---

# RFM Segmentation

Customers were segmented using:

- Recency (days since last purchase)
- Frequency (number of unique invoices)
- Monetary (total revenue contribution)

RFM scores were assigned using quantile-based scoring to classify customers into segments such as:

- Champions
- Loyal Customers
- Potential Loyalists
- At Risk
- Need Attention

---

# Segment-Level Findings

- Champions show low Recency, high Frequency, and high Monetary values.
- Loyal Customers purchase frequently and contribute steady revenue.
- At Risk customers have high Recency and declining engagement.
- Potential Loyalists demonstrate growth potential.

The segmentation logic aligns with expected behavioral patterns, validating the RFM methodology.

---

# Business Insights

1. Revenue is concentrated among a small segment of high-value customers.
2. Recency is a strong indicator of churn risk.
3. High-frequency customers represent strong lifetime value potential.
4. There is a meaningful inactive segment suitable for re-engagement campaigns.

---

# Strategic Recommendations

- Retain Champions through loyalty rewards and exclusive offers.
- Upsell Loyal Customers with premium or bundled products.
- Re-engage At Risk customers with targeted promotions.
- Nurture Potential Loyalists to increase purchase frequency.

---

# Conclusion

This project demonstrates how RFM analysis can convert raw transaction data into structured customer intelligence. 
The segmentation provides a foundation for retention strategy, targeted marketing, and revenue optimization.



