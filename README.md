# India E-Commerce — Sales & Customer Analytics (Python)

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-Interactive-3F4F75?logo=plotly&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

An end-to-end **Python analytics project** on Indian e-commerce sales data — from raw CSV to a cleaned dataset and exploratory insights across sales, customers, products, payments, delivery and ratings.

> 🎯 **Pipeline:** Load → Clean → Validate → Standardise → Explore → Visualise → Export

---

## 📑 Sections

### 🧠 1 — Business Problem
Defines the core questions: *what sells, where, to whom, how customers pay, and how the business is performing?*

### 📁 2 — Dataset & Dictionary
A single transactions table (~29 columns) covering orders, customers, products, pricing, payments, delivery and ratings — with a data dictionary documenting every field.

### 🛠️ 3 — Technologies Used
`Python`  `pandas` / `numpy` for wrangling  `matplotlib` for static charts  `plotly.express` for interactive charts  `Jupyter` notebook.

### 🧹 4 — Data Loading & Inspection
- Load `india_ecommerce_sales.csv`
- Inspect **shape, columns, dtypes**
- Check **nulls** and **duplicates**
- Statistical summaries (`describe`) for numeric and text columns

### 🧽 5 — Data Cleaning & Quality
- Drop nulls and duplicate rows
- Convert `Order_Date` → datetime; `Age`, `Delivery_Days` → integer
- Remove invalid records: `Quantity <= 0`, `Age > 100`, ratings outside 1–5
- Fix price outliers (e.g., an erroneous `Unit_Price` corrected)

### 🔤 6 — Text Standardisation
- Strip whitespace and apply title case to text columns
- Standardise categories: `F/M` → `Female/Male`  `Cod` → `Cash On Delivery`

### 💾 7 — Export
Writes the cleaned dataset to **`Clean_sales_ecommerce.csv`** — ready for BI tools (Power BI / Tableau).

### 📊 8 — Exploratory Analysis
| Analysis | What it answers |
|---|---|
| 🗂️ Category | Top categories by sales |
| 🌏 Region & State | Where revenue concentrates |
| 💳 Payment Method | How customers pay |
| 📦 Order Status | Fulfilment health |
| 🏆 Products | Top 10 by revenue and by profit |
| 📅 Time | Sales by year |
| 📱 Device Type | Where orders originate |
| ⭐ Ratings | Best- and worst-rated products |

**Visuals:** bar charts (category, region), pie charts (payment, order status, device), Plotly interactives — all styled with a custom navy palette.

---

## 🚀 Run It

```bash
pip install pandas numpy matplotlib plotly jupyter
jupyter notebook E-Commerce_Project.ipynb
```

Run cells top-to-bottom — the notebook loads the raw CSV, cleans it, runs the analysis, and writes `Clean_sales_ecommerce.csv` at the end.

---

## 📁 Project Structure

```
├── E-Commerce_Project.ipynb      # Full analysis notebook
├── india_ecommerce_sales.csv     # Raw input data
├── Clean_sales_ecommerce.csv     # Cleaned output
├── requirements.txt
└── README.md
```

---

## 💡 Key Takeaways

1. 🧹 The raw data needed real cleaning — nulls, duplicates, invalid quantities, age anomalies and price outliers were all handled.
2. 📏 A documented, repeatable pipeline turns messy CSVs into analysis-ready data.
3. 📊 The cleaned output feeds directly into the Power BI dashboard — Python for preparation, BI for presentation.
4. ⭐ Product ratings and profit rankings surface both the winners and the underperformers.

---

## 👤 Author

**Saloni Jain** — data cleaning, quality validation, exploratory analysis and visualisation.
