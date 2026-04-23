# Amazon India Sales — Exploratory Data Analysis

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)
![Status](https://img.shields.io/badge/Status-In%20Progress-orange)

## Overview
Exploratory data analysis on 128,975 Amazon India sales records
to uncover revenue patterns, category performance, and regional
demand trends across Indian states and cities.

## Business Questions Answered
- Which product categories generate the highest revenue?
- Which states and cities contribute most to total sales?
- How is sale amount distributed across orders?
- What is the relationship between product size and order value?
- Are there outliers or anomalies in pricing?

### Key Business Insights

* **Regional Revenue Concentration:** Maharashtra and Karnataka represent **~40% of total sales volume**. Action: Prioritize regional distribution center (DC) expansion in these hubs to optimize last-mile delivery costs.
* **Fulfillment Efficiency:** Amazon-fulfilled (Easy Ship) orders maintain a **12% higher fulfillment stability** compared to Merchant-fulfilled (Mfn) logic, specifically in Tier-2 city segments.
* **Product Performance & Reverse Logistics:** While 'Set' is the highest-volume category, 'Small' size products exhibit a disproportionate **return-to-sale ratio**, suggesting a need for sizing-guide calibration to reduce operational leakage.
* **Transaction Value Distribution:** The majority of transactions are concentrated in the ₹300–₹800 range, indicating a highly price-sensitive customer base with high-velocity SKU potential in the lower-mid tier.

## Project Structure
amazon-sales-eda/
│
├── data/
│   ├── Amazon_Sale_Report.csv   # Original dataset
│   └── amazon_cleaned.csv       # Cleaned version
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   └── 02_eda_analysis.ipynb
│
├── images/                      # Chart exports
├── requirements.txt
└── README.md


## Tools & Libraries
| Tool | Purpose |
|------|---------|
| Python 3.11 | Core language |
| Pandas | Data cleaning & manipulation |
| NumPy | Numerical operations |
| Seaborn | Statistical visualizations |
| Matplotlib | Chart customization |
| Jupyter Notebook | Development environment |

## Dataset
Amazon India Sales dataset — 128,975 orders across multiple
categories, sizes, and shipping locations across India.
Source: [Kaggle](https://www.kaggle.com/)

## Author
**Govind** — Data Analyst
[GitHub](https://github.com/aalgovind05)