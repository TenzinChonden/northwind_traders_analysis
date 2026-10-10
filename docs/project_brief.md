# Project Brief: Northwind Traders Customer & Revenue Optimization Analysis

**To:** Data Analytics Team  
**From:** Director of Sales & Strategy, Northwind Traders  
**Subject:** Q3 Commercial Performance & Customer Behavior Deep-Dive  

## Project Overview
Northwind Traders is preparing its commercial strategy for the upcoming fiscal year. Executive leadership is concerned that our marketing spend and inventory management are too generalized. We need a comprehensive data-driven evaluation of our historical customer purchasing behaviors, regional sales patterns, and product portfolio performance to maximize revenue and protect customer retention.

As our Analytics Lead for this project, you are tasked with querying our enterprise database, transforming the data, and delivering actionable business insights that answer critical commercial questions.

---

## Key Objectives & Resume-Ready Business Questions
Your analysis must provide definitive, data-backed answers to the following three core business pillars:

### 1. Customer Segmentation & Value (The RFM Framework)
* **Business Goal:** Identify our most valuable clients to protect against churn and target high-ROI loyalty campaigns.
* **Core Questions to Answer:**
  * Who are our top 10% highest-value customers based on total historical spend?
  * What is the distribution of customer purchasing frequency, and how many days on average elapse between repeat orders?
  * Can we segment our customer base into distinct tiers (e.g., VIP, Regular, At-Risk) using Recency, Frequency, and Monetary (RFM) metrics?

### 2. Product Portfolio & Margin Optimization
* **Business Goal:** Optimize inventory holding costs by identifying top revenue drivers versus underperforming stock.
* **Core Questions to Answer:**
  * Which product categories drive the highest gross revenue, and how do profit margins vary across categories when accounting for historical unit pricing and discounts?
  * Are there "dead weight" products that have low sales volume and high inventory levels tying up working capital?
  * Which specific products experience seasonal demand spikes or clusters in specific geographic regions?

### 3. Geographic & Shipping Efficiency
* **Business Goal:** Evaluate regional sales performance and logistics cost efficiency.
* **Core Questions to Answer:**
  * Which destination countries or cities generate the highest total freight costs relative to order values?
  * How do shipping lead times (time elapsed between order date and shipped date) vary across different shipping partners (`Shippers`), and does fulfillment speed impact customer re-order rates?

---

## Recommended Technical Workflow
To complete this analysis successfully, you are expected to execute the following pipeline:
1. **Extraction (SQL):** Write efficient, optimized SQL queries leveraging `pd.read_sql_query()` and your local SQLite database to pull pre-aggregated datasets (avoiding unnecessary memory overhead).
2. **Transformation & Cleaning (Pandas):** Handle missing values, parse datetime strings into usable timestamps, and compute derived columns (like line-item totals and delivery lead times).
3. **Exploratory Analysis & Aggregation:** Group, pivot, and calculate statistical summaries to surface insights.
4. **Visualization:** Produce clear charts using Matplotlib or Seaborn to illustrate your findings for executive stakeholders.

---

## Expected Project Deliverables for Your Portfolio / Resume
Upon completion, you should be able to feature this project on your resume with high-impact bullet points such as:
* *Engineered an end-to-end retail analytics pipeline in Python and SQL to evaluate 800+ customer records and multi-year order histories.*
* *Implemented an RFM (Recency, Frequency, Monetary) segmentation model to identify top-tier enterprise clients, driving targeted retention recommendations.*
* *Analyzed product portfolio profitability and shipping logistics efficiency, uncovering inventory bottlenecks and optimizing regional distribution metrics.*