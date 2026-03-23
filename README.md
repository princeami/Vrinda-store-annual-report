# 🛍️ Vrinda Store — Annual Sales Analysis 2022

![Dashboard Preview](dashboard_preview.png)

> **A complete end-to-end data analysis project** on 31,047 orders from Vrinda Store — an Indian fashion e-commerce brand. Includes data cleaning, exploratory analysis, visual dashboards, and business insights.

---

## 📊 Project Overview

| Field | Details |
|---|---|
| **Dataset** | Vrinda Store Sales Data 2022 |
| **Total Orders** | 31,047 |
| **Total Revenue** | ₹ 2,11,76,377 (Rs 2.12 Crore) |
| **Period** | January 2022 – December 2022 |
| **Tools Used** | Python, Pandas, Matplotlib, Power BI, ReportLab |
| **Output** | 2-page PDF Dashboard + Power BI Ready CSV |

---

## 🎯 Business Problem

Vrinda Store wanted to understand their 2022 annual sales performance to:
- Identify their best-performing months, channels, and states
- Understand their core customer demographics
- Find reasons behind Q4 revenue decline
- Make data-driven decisions for 2023 growth strategy

---

## 📁 Project Structure

```
vrinda-store-analysis/
│
├── data/
│   ├── Vrinda_Store_Data_Analysis.xlsx        # Raw dataset
│   └── Vrinda_Store_PowerBI_Data.csv          # Cleaned dataset for Power BI
│
├── dashboard/
│   └── Vrinda_Store_Dashboard.pdf             # Final 2-page PDF dashboard
│
├── notebooks/
│   └── vrinda_analysis.py                     # Python analysis script
│
├── powerbi/
│   └── Vrinda_PowerBI_Guide.pdf               # Step-by-step Power BI setup guide
│
└── README.md
```

---

## 📈 Key Findings & Insights

### 💰 Revenue & Orders
- **Total Revenue:** ₹2.12 Crore across 31,047 orders
- **Average Order Value:** ₹682
- **Peak Month:** March (₹19.3L) — best time for campaigns
- **Worst Month:** November (₹16.2L) — Q4 decline needs attention
- **Delivery Rate:** 92.3% — strong fulfilment performance

### 🛒 Sales Channels
| Channel | Revenue | Share |
|---|---|---|
| Amazon | ₹75.2L | 35.5% |
| Myntra | ₹49.4L | 23.3% |
| Flipkart | ₹45.7L | 21.6% |
| Ajio | ₹13.3L | 6.3% |
| Others | ₹28.1L | 13.3% |

> **Amazon dominates** — invest heavily in Amazon Ads and Prime listing optimization.

### 👗 Product Categories
| Category | Revenue Share |
|---|---|
| Set | 49.6% |
| Kurta | 23.4% |
| Western Dress | 14.9% |
| Top | 5.6% |
| Others | 6.5% |

> **Sets + Kurtas = 73% of all revenue** — these SKUs must never go out of stock.

### 👤 Customer Demographics
- **Women** contribute **64%** of total revenue vs Men at 36%
- **Age group 36–50** is the largest buyer segment (35.7% of customers)
- **Top sizes:** M, L, XL, S, XXL — stock these sizes as priority

### 🗺️ Geographic Performance
| State | Revenue |
|---|---|
| Maharashtra | ₹29.9L |
| Karnataka | ₹26.5L |
| Uttar Pradesh | ₹21.0L |
| Telangana | ₹17.1L |
| Tamil Nadu | ₹16.8L |

> **Maharashtra is #1** — prioritize warehouse and logistics investment here.

### ⚠️ Problem Areas
- **Return Rate:** 3.4% — improve product images and size guides
- **Cancellation Rate:** 2.7% — improve delivery ETAs and stock accuracy
- **Q4 Decline:** Revenue drops Oct–Dec — need festive season campaigns

---

## 🖥️ Dashboard Preview

### Page 1 — Sales Overview
- KPI Cards (Revenue, Orders, AOV, Delivery Rate)
- Monthly Revenue & Orders Trend (Line + Bar)
- Revenue by Gender (Pie Chart)
- Revenue by Sales Channel (Bar Chart)
- Category Mix (Donut Chart)
- Order Status Breakdown (Donut Chart)
- Top 8 States by Revenue (Bar Chart)
- Age Group Distribution (Bar Chart)
- Top Sizes Ordered (Bar Chart)
- 8 Key Insights & Recommendations Panel

### Page 2 — Deep Dive Analysis
- Gender × Channel Revenue Heatmap
- Monthly Orders by Channel (Stacked Bar)
- Revenue by Gender × Age Group (Grouped Bar)
- Average Order Value by State (Bar Chart)
- Top 10 SKUs by Revenue (Bar Chart)
- Monthly Revenue Trend by Channel (Line Chart)
- Executive Summary Metrics Table

---

## 🔧 How to Run

### Prerequisites
```bash
pip install pandas matplotlib openpyxl reportlab pypdf
```

### Run Analysis
```bash
# Clone the repo
git clone https://github.com/yourusername/vrinda-store-analysis.git
cd vrinda-store-analysis

# Run Python analysis and generate PDF dashboard
python notebooks/vrinda_analysis.py
```

### Open Power BI Dashboard
1. Open `data/Vrinda_Store_PowerBI_Data.csv` in Power BI Desktop
2. Follow the `powerbi/Vrinda_PowerBI_Guide.pdf` step by step
3. Build dynamic dashboard with 11 slicers

---

## 📊 Tools & Technologies

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0-lightblue?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.8-orange)
![PowerBI](https://img.shields.io/badge/Power_BI-Dashboard-yellow?logo=powerbi)
![ReportLab](https://img.shields.io/badge/ReportLab-PDF-red)

| Tool | Purpose |
|---|---|
| Python (Pandas) | Data cleaning, analysis, aggregation |
| Matplotlib | Chart generation |
| ReportLab | PDF dashboard creation |
| Power BI | Interactive dynamic dashboard |
| Excel / CSV | Raw data storage |

---

## 💡 Business Recommendations

1. **Launch pre-March campaigns** — Stock up inventory in Feb, run sales in March
2. **Double down on Amazon** — 35.5% revenue share, optimize listings and ads
3. **Target women aged 36–50** — highest revenue segment, offer loyalty rewards
4. **Never stock out Sets & Kurtas** — they drive 73% of all revenue
5. **Fix Q4 decline** — Run Diwali + Christmas offers in Oct–Dec
6. **Improve size guides** — Reduce 3.4% return rate with better product info
7. **Expand Maharashtra logistics** — Highest revenue state, faster delivery = more orders

---

## 📂 Dataset Info

| Column | Description |
|---|---|
| Order_ID | Unique order identifier |
| Customer_ID | Unique customer identifier |
| Date | Order date |
| Gender | Customer gender |
| Age / AgeGroup | Customer age and age bracket |
| Channel | Sales platform (Amazon, Myntra, etc.) |
| Category | Product category |
| SKU | Stock keeping unit code |
| Size | Product size |
| Qty | Quantity ordered |
| Revenue | Order value in INR |
| Order_Status | Delivered / Returned / Cancelled / Refunded |
| State | Shipping state |
| B2B | Business-to-business order flag |
