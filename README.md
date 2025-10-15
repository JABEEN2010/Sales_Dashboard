**📊 Sales Dashboard – Power BI Project**

**🧾 Overview**

This Power BI project presents a Sales Performance Dashboard that combines insights from Orders and Details datasets. It enables an interactive analysis of sales, profit, quantity, and customer trends across multiple dimensions such as city, category, and payment mode.

**🎯 Objectives**

To visualize total and monthly sales performance.

To identify top-performing categories, subcategories, and cities.

To analyze customer purchase behavior and profit trends.

To monitor payment mode distribution and sales contribution.

**🧩 Data Model**

The dashboard is built on a one-to-many relationship between the following tables:

Orders (1) ——< Details (∞)


Linked through the common field Order ID.

| 🧾 **Table** | 🔑 **Key Columns** | 📝 **Description** |
|--------------|--------------------|--------------------|
| **Orders**  | `Order ID`, `Order Date`, `CustomerName`, `State`, `City` | Contains **order-level** information |
| **Details** | `Order ID`, `Amount`, `Profit`, `Quantity`, `Category`, `Sub-Category`, `PaymentMode` | Contains **item-level transaction** details |


**📈 Key Insights**

Total Sales: $437.8K

Profit Margin: 8.4%

Average Profit per Order: $73.9

Total Quantity Sold: 5,615

Top 5 Cities by Sales: Pune, Thiruvananthapuram, Udaipur, Simla, Surat

Top Categories:

Electronics: $166K

Clothing: $144K

Furniture: $127K

Most Used Payment Mode: Cash on Delivery (35.4%)

**📊 Dashboard Features**

Slicers: City, Category, and Year-Month filters

Visuals:

Total Sales by Month

Profit Margin Trend

Top 5 Cities by Sales

Sales by Category & Sub-Category

Sales by Payment Mode

KPIs Displayed:

Total Sales

Profit Margin (%)

Average Profit per Order

Total Quantity

**⚙️ Tools & Techniques**

Tool: Power BI Desktop

Data Processing: Power Query for data cleaning and transformation

Modeling: Relationship between Orders and Details tables

DAX Measures:

Total Sales = SUM(Details[Amount])

Profit Margin = DIVIDE(SUM(Details[Profit]), SUM(Details[Amount]))

Avg Profit per Order = AVERAGE(Details[Profit])

Sales MoM Growth = (CurrentMonthSales - PreviousMonthSales) / PreviousMonthSales

**💡 Insights & Business Impact**

This dashboard empowers decision-makers to:

Identify high-performing cities and product categories.

Evaluate profitability and growth patterns.

Optimize payment strategies and customer engagement.

Plan targeted marketing campaigns based on sales performance.


