# Retail Sales Analytics

Analysis of retail POS (point-of-sale) data — covering data cleaning, sales trends,
market basket analysis, and brand performance.

## 📊 Dataset

**Raw data:** 131,265 transactions, 10 columns (Bill No, Date, Product, Qty, Rate, Amount, Total, etc.)
**After cleaning:** 130,553 transactions, 13 columns (added Year, Month, Weekday, Sales Category)

Cleaning steps: removed junk/service entries, validated Amount = Qty × Rate, dropped missing values, removed duplicates

## 🗂️ Project Structure

retail-sales-analytics/
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda_and_kpis.ipynb
│   ├── 03_market_basket_analysis.ipynb
│   └── 04_brand_analysis.ipynb
└── README.md

## 📓 What Each Notebook Does

**1. Data Cleaning** — cleans raw POS data, fixes missing values, engineers date/category features.

**2. EDA & KPIs** — sales trends, top products, and Pareto (80/20) analysis.
👉 998 products (21.6%) generate 80% of total revenue.

**3. Market Basket Analysis** — finds which products are frequently bought together using the Apriori algorithm.
👉 Strongest pairings found in grocery/spice combos, useful for cross-sell recommendations.

**4. Brand Analysis** — extracts brand names from product text and compares brand performance.
👉 ARUN leads revenue (₹2.4L), GOLDWINNER is the most premium (avg ₹161/item), AROKYA has the highest footfall (4,760 bills).

## 🛠️ Tools Used

1. Python pandas
2. numpy
3. matplotlib
4. seaborn
5. mlxtend
6. Jupyter Notebook
