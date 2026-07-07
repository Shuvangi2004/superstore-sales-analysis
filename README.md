# Superstore Sales Analysis — SQL, Python & Tableau

## Business Problem
A retail company wants to understand why profits vary across regions, 
categories, and customer segments, and identify actionable 
recommendations to improve profitability.

## Tools Used
- **SQL** (SQLite) — data extraction and analysis
- **Python** (pandas, matplotlib, seaborn) — EDA and statistical analysis
- **Tableau Public** — interactive dashboard

## Dataset
- Source: Kaggle Superstore Dataset
- 9,994 orders, 21 columns, 2014-2017

## Key Findings
- **Overall profit margin: 12.47%** across $2.3M in total sales
- **West region** leads in total sales; **Central region** significantly 
  underperforms at $8.39 average profit per order vs $31.73 for West
- **Technology** is the most profitable category (15.61% margin); 
  **Furniture** critically low at 3.88%
- **Discount-profit correlation: -0.22** — orders with >40% discount 
  almost always result in negative profit
- **Seasonality:** Sales consistently spike in March, September, 
  and November every year
- **Canon imageCLASS 2200 copier** is the single most profitable 
  product ($25,199 profit)

## SQL Queries Covered
- Basic aggregation (SUM, AVG, COUNT)
- GROUP BY and HAVING
- INNER JOINs across multiple tables
- CTEs (Common Table Expressions)
- Window Functions (RANK, PARTITION BY)
- Date functions (STRFTIME)

## Python Analysis Covered
- Data loading from SQLite using pandas
- Missing value detection
- Statistical summary and skewness analysis
- IQR-based outlier detection
- Correlation analysis
- 5 visualizations (histogram, bar charts, scatter plot, line chart)

## Live Dashboard
View the interactive Tableau dashboard here:
[Superstore Sales Dashboard](https://public.tableau.com/app/profile/shuvangi.bagchi/viz/SuperstoreSalesAnalysisSQLTableau_17834206754380/Dashboard1)

## Project Structure
superstore_project/
├── data/
│   └── superstore.csv
├── sql/
│   └── queries.sql
├── notebooks/
│   └── analysis.ipynb
└── README.md

## How to Run
1. Clone this repository
2. Run `setup_db.py` to load CSV into SQLite
3. Open `sql/queries.sql` in DB Browser for SQLite
4. Open `notebooks/analysis.ipynb` in Jupyter Notebook
