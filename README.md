# Business Performance Overview Dashboard

**A 3-page Power BI executive dashboard tracking sales, customer, and marketing performance for a mid-size B2B business — built with drill-through order-level detail and YoY/target tracking baked into every KPI.**

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

---

## 📌 Overview

This dashboard gives leadership a single view across three connected areas — overall business health, sales performance, and customer/marketing effectiveness — with the ability to drill from a summary KPI straight down to individual order line items. It's built to answer the two questions executives actually ask in a review meeting: *"Are we on track?"* and *"Why or why not?"*

## ❓ Problem

- Sales, customer, and campaign data lived across disconnected views, so answering "is a soft month a sales problem or a marketing problem" required manually cross-referencing multiple reports.
- Leadership needed **target and YoY context on every number**, not just raw totals — a strong-looking total can hide a miss against plan.
- No easy way to go from "which customer/order is driving this number" back to the source transaction.

## 📈 Report Pages

### 1. Business Performance Overview
Executive summary: Total Sales (£527K, +97.8% YoY), Total Orders, Total Customers, Avg Order Value, Gross Margin % (36.9%), and Sales-to-Target % (95.4%, flagged "At Risk"). Includes top 5 products, order fulfillment pipeline (Placed → Shipped → Delivered → Invoiced → Paid, with drop-off at each stage), sales by region, sales by category, and top 5 cities.

### 2. Sales Performance
Sales vs. Target by month, sales trend vs. last year, a full category/sub-category breakdown table with gross margin %, a margin-vs-sales bubble chart by product category, and sales by brand.

### 3. Customer & Marketing
Revenue by account manager over time, Top 10 customers by sales with credit limit and DSO (Days Sales Outstanding) status, customers by segment (Enterprise/Mid-Market/SMB), campaign spend by initiative, and spend by channel (Paid Search/Social/Email/Display).

### Drill-through: Customer Detail
Click any customer to drill into their individual order history — Order ID, date, line total, and credit limit.

## 💡 Key Findings

- **Sales-to-Target sits at 95.4% but is flagged "At Risk"** — despite strong 97.8% YoY growth, the gap to target is the more actionable number for a leadership review than the growth headline alone.
- **Order fulfillment has a real leak, not just a rounding gap** — Paid stage drops to 88.24% of Invoiced (only 77.3% of all Placed orders reach Paid), meaning collections — not sales or shipping — is the biggest bottleneck in the funnel.
- **Electronics leads on revenue (£131K) but not margin** — the margin-vs-sales bubble chart shows Electronics trades volume for thinner margin versus categories like Beauty, which is a more profitable mix than the headline sales-by-category chart alone suggests.
- **Revenue variance is negative (-£25K) even with the business ahead YoY** — a reminder that target-tracking and year-over-year comparisons can tell different stories in the same period.

## 🧰 Tech Stack

| Layer | Tool |
|---|---|
| Data Modeling | Power BI |
| Metrics | DAX (YoY, target variance, DSO, funnel conversion) |
| Visualization | Power BI (drill-through, cross-page slicers, ribbon charts) |

## 📂 Repo Structure

```
├── Report/
│   └── Business_Performance.pbix
├── Data/
│   └── (sample/synthetic sales dataset)
├── Screenshots/
│   ├── Overview.png
│   ├── SalesPerformance.png
│   └── CustomerMarketing.png
├── Sales_Marketing_Performance_Dashboard.pdf   # static export for viewers without Power BI Desktop
└── README.md
```

## 🚀 How to Reproduce

1. Download `Report/Business_Performance.pbix`
2. Open in Power BI Desktop (free) — data is embedded, no external connections required
3. Use the top nav (Overview / Sales Performance / Customer & Marketing) to move between pages; click a customer row on page 3 to drill through to order detail

## 🔗 Live Report

*(Recommended: publish to Power BI Service or Power BI Public and link here — a clickable live report is more convincing to reviewers than static screenshots.)*

---

*Dataset: sample/synthetic sales data — no real company or customer data used.*
