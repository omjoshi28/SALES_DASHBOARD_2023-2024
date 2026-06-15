# 📊 Sales Dashboard 2023–2024
### An Interactive Power BI Dashboard for Indian Retail Sales Analysis

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

![Dashboard Preview](./Screenshot_2026-05-14_125514.png)

---

## 📌 Table of Contents

- [About the Project](#-about-the-project)
- [Why I Built This](#-why-i-built-this)
- [Dataset Overview](#-dataset-overview)
- [Dashboard Features](#-dashboard-features)
- [Key Insights & Findings](#-key-insights--findings)
- [Q&A — Business Questions Answered](#-qa--business-questions-answered)
- [Getting Started](#-getting-started)
- [Project Structure](#-project-structure)
- [Lessons Learned](#-lessons-learned)
- [Future Improvements](#-future-improvements)
- [Connect With Me](#-connect-with-me)

---

## 🧠 About the Project

This is an end-to-end **sales analytics dashboard** built in **Power BI**, using a custom retail dataset spanning **January 2023 to November 2024**. It tracks 205 orders across 5 product categories, 4 Indian regions, 8 states, and 16 cities — giving a holistic view of how sales, profit, and quantity shift over time, across geographies, and within product lines.

| Metric | Value |
|---|---|
| 💰 Total Sales | ₹54.54 Lakh (5.45M) |
| 📈 Total Profit | ₹24.24 Lakh (2.42M) |
| 📦 Total Quantity | 2,017 units |
| 🛒 Total Orders | 205 |
| 👥 Unique Customers | 49 |
| 🏷️ Products | 25 unique SKUs |
| 🗺️ Coverage | 8 states · 16 cities |
| 📅 Period | Jan 2023 – Nov 2024 |

---

## 💡 Why I Built This

I wanted to go beyond just learning Power BI features and actually apply them to answer **real business questions**. Retail sales data is something everyone can relate to — and analyzing it end-to-end (from raw Excel data to an interactive dashboard) is exactly the kind of workflow I'd do on the job.

The specific goals I had in mind:

- **Practice data modelling** — cleaning and structuring a raw Excel dataset for BI use
- **Build interactive visuals** — slicers, maps, trend charts, and KPI cards that respond to filters
- **Tell a story with data** — not just display numbers, but surface insights someone can act on
- **Understand regional and seasonal patterns** — which months, regions, and categories drive the most value
- **Document the process end-to-end** — like a real project, with a README that explains the thinking

---

## 📂 Dataset Overview

**File:** `SALES_DATASET.xlsx`

The dataset was structured as a single flat table with 205 rows and 20 columns:

| Column | Description |
|---|---|
| `Order ID` | Unique order identifier (ORD00001 – ORD00205) |
| `Customer ID / Name` | Customer reference |
| `Order Date / Ship Date` | Transaction and shipping dates |
| `Status` | Shipped · Delivered · Processing · Returned · Cancelled |
| `Product Name` | 25 distinct products |
| `Category` | Furniture, Electronics, Sports, Clothing, Office Supplies |
| `Quantity` | Units ordered |
| `Unit Price` | Price per unit (₹) |
| `Sales Amount` | Total revenue for the order |
| `Cost` | Cost of goods |
| `Profit` | Sales Amount − Cost |
| `Region` | East, West, North, South |
| `Country / State / City` | Indian geography |
| `Month Number / Month Name / Year` | Date dimensions |

**Order Status Breakdown:**

| Status | Count |
|---|---|
| Shipped | 58 (28.3%) |
| Returned | 47 (22.9%) |
| Delivered | 41 (20.0%) |
| Processing | 30 (14.6%) |
| Cancelled | 29 (14.1%) |

> ⚠️ ~37% of orders are either Returned or Cancelled — a key area flagged for investigation.

---

## 🎛️ Dashboard Features

| Visual | Purpose |
|---|---|
| **KPI Cards** | Instant view of Total Sales, Total Profit, Total Quantity |
| **Year Slicer (2023 / 2024)** | Toggle between years to compare performance |
| **Order ID Slicer** | Filter down to a single order for drill-through |
| **Total Sales by Category** | Horizontal bar chart ranking categories by revenue |
| **Sales Distribution by Region** | Donut chart showing each region's % share |
| **Monthly Sales Trend** | Area chart tracking volume across 12 months |
| **Quantity Distribution by Category** | Bar chart showing units sold per category |
| **Regional Sales Map** | Bing Maps bubble chart showing city-level sales density |

---

## 📊 Key Insights & Findings

### 1. 🏆 Category Performance

| Category | Sales (₹) | Profit (₹) | Units | Profit Margin |
|---|---|---|---|---|
| Furniture | 14,33,774 | 6,58,456 | 487 | **45.9%** |
| Electronics | 12,35,143 | 5,46,029 | 490 | 44.2% |
| Sports | 9,84,102 | 4,24,981 | 319 | 43.2% |
| Clothing | 9,83,442 | 4,35,252 | 385 | 44.3% |
| Office Supplies | 8,17,253 | 3,59,480 | 336 | 44.0% |

**Furniture is the top revenue and profit margin category**, even with fewer units than Electronics.

---

### 2. 🌍 Regional Breakdown

| Region | Sales (₹) | Profit (₹) | Share |
|---|---|---|---|
| East | 14,86,980 | 6,71,533 | 27.3% |
| South | 14,83,260 | 6,50,438 | 27.2% |
| West | 13,08,411 | 5,90,666 | 24.0% |
| North | 11,75,063 | 5,11,561 | 21.5% |

East and South together account for **54.5% of total sales**. The North region underperforms and warrants attention.

---

### 3. 📅 Year-on-Year Comparison

| Year | Sales (₹) | Profit (₹) | Units |
|---|---|---|---|
| 2023 | 30,60,989 | 13,29,791 | 1,086 |
| 2024 | 23,92,724 | 10,94,406 | 931 |

**2023 outperformed 2024** — partly because the 2024 data covers up to November (not a full year), but the monthly averages also show a declining trend worth monitoring.

---

### 4. 📆 Monthly Sales Trend

| Month | Sales (₹) |
|---|---|
| 🥇 September | 6,83,444 |
| 🥈 May | 6,14,037 |
| 🥉 February | 5,24,655 |
| ... | ... |
| December | 3,24,909 |
| June | 3,38,315 |
| March | 3,45,243 |

**September and May are the peak months** — likely aligned with festive shopping and summer buying patterns. December and June are relatively slow.

---

### 5. 🛍️ Top Products by Revenue

| Rank | Product | Sales (₹) |
|---|---|---|
| 1 | Yoga Mat | 4,24,743 |
| 2 | Sofa | 3,60,044 |
| 3 | Bookshelf | 3,48,343 |
| 4 | Wardrobe | 3,02,284 |
| 5 | Tablet | 2,77,493 |

Yoga Mat being the #1 product is a surprising finding — Sports has lower overall category revenue but one product punches well above its weight.

---

### 6. 🏙️ Top Cities by Sales

| Rank | City | Sales (₹) |
|---|---|---|
| 1 | Bengaluru | 5,23,934 |
| 2 | Cuttack | 4,89,378 |
| 3 | Surat | 4,82,480 |
| 4 | Kolkata | 4,44,112 |
| 5 | Mysuru | 3,59,523 |

Bengaluru leads, but Cuttack and Surat are very close behind — showing strong Tier-2 city performance.

---

### 7. 💹 Overall Profitability

- **Average Profit Margin: 45.0%** — strong and consistent across all categories (range: 43.2% – 45.9%)
- **Average Order Value: ₹26,603**
- **Highest Single Order: ₹57,272**
- **Lowest Single Order: ₹1,171**

---

## ❓ Q&A — Business Questions Answered

**Q: Which category should the business prioritize for growth?**
> Furniture — it has the highest revenue (₹14.3L), best profit margin (45.9%), and strong unit volume. Electronics is close in units but lower in margin.

**Q: Which region needs the most attention?**
> The North region contributes only 21.5% of total sales and the lowest profit (₹5.1L). Targeted campaigns or distribution improvements in Delhi/Punjab could close the gap with East and South.

**Q: Is the business growing year over year?**
> 2023 generated ₹30.6L vs ₹23.9L in 2024 — however, 2024 data is not yet complete (goes to ~November), so a like-for-like comparison isn't fully fair. Based on comparable months, the trend is flat to slightly declining.

**Q: When should the business run promotions?**
> Double down in **August/September** (pre-peak) and plan recovery campaigns in **December and June** which are the two lowest-revenue months.

**Q: Why is the return/cancellation rate so high (37%)?**
> 47 Returned + 29 Cancelled = 76 out of 205 orders. This is a significant operational red flag. A follow-up analysis on which products, categories, or regions drive returns would be the next step.

**Q: What's the most surprising finding?**
> Yoga Mat outperforming every Electronics and Furniture product individually, generating ₹4.24L in sales alone — more than any other single SKU. Sports as a category underperforms, but this one product is a hidden gem.

---

## 🚀 Getting Started

### Prerequisites

- **Power BI Desktop** (free) — [Download here](https://powerbi.microsoft.com/en-us/desktop/)
- Microsoft Excel (to view the raw dataset - https://github.com/omjoshi28/SALES_DASHBOARD_2023-2024/blob/main/SALES_DATASET.xlsx)

### Steps

1. **Clone this repository**
   ```bash
   git clone https://github.com/omjoshi28/SALES_DASHBOARD_2023-2024
   cd SALES_DASHBOARD_2023-2024
   ```

2. **Open the dashboard**
   ```
   Double-click: SALES_DASHBOARD_2023-2024.pbix
   ```

3. **Refresh data** (if prompted)
   - Go to **Home → Transform Data → Data Source Settings**
   - Point the source to `SALES_DATASET.xlsx` in the repo folder
   - Click **Refresh**

4. **Explore**
   - Use the **Year slicer** to toggle 2023/2024
   - Use the **Order ID slicer** for order-level drill-through
   - Click any region or category to cross-filter all other visuals

---

## 📁 Project Structure

```
sales-dashboard-2023-2024/
│
├── 📊 SALES_DASHBOARD_2023-2024.pbix   # Power BI dashboard file
├── 📋 SALES_DATASET.xlsx               # Raw source data (205 orders, 20 columns)
├── 🖼️  SALES_DASHBOARD.png # Dashboard preview image
└── 📄 README.md                        # This file
```

---

## 📚 Lessons Learned

- **Data quality matters first** — Spending time structuring the Excel file properly (clean column names, consistent date formats, no merged cells) saved a lot of time in Power BI
- **DAX measures vs. calculated columns** — Learned when to use each; measures are better for aggregations that change with filters
- **Map visuals need clean location data** — City + State + Country together gave much better Bing Maps matching than city alone
- **A 45% return/cancel rate is a story** — What looks like a "clean" dataset can hide operational problems that only surface when you look at Status breakdowns
- **Design for the reader, not yourself** — The dark theme with high-contrast labels makes the dashboard scannable in under 30 seconds

---

## 🔮 Future Improvements

- [ ] Add a **Returns Analysis page** — which products/regions/customers cancel or return most
- [ ] Build a **Customer Segmentation view** — RFM (Recency, Frequency, Monetary) analysis across 49 customers
- [ ] Add **forecast visuals** — Power BI's built-in analytics to project 2025 sales
- [ ] Create a **mobile layout** — optimise for Power BI mobile app
- [ ] Connect to a **live database** instead of static Excel for real-time refresh
- [ ] Add **tooltips** — hover cards on the map showing city-level KPIs

---

## 🤝 Connect With Me

Built by **Om Joshi**
- 🔗 LinkedIn: [https://linkedin.com/in/om-joshi028/]
- 💻 GitHub: [https://github.com/omjoshi28/SALES_DASHBOARD_2023-2024]
- 📧 Email: omjoshi2807@gmail.com

> ⭐ If this project helped you or you liked the approach, give it a star — it means a lot!

---

