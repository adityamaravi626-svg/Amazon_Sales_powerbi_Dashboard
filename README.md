# Amazon Sales Dashboard using Power BI

## Project Overview

The Amazon Sales Dashboard is a business intelligence project developed using Microsoft Power BI to analyze sales performance, profitability, product categories, customer orders, payment methods, fulfilment status, and geographic distribution.

The primary objective is to transform raw Amazon sales data into an interactive and easy-to-understand dashboard that helps non-technical managers monitor business performance and make informed decisions.

## Objectives

- Analyze overall sales and profit performance.
- Monitor total orders, units sold, average order value, and profit margin.
- Identify top-performing product categories and products.
- Analyze delivered, shipped, returned, and cancelled orders.
- Evaluate sales and profit across payment methods and fulfilment methods.
- Compare sales, profit, and order volumes across states.
- Present business insights through interactive visualizations.

## Tools and Technologies

- Microsoft Power BI
- Power Query for data cleaning and transformation
- DAX (Data Analysis Expressions) for measures and calculations
- Microsoft Excel for the source dataset

## Dashboard Pages

### Page 1: Overall Sales and Profit Performance
- Total Sales
- Total Profit
- Total Orders
- Total Units Sold
- Average Order Value
- Profit Margin Percentage
- Monthly Sales and Profit Trend

### Page 2: Product Performance
- Category-wise Sales
- Category-wise Profit
- Category-wise Units Sold
- Top 10 Products by Sales

### Page 3: Order Status and Returns
- Delivered Orders
- Shipped Orders
- Returned Orders
- Cancelled Orders
- Return Rate
- Cancellation Rate
- Category-wise Returns and Cancellations

### Page 4: Payment, Fulfilment and Geographic Performance
- Sales by Payment Method
- Profit by Payment Method
- Sales by Fulfilment Method
- Profit by Fulfilment Method
- State-wise Sales
- State-wise Profit
- State-wise Orders

## Key DAX Measures

The project uses DAX measures to calculate business KPIs dynamically.

**Total Sales**
```dax
Total Sales =
SUM(Sheet1[Total_Sales_INR])
```

**Total Profit**
```dax
Total Profit =
SUM(Sheet1[Profit_INR])
```

**Total Orders**
```dax
Total Orders =
DISTINCTCOUNT(Sheet1[Order_ID])
```

**Total Units Sold**
```dax
Total Units Sold =
SUM(Sheet1[Quantity])
```

**Average Order Value**
```dax
Average Order Value =
DIVIDE([Total Sales], [Total Orders], 0)
```

**Profit Margin**
```dax
Profit Margin % =
DIVIDE([Total Profit], [Total Sales], 0)
```

The measures are designed to respond to report filters and slicers.

## Interactive Features

- Date-based filtering
- State and category filtering
- Dynamic KPI cards
- Monthly sales and profit trend analysis
- Product ranking by sales
- Comparative analysis across payment and fulfilment methods

## Dataset

The project uses an Amazon sales dataset in Excel format. The dataset contains fields related to order IDs, order dates, product categories, products, quantities, unit prices, discounts, sales amounts, profit, payment methods, fulfilment methods, order statuses, and shipping states.

## Business Value

This dashboard helps managers identify sales trends, understand profitability, recognize high-performing products, monitor order outcomes, compare payment and fulfilment methods, and evaluate geographic performance.

## Author Aditya Maravi

