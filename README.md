# Amazon India Sales — Exploratory Data Analysis

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## Overview

Exploratory data analysis on 128,975 Amazon India sales records to uncover revenue patterns, category performance, and regional demand trends across Indian states and cities.

The goal of this project is to think like a junior data analyst working with an e‑commerce team and use Python to:

- Clean and prepare a raw sales dataset.
- Explore revenue, products, customers and fulfillment behaviour.
- Convert findings into simple, business-focused insights.

---

## Business Questions Answered

- Which product categories generate the highest revenue?
- Which states and cities contribute most to total sales?
- How is sale amount distributed across orders?
- What is the relationship between product size and order value?
- Are there outliers or anomalies in pricing?
- How do different fulfillment types perform?

---

## Key Business Insights

- **Regional revenue concentration:** Maharashtra and Karnataka represent **~40% of total sales volume**. Action: prioritize regional distribution centre (DC) expansion in these hubs to optimise last‑mile delivery cost and delivery time.

- **Fulfillment efficiency:** Amazon‑fulfilled (Easy Ship) orders show around **12% higher fulfillment stability** compared to Merchant‑fulfilled (Mfn) logic, especially in Tier‑2 city segments. This suggests centralised logistics handles variability in smaller cities better than individual merchants.

- **Product performance and reverse logistics:** While “Set” is one of the highest‑volume categories, **small size products** have a disproportionately high **return‑to‑sale ratio**, which points to sizing issues or mismatched expectations. Better size guides, images and product descriptions are needed to reduce reverse logistics cost.

- **Transaction value distribution:** Most transactions fall in the **₹300–₹800** range, which indicates a price‑sensitive customer base with high‑velocity SKUs in the lower‑mid price tier. This band is ideal for bundles, add‑ons and repeat purchase strategies.

You can see supporting charts for these insights in the `images/` folder and inside the EDA notebook.

---

## Project Structure

```text
amazon-sales-eda/
├── data/
│   ├── Amazon_Sale_Report.csv   # Original dataset
│   └── amazon_cleaned.csv       # Cleaned dataset used for EDA
├── notebooks/
│   ├── 01_data_cleaning.ipynb   # Handling missing values and data preparation
│   └── 02_eda_analysis.ipynb    # Exploratory data analysis and visualisations
├── images/                      # Exported charts (categories, states, distribution, correlation etc.)
├── requirements.txt
└── README.md
```

---

## Tools and Libraries

| Tool / Library    | Purpose                          |
|-------------------|----------------------------------|
| Python 3.11       | Core language                    |
| Pandas            | Data cleaning and manipulation   |
| NumPy             | Numerical operations             |
| Seaborn           | Statistical visualisations       |
| Matplotlib        | Chart customisation              |
| Jupyter Notebook  | Development environment          |

---

## Dataset

- **Name:** Amazon India Sales dataset  
- **Size:** 128,975 orders across multiple product categories, sizes and shipping locations in India.  
- **Fields include:** order date, state, city, category, size, sale amount, fulfilment type and other order-level attributes.  

Source: public e‑commerce sales data from [Kaggle](https://www.kaggle.com/).  
In this project I use `Amazon_Sale_Report.csv` as the raw input and create a cleaned version `amazon_cleaned.csv` for analysis.

---

## How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/aalgovind05/amazon-sales-eda.git
   cd amazon-sales-eda
   ```

2. Create a virtual environment (optional but recommended) and install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebooks:

   - Start Jupyter:

     ```bash
     jupyter notebook
     ```

   - Run `notebooks/01_data_cleaning.ipynb` to see how the raw file is cleaned into `amazon_cleaned.csv`.
   - Run `notebooks/02_eda_analysis.ipynb` to explore the EDA, charts and insights.

All key charts are also exported into the `images/` folder.

---

## What I Practised

In this project I focused on:

- Cleaning a real‑world e‑commerce dataset using Pandas.
- Performing EDA with groupby, aggregations and visualisations.
- Segmenting performance by region, product category, size and fulfilment type.
- Turning technical analysis into simple business insights and suggested actions for an e‑commerce team.

---

## Author

**Govind** — Data Analyst  
[GitHub](https://github.com/aalgovind05) • [LinkedIn](https://linkedin.com/in/aal-govind-4b2413279)