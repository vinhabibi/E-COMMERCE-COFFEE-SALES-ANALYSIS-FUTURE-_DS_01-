# E-Commerce Coffee Shop Sales Analysis

## Overview

This repository contains a dataset and a Power BI dashboard for analyzing sales data from an e-commerce coffee shop. The dashboard provides key insights into transaction metrics, revenue trends, peak sales periods, and performance by coffee type, time of day, day of week, and month. The data covers transactions from **March 2024 to March 2025**, focusing on various coffee products and sales patterns.

The project is designed to help understand customer behavior, optimize inventory, and identify growth opportunities in an online coffee retail business.

---

## Dataset

The dataset is stored in [`Coffe_sales.csv`](Coffe_sales.csv), a CSV file containing transaction-level data. It includes **thousands of records** spanning over a year.

### Columns
| Column        | Description |
|---------------|-----------|
| `hour_of_day` | Hour of transaction (0–23) |
| `cash_type`   | Payment method (e.g., `card`) |
| `money`       | Transaction amount |
| `coffee_name` | Coffee type (e.g., `Latte`, `Americano`) |
| `Time_of_Day` | Categorized time: `Morning`, `Afternoon`, `Night` |
| `Weekday`     | Day of week (e.g., `Fri`, `Sat`) |
| `Month_name`  | Month name (e.g., `Mar`) |
| `Weekdaysort` | Sort order for weekdays (1 = Mon, 7 = Sun) |
| `Monthsort`   | Sort order for months |
| `Date`        | Transaction date (`YYYY-MM-DD`) |
| `Time`        | Transaction time (`HH:MM:SS`) |

### Sample Data
| hour_of_day | cash_type | money | coffee_name       | Time_of_Day | Weekday | Month_name | Date       | Time            |
|-------------|-----------|-------|-------------------|-------------|---------|------------|------------|-----------------|
| 10          | card      | 38.7  | Latte             | Morning     | Fri         | Mar        | 2024-03-01 | 10:15:50.520000 |
| 12          | card      | 38.7  | Hot Chocolate     | Afternoon   | Fri         | Mar        | 2024-03-01 | 12:19:22.539000 |
| 19          | card      | 33.8  | Americano with Milk | Night     | Sun         | Mar        | 2024-03-03 | 19:23:15.887000 |

---

## Dashboard (Power BI)

The interactive dashboard is built in **Power BI** and consists of **two pages** with filters for **year** and **month**.

### Page 1: Executive Summary
**Key Metrics:**
- **Average Transaction Value**: `$31.65`
- **Monthly Sales**: `1,122.5K`
- **Peak Hour**: `10 AM`
- **Total Revenue**: `1,122.5K`
- **Total Transactions**: `4K`

**Visuals:**
- Revenue by Coffee Type (Bar)
- Sales by Hour of Day (Weekday)
- Daily Sales Trend (This Week)
- Detailed sales table by Time of Day & Weekday

---

### Page 2: Deep Dive
**Visuals:**
- **Sales Distribution by Time of Day** (Pie Chart)
  - Morning: 32.01%  
  - Afternoon: 34.02%  
  - Night: 33.97%
- **Top Coffee Types by Revenue** (Horizontal Bar)
- **Average Order Value (AOV) by Day of Week**
- **Monthly Sales Trend**
- **Revenue vs. Transactions by Coffee Type** (Combo Chart)

---

## Key Insights

| Insight | Recommendation |
|-------|----------------|
| **Latte & Cappuccino** dominate revenue | Promote bundles or loyalty for these items |
| **Peak at 10 AM** across weekdays | Increase staffing & inventory during morning rush |
| **Even distribution** across Morning/Afternoon/Night | Maintain 24/7 online availability |
| **March & October** highest sales | Plan promotions during high seasons |
| **Card-only payments** | No cash handling — streamline operations |

---
2. Open in Power BI

Download Power BI Desktop (free): https://powerbi.microsoft.com/desktop/
Open Coffee Shop Sales Dashboard.pbix (or import Coffe_sales.csv)
Explore filters and drill-throughs

3. Optional: Python Analysis
bashpip install pandas matplotlib seaborn
python analysis.py

Project Structure
textcoffee-shop-sales-analysis/
├── Coffe_sales.csv              # Raw transaction data
├── Coffee Shop Sales Dashboard.pbix  # Power BI file (optional)
├── screenshots/
│   ├── page1.png
│   └── page2.png
├── analysis.py                  # Sample Python script
└── README.md                    # This file

Contributing
We welcome contributions! To contribute:

Fork the repo
Create a branch: git checkout -b feature/new-insight
Commit changes: git commit -m "Add new insight"
Push and open a Pull Request


License
This project is licensed under the MIT License – see LICENSE for details.

Acknowledgments

Data: E-commerce coffee shop transaction logs (2024–2025)
Tools: Power BI, Python (pandas), GitHub
Let’s brew better business decisions with data! ☕📊

---

