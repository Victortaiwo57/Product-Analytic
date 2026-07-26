# Product-Analytic
# Sales Pipeline Dashboard (Power BI)

A 3-page executive-to-operational sales analytics dashboard built in Power BI, covering revenue performance, sales team activity, and pipeline health for a B2B sales organization.

![Power BI](https://github.com/Victortaiwo57/Product-Analytic/blob/main/Screenshot%202026-07-26%20013935.png)
![DAX](https://img.shields.io/badge/DAX-2C2C2C?style=flat)
![Power Query](https://img.shields.io/badge/Power%20Query-217346?style=flat)

---

## 📊 Project Description

This project simulates a B2B sales pipeline for a multi-region company (Europe, North America, Asia-Pacific, Latin America) across seven industries. The goal was to design a report that three different audiences could use without modification:

- **Leadership** — a one-glance snapshot of revenue, pipeline value, and forecast health
- **Sales managers** — rep-level performance, funnel conversion, and team activity tracking
- **Revenue operations** — stalled deal detection, lost-reason analysis, and pipeline aging

Rather than building a single dense report, the dashboard is split into three purpose-built pages, each scoped to answer one core business question for one core audience, with consistent slicers and visual language tying them together.

---

## 🗂 Pages

### 1. Executive Overview
- KPI cards: Total Revenue, Pipeline Value, Win Rate, Average Deal Size, Weighted Pipeline (each with YoY trend + sparkline)
- Monthly Total Revenue vs. Revenue Trailing 12M (bar + line combo)
- Next-quarter forecast card
- Revenue by region (donut chart)

### 2. Sales Performance
- Salesperson leaderboard (revenue by rep)
- Conversion funnel (Lead In → Qualified → Proposal → Negotiation → Contracting, with overall conversion rate)
- Region × Industry revenue matrix with conditional formatting
- Activities logged by region and activity type (stacked bar)

### 3. Pipeline Health
- KPI cards: Stalled Deals (30d+), Stalled Deal Value, Avg Sales Cycle, Deal Count
- Deals stuck in stage (table: count, avg age, stalled value by stage)
- Lost reason pareto (ranked bar chart of lost value by reason)
- Pipeline aging distribution (0-30 / 31-60 / 61-90 / 90+ days)
- Linear trend forecast vs. pipeline-weighted forecast

---

## 🛠 Tech Stack / Skills Demonstrated

- **Data modeling** — star schema with fact/dimension tables and conformed dimensions across all three pages
- **DAX** — time-intelligence measures (YoY, trailing 12-month averages), weighted pipeline forecasting, stage-aging calculations
- **Power Query** — data cleaning, shaping, and categorization logic (e.g. lost-reason and stage-aging buckets) prior to load
- **UX/UI design** — consistent brand palette, card-based KPI layout, persistent filter panel for cross-page slicer consistency

---

## 📁 Repo Structure

```
sales-pipeline-dashboard/
├── Sales_Pipeline_Dashboard.pbix     # Power BI source file
├── /screenshots                      # Page-by-page exports (PNG/PDF)
├── /data                             # Sample/synthetic dataset used (if shareable)
└── README.md
```

---

## 🚀 How to View

1. Clone or download this repo
2. Open `Sales_Pipeline_Dashboard.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
3. Use the **Product**, **Activity**, and **Role** slicers to filter each page; the **All Deal / Won / Lost** toggle on the Executive Overview page filters that page's visuals

*(If you don't have Power BI Desktop, see the `/screenshots` folder for static page exports.)*

---

## 💡 Design Notes

This project leans on a more deliberate, product-minded approach: each page has a single audience and a single job, the visual language (color, typography, card layout) stays consistent throughout so the report reads as one product rather than three disconnected charts, and chart types are chosen for how well their shape communicates the insight (e.g. a Pareto for lost-reason drivers, a funnel for stage drop-off) rather than defaulting to tables everywhere.

---

## 📬 Contact

Open to freelance Power BI / data analytics projects — reach out via [Upwork profile link] or [email].
