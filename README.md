# Maven Toys Inventory & Demand Analysis

An advanced **Microsoft Excel business intelligence project** analyzing retail inventory, product demand, stock-out exposure, and inventory coverage using the Maven Toys Mexico Toy Sales dataset.

## 📊 Dashboard Preview

![Maven Toys Inventory & Demand Analysis](https://github.com/Ajmal-SR/Maven-Toys-Inventory-Demand-Analysis/blob/d3d2c1778175d577ff23c87a63a69e54a62084a3/Maven%20Toys%20Inventory%20and%20Demand%20Analysis%20Dashboard.png)

## 🎯 Project Objective

The goal of this project is to transform retail sales and inventory data into practical business insights for monitoring stock availability and demand.

The analysis focuses on:

- Inventory availability by store and product
- Out-of-stock products
- Low-inventory products
- Fast-moving and slow-moving products
- Average daily demand
- Estimated Days of Inventory
- Replenishment attention areas
- Product-category demand
- Store inventory exposure
- Current inventory compared with historical demand

## 🏢 Business Problem

A retail business needs to understand whether its current inventory is sufficient relative to historical demand.

Looking only at stock quantity does not provide enough context. A product with relatively high inventory may still have tighter coverage if its demand is high.

Therefore, this project combines:

**Current Inventory + Historical Demand + Days of Inventory**

to identify products and stores that require closer inventory monitoring.

## 🗂️ Dataset

The project uses the **Maven Toys Mexico Toy Sales** dataset.

| Dataset | Rows | Columns |
|---|---:|---:|
| Sales | 829,262 | 5 |
| Inventory | 1,593 | 3 |
| Products | 35 | 5 |
| Stores | 50 | 5 |
| Calendar | 638 | 1 |

### Main Data

**Sales**

- `Sale_ID`
- `Date`
- `Store_ID`
- `Product_ID`
- `Units`

**Inventory**

- `Store_ID`
- `Product_ID`
- `Stock_On_Hand`

**Products**

- `Product_ID`
- `Product_Name`
- `Product_Category`
- `Product_Cost`
- `Product_Price`

**Stores**

- `Store_ID`
- `Store_Name`
- `Store_City`
- `Store_Location`
- `Store_Open_Date`

**Calendar**

- `Date`

## 🛠️ Tools & Techniques

- Microsoft Excel
- Power Query
- Excel Data Model
- PivotTables
- PivotCharts
- Excel Formulas
- Data Cleaning
- Data Transformation
- Data Modeling
- Inventory Analysis
- Demand Analysis
- Stock-Out Analysis
- KPI Reporting
- Dashboard Development

## 🔄 Analysis Workflow

Raw Data  
↓  
Power Query Cleaning  
↓  
Data Model & Relationships  
↓  
PivotTable Analysis  
↓  
Business Questions  
↓  
Inventory & Demand Metrics  
↓  
Dashboard

## 📌 Business Questions

The analysis addresses the following business questions:

1. How much inventory is currently available at each store?
2. Which products are currently out of stock?
3. Which products have low inventory levels?
4. Which products are fast-moving?
5. Which products are slow-moving?
6. What is the average daily demand for each product?
7. How many days will the current inventory last based on average demand?
8. Which product-store combinations should receive replenishment attention?
9. Which products have the highest stock-out exposure?
10. Which stores have the lowest current inventory?
11. Which product categories have the highest demand?
12. How does current inventory compare with historical sales demand?

## 📐 Key Metrics

### Average Daily Demand

**Average Daily Demand = Total Units Sold ÷ Calendar Days**

The analysis uses **638 calendar days**.

**Total Units Sold:** 1,090,565

**Average Daily Demand:** approximately **1,709 units/day**

### Days of Inventory

**Days of Inventory = Current Inventory ÷ Average Daily Demand**

A lower Days of Inventory value indicates tighter inventory coverage relative to historical demand.

**Current Inventory:** 29,742 units

**Average Days of Inventory:** approximately **17.4 days**

## 📈 Dashboard KPIs

| KPI | Value |
|---|---:|
| Total Units Sold | 1,090,565 |
| Current Inventory | 29,742 |
| Average Daily Demand | 1,709 units/day |
| Average Days of Inventory | 17.4 days |
| Total Products | 35 |
| Total Stores | 50 |

## 📥 Project File

The complete Excel workbook is available for download:

[Download Excel Workbook](https://github.com/Ajmal-SR/Maven-Toys-Inventory-Demand-Analysis/releases/download/v1.0/Maven.Toys.Inventory.and.Demand.Analysis.xlsx)

## 📊 Dashboard Visualizations

The dashboard includes:

- **Top 10 Fast-Moving Products**
- **Demand by Product Category**
- **Lowest 10 Stores by Inventory**
- **10 Products with Lowest Days of Inventory**

These visuals provide a concise view of product demand, category demand, store inventory levels, and inventory coverage.

## 🔍 Key Findings

- Total historical units sold: **1,090,565**
- Current inventory: **29,742 units**
- Average historical demand: approximately **1,709 units per day**
- Overall inventory coverage: approximately **17.4 days**
- The analysis covers **35 products across 50 stores**
- Several product-store combinations currently have **zero inventory**
- **Colorbuds, PlayDoh Can, Barrel O' Slime, and Deck Of Cards** have among the lowest estimated Days of Inventory
- Products with lower Days of Inventory have tighter stock coverage relative to historical demand
- Combining current inventory with historical demand provides more context than inventory quantity alone

## 📦 Replenishment Analysis

Product-store combinations were reviewed using current stock levels and historical demand indicators.

The analysis uses:

- **0 units** → Current stock-out condition
- **1–5 units** → Very low current inventory
- **Lower Days of Inventory** → Tighter stock coverage relative to historical demand

Products with zero inventory represent current stock-out conditions, while products with very low inventory or low Days of Inventory require closer monitoring.

The dataset does not contain supplier lead times, purchase orders, reorder points, or safety-stock targets. Therefore, replenishment attention is based on available inventory and historical demand indicators rather than a formal procurement optimization model.

## 🧮 Inventory Coverage Analysis

Days of Inventory is used to compare current inventory with historical average daily demand.

The products with the lowest estimated inventory coverage include:

| Product | Days of Inventory |
|---|---:|
| Colorbuds | 3.75 |
| PlayDoh Can | 3.80 |
| Barrel O' Slime | 4.27 |
| Deck Of Cards | 4.66 |
| Magic Sand | 6.46 |
| Splash Balls | 6.50 |
| Lego Bricks | 6.56 |
| Action Figure | 6.76 |
| Rubik's Cube | 8.58 |
| Animal Figures | 10.02 |

These values indicate comparatively tighter inventory coverage based on historical average demand.

## 🏪 Store Inventory Analysis

Store-level inventory was analyzed to identify locations with lower current stock levels.

The **Lowest 10 Stores by Inventory** dashboard visual highlights stores with the lowest total current inventory.

This analysis provides a simple way to identify stores that may require closer inventory monitoring.

Low inventory at a store does not automatically indicate higher operational risk because store-level demand can vary.

## 📦 Product Demand Analysis

Historical sales were analyzed to identify fast-moving and slow-moving products.

### Fast-Moving Products

Products with higher total historical units sold are classified as fast-moving within this analysis.

The dashboard highlights the **Top 10 Fast-Moving Products**.

### Slow-Moving Products

Products with lower historical units sold are classified as slow-moving within the analyzed period.

This distinction provides context when interpreting current inventory levels.

## 📊 Product Category Demand

Product-category demand was analyzed using total historical units sold.

The **Demand by Product Category** dashboard visual compares demand across product categories and helps identify categories with relatively higher historical sales volume.

## 🧹 Data Preparation

Power Query was used for data preparation and cleaning before analysis.

The workflow included:

- Loading source datasets
- Preparing and cleaning columns
- Checking data structure
- Preparing analysis-ready tables
- Combining relevant product and store information
- Preparing data for the Excel Data Model

The prepared datasets were then used for PivotTable-based business analysis.

## 🔗 Data Model

The project uses relationships between the main datasets.

**Products → Sales**

**Products → Inventory**

**Stores → Inventory**

Main relationships:

- `Products[Product_ID]` → `Sales[Product_ID]`
- `Products[Product_ID]` → `Inventory[Product_ID]`
- `Stores[Store_ID]` → `Inventory[Store_ID]`

This structure supports product-level, store-level, and inventory analysis.

## 📊 Analytical Approach

The project uses PivotTables and Excel calculations to answer the business questions.

The analysis includes:

- Inventory by store
- Out-of-stock product analysis
- Low-inventory product analysis
- Fast-moving products
- Slow-moving products
- Average daily demand
- Days of Inventory
- Product-store replenishment attention
- Product stock-out exposure
- Store inventory exposure
- Category demand
- Inventory compared with historical demand

For selected analyses, PivotTable results were copied as values into normal Excel tables to support clean sorting and dashboard chart preparation.

## 📁 Workbook Structure

Inventory Demand Stock Risk Intelligence.xlsx

├── README  
├── Raw_Sales  
├── Raw_Inventory  
├── Raw_Products  
├── Raw_Stores  
├── Calendar  
├── Analysis  
└── Dashboard

### Sheet Overview

| Sheet | Purpose |
|---|---|
| README | Project documentation |
| Raw_Sales | Prepared sales data |
| Raw_Inventory | Current inventory data |
| Raw_Products | Product master data |
| Raw_Stores | Store master data |
| Calendar | Date reference table |
| Analysis | Business question analysis |
| Dashboard | Final inventory and demand dashboard |

## ⚠️ Limitations

The dataset does not include:

- Supplier information
- Purchase orders
- Supplier lead times
- Reorder points
- Safety stock levels
- Future demand forecasts
- Promotion calendars
- Planned replenishment quantities

Therefore, the replenishment analysis is based on **current inventory and historical demand indicators** available in the dataset.

The Days of Inventory metric is an estimate based on historical average daily demand and assumes that demand patterns remain broadly similar.

This project should therefore be interpreted as an **inventory monitoring and demand analysis framework**, rather than a complete procurement planning system.

## 💼 Business Value

This project demonstrates how Excel can be used to transform a large retail dataset into practical business insights.

The analysis can help business teams:

- Monitor inventory availability
- Identify current stock-out conditions
- Track low-inventory products
- Understand historical product demand
- Identify fast-moving products
- Monitor inventory coverage
- Compare current inventory with historical demand
- Identify stores requiring closer inventory monitoring
- Support data-driven inventory discussions

## 🚀 Skills Demonstrated

### Excel

- Power Query
- PivotTables
- PivotCharts
- Excel Formulas
- Excel Data Model
- Dashboard Development

### Data Analytics

- Data Cleaning
- Data Transformation
- Inventory Analysis
- Demand Analysis
- Stock-Out Analysis
- Product Performance Analysis
- Store-Level Analysis
- KPI Reporting
- Business Question Analysis

### Business Intelligence

- Data Modeling
- Data Visualization
- Analytical Storytelling
- Business Insight Generation
- Dashboard Design

## 👤 Author

**Ajmal Sr**

BSc Computer Science | Data Analytics & Business Intelligence

- GitHub: [Ajmal-SR](https://github.com/Ajmal-SR)
- LinkedIn: [Ajmal Sr](https://linkedin.com/in/ajmal-sr-)

## 📌 Project Summary

**Maven Toys Inventory & Demand Analysis** is an advanced Excel business intelligence project that combines historical sales, current inventory, product, store, and calendar data to analyze inventory availability and demand.

The project demonstrates an end-to-end analytical workflow using **Power Query, Excel Data Model, PivotTables, PivotCharts, Excel formulas, and dashboard design**.

The final dashboard provides a concise view of inventory levels, demand patterns, inventory coverage, fast-moving products, product-category demand, and stores requiring closer inventory monitoring.
