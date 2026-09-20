# Maven Toys Inventory & Demand Analysis 
 
An advanced **Microsoft Excel business intelligence project** analyzing retail inventory, product demand, stock-out exposure, and inventory coverage using the Maven Toys Mexico Toy Sales dataset. 
 
## 📊 Dashboard Preview 
 
![Maven Toys Inventory & Demand Analysis](images/dashboard.png) 
 
## 🎯 Project Objective 
 
The goal of this project is to transform retail sales and inventory data into practical insights for monitoring stock availability and demand. 
 
The analysis focuses on: 
 
- Inventory availability by store and product 
- Out-of-stock products 
- Low-inventory products 
- Fast- and slow-moving products 
- Average daily demand 
- Estimated Days of Inventory 
- Replenishment attention areas 
- Product-category demand 
- Store inventory exposure 
 
## 🏢 Business Problem 
 
A retailer needs to understand whether current inventory is sufficient relative to historical demand. 
 
Instead of looking at stock quantity alone, this project combines: 
 
**Current Inventory + Historical Demand + Days of Inventory** 
 
to identify products with tighter inventory coverage. 
 
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
 
## 🛠️ Tools & Techniques 
 
- Microsoft Excel 
- Power Query 
- Excel Data Model 
- PivotTables 
- PivotCharts 
- Excel formulas 
- Data cleaning and transformation 
- Inventory analysis 
- Demand analysis 
- Business KPI development 
- Dashboard design 
 
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
 
📌 Business Questions 
 
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
     
📐 Key Metrics 
Average Daily Demand 
Average Daily Demand = 
Total Units Sold ÷ Calendar Days 
 
The analysis uses 638 calendar days. 
 
Days of Inventory 
Days of Inventory = 
Current Inventory ÷ Average Daily Demand 
 
A lower Days of Inventory value indicates tighter inventory coverage relative to historical demand. 
 
📈 Dashboard KPIs 
KPI	Value 
Total Units Sold	1,090,565 
Current Inventory	29,742 
Average Daily Demand	1,709 units/day 
Average Days of Inventory	17.4 days 
Total Products	35 
Total Stores	50 
📊 Dashboard Visualizations 
 
The dashboard includes: 
 
Top 10 Fast-Moving Products 
Demand by Product Category 
Lowest 10 Stores by Inventory 
10 Products with Lowest Days of Inventory 
🔍 Key Findings 
Total historical units sold: 1,090,565 
Current inventory: 29,742 units 
Average historical demand: approximately 1,709 units per day 
Overall inventory coverage: approximately 17.4 days 
The analysis covers 35 products across 50 stores 
Several product-store combinations currently have zero inventory 
Colorbuds, PlayDoh Can, Barrel O' Slime, and Deck Of Cards have among the lowest estimated Days of Inventory 
Combining current inventory with historical demand provides more context than inventory quantity alone 
📦 Replenishment Analysis 
 
Product-store combinations were reviewed using current stock levels and historical demand indicators. 
 
The analysis uses: 
 
0 units → Current stock-out condition 
1–5 units → Very low current inventory 
Lower Days of Inventory → Tighter stock coverage relative to historical demand 
 
The dataset does not contain supplier lead times, purchase orders, reorder points, or safety-stock targets. Therefore, replenishment attention is based on the available inventory and historical demand indicators rather than a formal procurement optimization model. 
 
📁 Workbook Structure 
Inventory Demand Stock Risk Intelligence.xlsx 
 
├── README 
├── Raw_Sales 
├── Raw_Inventory 
├── Raw_Products 
├── Raw_Stores 
├── Calendar 
├── Analysis 
└── Dashboard 
Sheet Overview 
Sheet	Purpose 
README	Project documentation 
Raw_Sales	Prepared sales data 
Raw_Inventory	Current inventory data 
Raw_Products	Product master data 
Raw_Stores	Store master data 
Calendar	Date reference table 
Analysis	Business question analysis 
Dashboard	Final inventory and demand dashboard 
⚠️ Limitations 
 
The dataset does not include: 
 
Supplier information 
Purchase orders 
Supplier lead times 
Reorder points 
Safety stock levels 
Future demand forecasts 
Promotion calendars 
Planned replenishment quantities 
 
Therefore, the replenishment analysis is based on current inventory and historical demand indicators available in the dataset. 
 
🚀 Skills Demonstrated 
Excel 
Power Query 
PivotTables 
PivotCharts 
Excel Formulas 
Data Model 
Dashboard Development 
Data Analytics 
Data Cleaning 
Data Transformation 
Inventory Analysis 
Demand Analysis 
Stock-Out Analysis 
KPI Reporting 
Business Question Analysis 
Business Intelligence 
Data Modeling 
Data Visualization 
Analytical Storytelling 
Business Insight Generation 
👤 Author 
 
Ajmal Sr 
 
BSc Computer Science | Data Analytics & Business Intelligence 
 
GitHub: Ajmal-SR 
LinkedIn: Ajmal Sr b
