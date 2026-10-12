# Northwind Traders Operational & Logistics Analysis

## Background on Northwind Traders Data
The Northwind Traders dataset is a classic, widely recognized sample database originally created by Microsoft. It represents a fictional specialty foods export-import enterprise—Northwind Traders—tracking comprehensive transactional and operational data. The dataset captures inventory, orders, customer details, suppliers, shipping logistics, and employee territories, making it a standard benchmark for relational database querying, data engineering, and business intelligence analytics.

---

## Repository Structure & Notebooks

This repository contains a multi-part operational analysis of the Northwind database, broken down into distinct analytical workflows:

### 1. Margin & Revenue Optimization (`Margin_Optimization.ipynb`)
* **Objective:** Evaluate top-performing product categories, pricing strategies, and inventory health.
* **Key Insights:** 
  * Beverages leads total portfolio performance with $93.66M in gross revenue across 15,216 orders.
  * Meat/Poultry and Confections follow closely as top revenue drivers, generating $66.96M and $66.94M respectively.
  * Average unit prices reach their highest in Meat/Poultry at $53.96 and Beverages at $37.90.
  * Demand analysis reveals consistent seasonal volume surges across categories during late summer, peaking notably in August (e.g., Beverages reaching 225,827 units and Confections hitting 243,368 units).

### 2. Geographic & Shipping Efficiency (`Geographic__Shipping_Effeciency.ipynb`)
* **Objective:** Examine regional shipping overhead, freight-to-revenue ratios, and carrier performance.
* **Key Insights:** 
  * Proximity drives extreme cost efficiency, with Belgium achieving the lowest freight cost ratio relative to order value at approximately 0.94%.
  * Across the three primary carriers (Federal Shipping, Speedy Express, and United Package), fulfillment performance is tightly clustered, averaging between 7.21 and 7.45 days with median delivery speeds sitting at 5 to 6 days.
  * Carriers manage heavy volumes ranging from 5,400 to 5,600 orders each, though maximum lead time outliers reach up to 35 to 37 days due to transit or stock bottlenecks.

### 3. Executive Synthesis & Reporting
* **Objective:** Consolidate findings from product portfolio health and fulfillment operations into actionable operational recommendations for supply chain and inventory management.

---

## Tech Stack
* **Python:** Pandas, NumPy, Matplotlib, Seaborn
* **Database & SQL:** Relational querying via SQLAlchemy and SQLite
* **Environment:** Jupyter Notebooks
