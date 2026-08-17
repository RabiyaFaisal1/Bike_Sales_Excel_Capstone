🚲 Bike Sales Dashboard (Excel)

An interactive Excel dashboard analyzing customer demographics and purchasing behavior for a bike sales dataset of 1,000+ customer records. Built as a capstone project while following Alex The Analyst's Data Analyst Bootcamp.

## 📊 Overview

This project explores what drives bike purchases across income, gender, age, commute distance, and region — using PivotTables, PivotCharts, and interactive slicers to let users filter and explore the data live.

**Dashboard KPIs**
- Total Customers: 1,000
- Bike Purchase Rate: 48%
- Average Income (Buyers): $57,962.58
- Average Income (Non-Buyers): $54,874.76

**Dashboard Visualizations**
- Average Income Per Purchase — income by gender and purchase status
- Customer Commute Distance — purchases across commute-distance groups
- Customer Age Brackets — purchases across age groups
- Purchases by Region — purchases across Europe, North America, and Pacific

**Interactive Filters**
Slicers for Marital Status, Region, Education, and Cars — connected across all PivotTables so filtering any one updates every chart and KPI at once.

## 🧹 Data Cleaning

Raw data contained coded values, inconsistent formatting, and messy ranges that needed cleaning before analysis. All cleaning was done on a separate `working sheet` so the original `bike_buyers` sheet stayed untouched as a raw reference copy.

- **Duplicates**: Detected and removed 26 duplicate records
- **Categorical codes**: Standardized Marital Status (`M`/`S` → `Married`/`Single`) and Gender (`M`/`F` → `Male`/`Female`) using Find & Replace
- **Income formatting**: Prepared Income as numeric for accurate calculations
- **Age brackets**: Grouped raw ages into `Adolescent`, `Middle Age`, and `Old` using nested `IF` statements
- **Commute labels**: Relabeled `10+ Miles` to `More than 10 Miles` for consistent, readable chart axis labels

## 📈 Analysis

Four PivotTables were built to examine different aspects of purchasing behavior, each paired with a PivotChart:

1. **Income vs. Purchase** — average income by Gender and Purchased Bike status
2. **Commute Distance** — purchase counts by commute-distance bucket
3. **Age Brackets** — purchase counts by age group
4. **Region** — purchase counts by Region

## 🛠️ Tools & Skills

| Tool | Microsoft Excel |
|---|---|
| **Skills** | Data cleaning, duplicate removal, Find & Replace, nested IF logic, PivotTables, PivotCharts, interactive slicers, KPI creation, `GETPIVOTDATA`, dashboard design |

## 🔄 Workflow

```
Raw Data → Data Cleaning → Duplicate Removal → Categorical Standardization
→ Age Bracket Creation → PivotTables → PivotCharts → Interactive Slicers
→ Bike Sales Dashboard
```

## 💡 Key Takeaways

- **Cleaning took longer than building** — clean, consistent inputs are the real foundation of a trustworthy dashboard, not the charts themselves.
- **Slicers only control PivotTables that share the same pivot cache.** Building PivotTables independently (rather than copying from one shared source) can silently break cross-filtering — worth setting up correctly from the start on future projects.

## 👩‍💻 Project Type

Data Analytics | Microsoft Excel | Dashboard Project — built as part of an ongoing data analytics learning journey.
