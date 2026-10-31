# superstore-sales-analysis
   # Superstore Sales Analysis

**Why is a store with $2.3M in sales keeping only 12.5% as profit, and what should it change?**

I analyzed 9,994 retail orders (2014–2017) from a US superstore to find what drives sales and profit, segmented its customers with RFM analysis, and turned the findings into business recommendations.

**Tools:** Python · pandas · NumPy · SQL (SQLite) · Matplotlib · Google Colab

## Key findings

| # | Finding |
|---|---|
| 1 | **Discounts drive losses.** Undiscounted orders earn a **29.5%** margin; orders discounted above 40% run at **–77.4%**. |
| 2 | **3 sub-categories lose money**, led by **Tables (–$17,725)**. |
| 3 | **Technology** is the most profitable category: **$145,455** profit at a **17.4%** margin. |
| 4 | **West** is the most profitable region; **Central** is the weakest at a **7.9%** margin. |
| 5 | Sales **peak in November**, a clear seasonal pattern. |
| 6 | The **top 20% of customers generate 48%** of sales. The **Consumer** segment brings the most sales ($1.16M). |
| 7 | **RFM:** 176 Champions drive **35.0%** of sales, but **217 At-Risk customers** (avg 213 days since last order) hold **37.3%**, more than the Champions. |

## Recommendations

1. **Cap discounts at around 20%.** Deep discounts turn orders unprofitable.
2. **Review pricing and costs for Tables** and the other loss-making sub-categories.
3. **Investigate the Central region** and the least profitable states, especially their discount levels.
4. **Plan inventory and campaigns ahead of November.**
5. **Run a win-back campaign for At-Risk customers.** They hold over a third of sales and haven't ordered in about 7 months.
6. **Reward Champions** with a loyalty programme to protect their revenue.

## What I did

1. **Checked data quality:** 9,994 rows, 21 columns, no missing values or duplicates; dates were stored as text.
2. **Cleaned the data:** standardized column names, converted dates, added year, month, profit margin and days-to-ship columns.
3. **Explored the data with pandas:** sales and profit by category, sub-category, region, state, month and discount band.
4. **Queried with SQL:** loaded the data into SQLite and compared customer segments and top customers with GROUP BY queries.
5. **Segmented customers with RFM:** scored each customer on Recency, Frequency and Monetary value, and grouped them into Champions, Loyal, Promising, At Risk and Lost.
6. **Wrote insights and recommendations** from the results.

## Dataset

[Superstore Dataset on Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final): 9,994 rows, 21 columns.

## How to run

Open `Superstore_Sales_Analysis.ipynb` in Google Colab, click **Runtime → Run all**, and upload the dataset zip when prompted.

---
**Author:** Anies Faizie · [GitHub](https://github.com/aaniesfaizie-ship-it)
