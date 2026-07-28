# AdventureWorks Excel Analytics

> An end-to-end Excel Business Intelligence and Sales Analytics project focused on transforming raw AdventureWorks data into actionable business insights.

---

## 📊 Project Overview

This project analyzes AdventureWorks sales data using **Microsoft Excel** to understand revenue performance, profitability, product performance, category trends, geographic markets, reseller performance, salesperson effectiveness, and target achievement.

The project goes beyond simple sales reporting by combining:

- Revenue analysis
- Profitability analysis
- Product and category analysis
- Regional analysis
- Reseller analysis
- Salesperson performance
- Target achievement analysis
- Business recommendations

The goal is to answer an important business question:

> **How can the business increase profitable growth while improving sales performance and reducing revenue and margin risks?**

---

## 🎯 Business Problem

Management needs a clear understanding of what is driving business performance and where improvement opportunities exist.

The analysis addresses questions such as:

- How are sales changing over time?
- Is revenue generating sufficient profit?
- Which products drive sales?
- Which products drive profit?
- Which categories perform best?
- Which regions drive sales?
- Which regions are most profitable?
- Which resellers are most important?
- Which reseller segments generate the most profit?
- Who generates the most sales?
- Who generates the most profit?
- Who performs best relative to target?
- Where are the biggest profitability risks?
- Where are the strongest growth opportunities?

---

## 🗂️ Dataset

The project uses the **AdventureWorks sales dataset**.

The analysis covers information related to:

- Products
- Product Categories
- Product Subcategories
- Sales
- Resellers
- Salespersons
- Salesperson Regions
- Regions
- Targets

The dataset enables analysis across multiple business dimensions:

Products
    ↓
Categories & Subcategories

Sales
    ↓
Products
    ↓
Resellers
    ↓
Regions
    ↓
Salespersons
    ↓
Targets

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Microsoft Excel | Data analysis and dashboard development |
| Excel PivotTables | Business analysis and aggregation |
| Excel PivotCharts | Data visualization |
| Excel Formulas | KPI and business calculations |
| Power Query | Data preparation and transformation |
| GitHub | Project documentation and version control |

## 📁 Project Structure

```text
AdventureWorks-Excel-Analytics/
│
├── Dashboard/
│   └── Dashboard_Preview.png
│
├── Dataset/
│   └── AdventureWorks_Dataset/
│
├── Documentation/
│   ├── Business_Insights.md
│   ├── Project_Report.md
│   └── Insight.md
│
├── Excel/
│   └── AdventureWorks-Excel-Analytics.xlsx
│
├── Images/
│   ├── KPI Screenshots/
│   └── PivotTable Screenshots/
│
├── .gitignore
├── DAX.md
├── LICENSE
└── README.md
```

## 📈 Key Analysis

### 1. Overall Business Performance

The business generated approximately:

- **Total Sales:** $77.55M
- **Total Profit:** Approximately $1.10M

The analysis indicates that the business generates strong revenue but operates with relatively low overall profitability.

This highlights the importance of improving:

- Pricing
- Product costs
- Discounting
- Product mix
- Reseller margins

### 2. Sales Trend Analysis

Sales increased significantly over the analyzed period.

- **Best Year:** 2019 — approximately $32.50M
- **Worst Year:** 2017 — approximately $8.07M
- **Peak Sales Month:** August — approximately $9.46M
- **Lowest Sales Month:** June — approximately $3.13M

The sales trend indicates strong overall growth, although monthly performance fluctuates.

This may indicate potential seasonality or changes in customer demand.

### 3. Product Analysis

The **Mountain-200 Black, 38** product was the strongest individual product based on both sales and profit.

- **Sales:** $2.94M
- **Profit:** $272.77K
- **Profit Margin:** 9.26%

The Mountain-200 product family is a major revenue and profit engine.

#### Core Star Products

The strongest products combine:

**High Sales + High Profit**

These products should receive priority in:

- Inventory availability
- Reseller support
- Marketing investment
- Pricing monitoring

#### Margin Risk Products

Several high-sales products generate negative profit.

For example:

**Touring-1000 Yellow, 60**

- **Sales:** $1.09M
- **Profit:** -$192.33K
- **Profit Margin:** -17.65%

These products require investigation into pricing, costs, discounts, and product mix.

#### Product Revenue Concentration

- **Top 10 Product Sales:** $19.66M
- **Total Sales:** $77.55M
- **Top 10 Contribution:** 25.35%

The top 10 products contribute approximately **25.35% of total sales**, indicating moderate product revenue concentration.

### 4. Category Analysis

The **Bikes** category is the leading category by sales.

- **Bikes Sales:** $64.07M

However, Bikes generated approximately:

- **Profit:** -$435.68K

Meanwhile, **Components** generated:

- **Sales:** $11.23M
- **Profit:** $1.00M

This is one of the most important findings in the project:

> The category generating the most revenue is not necessarily the category generating the most profit.

The **Bikes** category represents a significant margin risk and should be reviewed for:

- Pricing
- Discounting
- Product mix
- Product costs
- Reseller pricing

### 5. Regional Analysis

The **Southwest** was the leading region by sales.

- **Sales:** $18.00M
- **Sales Contribution:** Approximately 23%

The **Canada** market was the leading country by sales.

- **Sales:** $13.88M

Regional performance also shows that sales leadership and profitability leadership are not always aligned.

Some markets generate strong sales but weak or negative profit, creating opportunities for regional pricing and cost optimization.

### 6. Reseller Analysis

#### Top Reseller

**Brakes and Gears**

- **Sales:** $882.27K
- **Profit:** $67.90K

Brakes and Gears is the strongest individual reseller by both sales and profit.

#### Business Type Performance

**Top Business Type by Sales:**

**Warehouse — $37.43M**

**Top Business Type by Profit:**

**Value Added Reseller — $582.86K**

This demonstrates that the largest sales channel is not necessarily the most profitable channel.

#### Reseller Concentration

- **Top 10 Reseller Sales:** $7.74M
- **Total Sales:** $77.55M
- **Top 10 Contribution:** 9.98%

The top 10 resellers contribute only **9.98% of total sales**, indicating relatively low reseller concentration.

This reduces dependency risk and suggests that the business has a diversified reseller network.

### 7. Salesperson Analysis

#### Top Salesperson by Sales

**Linda Mitchell**

- **Sales:** $10.16M

#### Top Salesperson by Profit

**Jae Pak**

- **Profit:** $264.95K

#### Highest Profit Margin

**Pamela Ansman-Wolfe**

- **Profit Margin:** 4.23%

The analysis shows that the highest-sales salesperson is not necessarily the highest-profit salesperson.

Salesperson performance should therefore be evaluated using:

- Sales
- Profit
- Profit Margin
- Quantity
- Target Achievement

## 8. Target Performance Analysis

Target analysis provides a different perspective from actual sales performance.

The analysis compares:

**Actual Sales**  
+  
**Assigned Target**  
↓  
**Target Variance**  
↓  
**Target Achievement %**

### Key Finding

**Jillian Carson** recorded the highest target achievement among the provided salesperson target data:

- **Achievement:** 71.34%

**Stephen Jiang** recorded:

- **Achievement:** 0.97%
- **Largest Negative Variance:** Approximately -$109.08M

This demonstrates an important business principle:

> A salesperson with high sales may still perform below target if their assigned target is significantly higher.

Therefore, actual sales performance and target achievement should be analyzed together.

---

## 🔎 Key Insights

### 1. Strong Sales Does Not Always Mean Strong Profit

The business generates approximately **$77.55M in sales**, but profitability is relatively low.

High revenue areas should be reviewed for margin pressure.

### 2. Mountain-200 Is a Core Business Driver

The Mountain-200 product family generates strong sales and substantial absolute profit.

These products should be protected through strong inventory management and reseller support.

### 3. Bikes Is the Biggest Revenue Risk

Bikes generates approximately **$64.07M in sales** but records negative profit.

This is a major profitability issue requiring deeper pricing and cost analysis.

### 4. The Reseller Network Is Well Diversified

The top 10 resellers contribute only **9.98% of total sales**.

This indicates relatively low dependency on major reseller partners.

### 5. Sales and Target Achievement Tell Different Stories

The highest-sales salesperson is not necessarily the strongest performer relative to their assigned target.

Performance evaluation should combine:

**Actual Sales + Profitability + Target Achievement**

## 💡 Business Recommendations

### 1. Improve Profitability

Review high-sales, low-profit products and categories.

Focus on:

- Pricing
- Discounts
- Product costs
- Product mix
- Reseller margins

### 2. Protect Core Products

Maintain inventory availability and reseller support for high-performing Mountain-200 products.

Avoid stock-outs and continue strategic investment in proven revenue and profit drivers.

### 3. Develop High-Margin Growth Opportunities

Increase marketing and reseller focus on products with strong profit margins but relatively low sales.

Examples include:

- Hitch Rack - 4-Bike
- Classic Vest
- Sport-100 Helmet
- Hydration Pack

### 4. Improve Category Profitability

Investigate the negative profitability of the Bikes category while maintaining its strong sales contribution.

Use Components and other profitable categories as benchmarks for improving margin performance.

### 5. Strengthen Strategic Resellers

Maintain strong partnerships with high-sales, high-profit resellers such as Brakes and Gears.

At the same time, investigate high-sales, low-profit reseller relationships.

### 6. Improve Salesperson Performance

Recognize high-performing salespeople and share successful sales practices across the team.

Evaluate salespeople using both:

- Actual performance
- Target achievement

### 7. Improve Target Setting

Use historical sales performance and market potential to establish targets that are:

- Challenging
- Realistic
- Territory-aware
- Data-driven

---

## 📊 Dashboard Preview

The Excel dashboard provides an interactive overview of business performance across multiple dimensions.

### Dashboard Includes

- Total Sales KPI
- Total Profit KPI
- Profit Margin KPI
- Sales Trend
- Product Performance
- Category Performance
- Regional Performance
- Reseller Performance
- Salesperson Performance
- Target Achievement

### Dashboard Preview

![AdventureWorks Excel Dashboard](Images/Dashboard_Preview.png)

## 🎯 Final Business Takeaway

The AdventureWorks analysis demonstrates that the business has strong revenue-generating capabilities but significant opportunities to improve profitability.

The most important strategic priority is to move from revenue-focused growth toward profitable growth.

The business should:

- Protect high-performing core products
- Improve margins in high-sales/low-profit areas
- Expand high-margin growth opportunities
- Maintain a diversified reseller network
- Evaluate sales performance against both actual results and assigned targets

This analysis provides a data-driven foundation for better decisions across sales, products, categories, regions, resellers, salespeople, and target planning.

---

## ⭐ Project Highlights

- End-to-end Excel Business Intelligence project
- Multi-dimensional sales and profitability analysis
- PivotTable-driven business analysis
- Product and category profitability analysis
- Geographic performance analysis
- Reseller concentration analysis
- Salesperson profitability analysis
- Target achievement analysis
- Business recommendations based on data
- GitHub-ready documentation

---

## 👤 Author

**Sara Yeana**

This project was created as part of a practical Data Analytics and Business Intelligence portfolio to demonstrate skills in:

- Microsoft Excel
- Data Analysis
- Business Intelligence
- Sales Analytics
- Profitability Analysis
- PivotTables
- Dashboard Development
- Business Problem Solving
- Data-Driven Recommendations
