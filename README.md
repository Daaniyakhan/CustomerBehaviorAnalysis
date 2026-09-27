# Customer Shopping Behavior Analysis

A data analytics project exploring customer shopping behavior across 3,900 retail transactions, using Python, SQL, and Power BI.

## Overview

This project analyzes retail transaction data to understand customer spending patterns, segments, and product preferences. It follows a complete analytics workflow: cleaning and exploring the data in Python, answering business questions with SQL, and visualizing the results in an interactive Power BI dashboard.

## Dataset

**Source:** [Customer Shopping Trends Dataset](https://www.kaggle.com/) (Kaggle)
**Size:** 3,900 transactions · 18 columns
**Fields:** Customer demographics (Age, Gender, Location, Subscription Status), purchase details (Item, Category, Amount, Season, Size, Color), and shopping behavior (Discount Applied, Payment Method, Shipping Type, Review Rating, Frequency of Purchases)

## Tools & Technologies

`Python` (pandas, NumPy, Matplotlib, Seaborn) · `PostgreSQL` · `SQL` · `Power BI` · `Jupyter Notebook`

## Project Structure

```
customer-shopping-behavior-analysis/
├── data/                    # raw dataset (not committed — see .gitignore)
├── notebooks/                # Python data cleaning & EDA
├── sql/                       # business analysis queries
├── powerbi/                  # Power BI dashboard file (.pbix)
├── assets/                   # dashboard screenshot
└── README.md
```

## Methodology

1. **Data Cleaning (Python)** — handled missing values, standardized column names, engineered new features (e.g. age groups), removed redundant columns
2. **SQL Analysis (PostgreSQL)** — wrote queries to answer business questions like revenue by segment, discount impact, and top-performing products
3. **Dashboard (Power BI)** — built an interactive dashboard to visualize customer behavior and revenue trends

## Dashboard

![Customer Behavior Dashboard](assets/powerbi_dashboard.png)

The dashboard shows customer count, average purchase amount, and average review rating at a glance, with breakdowns of revenue and sales by category and age group, subscription status, and filters for gender, category, and shipping type.

## Key Insights

- Non-subscribers account for the majority of revenue and customer base (73%)
- Clothing is the top-performing category by both revenue and sales
- Young Adults generate the highest revenue among all age groups

## How to Run

1. Clone the repo and place the dataset in `data/`
2. Run the notebook in `notebooks/` to clean the data and load it into PostgreSQL
3. Run the queries in `sql/` against the database
4. Open the `.pbix` file in `powerbi/` with Power BI Desktop to explore the dashboard
