# Sales Performance Analysis

## 1. Project Overview

The Sales Performance Analysis project aims to evaluate sales revenue, product profitability, monthly sales trends, and discount effectiveness. The objective is to identify high- and low-performing products, understand fluctuations in monthly sales, and determine whether discounts are reducing profitability.

The analysis supports management in making data-driven decisions related to pricing strategies, discount policies, sales planning, and profitability improvement.

## 2. Problem Statement

The organization needs a data-driven Sales Performance Analysis to understand revenue and profitability trends, identify high- and low-performing products, customers, regions, and salespeople, evaluate the impact of discounts, and identify data-quality issues affecting sales reporting.

Management wants to improve product sales profitability by understanding which products generate high revenue but relatively low profit, identifying monthly sales fluctuations and periods of unusually high or declining performance, and evaluating whether the discounts offered to increase sales are negatively affecting profitability.

The objective is to analyze product profitability, monthly sales trends, and discount effectiveness using reliable sales data and provide actionable insights for pricing, discount, and sales planning decisions.

## 3. Project Objectives

* Analyze overall sales revenue and profitability.
* Identify high-revenue and low-profit-margin products.
* Analyze monthly sales trends and fluctuations.
* Evaluate the relationship between discount levels and profit margins.
* Compare sales performance across customers, regions, and salespeople.
* Identify and resolve data-quality issues.
* Develop actionable business recommendations for management.

## 🛠️ Tools and Technologies

* **Microsoft Excel:** Data inspection, cleaning, and validation.
* **Power Query:** Data transformation and preparation.
* **Power BI:** Data modeling, DAX calculations, reports, and dashboards.
* **DAX:** KPI calculations and business measures.
* **Excel** - Source data 


### 🏗️ Data Model - Star Schema
**Fact Table:** Fact Sales (Order_ID,Order_Date,Customer_ID,Product_ID,Region_ID,City_ID,Salesperson_ID,Sales_Channel_ID,Payment_Method,Quantity,Discount_Pct,
Order_Status).

**Dimension tables (8):** Dim_Category, Dim_Product, Dim_Customer, Dim_Region, Dim_City, Dim_SalesChannel, Dim_SalesPerson, Dim_Manufacturer.

**Relationship:** 1-to-Many.

## 5. Key Business Questions

1. Which products generate the highest net sales?
2. Which products generate high revenue but relatively low profit margins?
3. Which month has the highest and lowest sales?
4. How does profitability change across months?
5. Do higher discounts correspond to lower profit margins?
6. Which discount band generates the highest profit?
7. Which customers contribute the most revenue and profit?
8. Which salespeople generate the highest profit?
9. Which regions or sales channels perform best?
10. What data-quality issues could affect reporting accuracy?

## 6. Key Insights and Analysis

### Insight 1: Product Profitability

**Observation:** Some products may generate high revenue but relatively low profit margins. Revenue alone is therefore insufficient to evaluate product performance.

**Analysis:**

* Compare net sales, total profit, and profit margin by product.
* Identify products with high revenue and low profit margins.
* Compare product-level costs and discount percentages.
* Investigate whether low margins are associated with higher costs or aggressive discounts.

**Recommendations:**

* Review the pricing strategy for high-revenue, low-margin products.
* Negotiate better purchase prices with suppliers where possible.
* Prioritize products that generate both strong sales and healthy profit margins.
* Review low-margin products before changing their prices or promotional support.

**Expected impact:** Improved product profitability and more effective allocation of marketing resources.

### Insight 2: Monthly Sales Trends

**Observation:** Monthly sales fluctuate, with October identified as the highest-sales month and July as the lowest-sales month in the analyzed dataset.

**Analysis:**

* Compare monthly net sales and profit.
* Identify months with significant increases or decreases.
* Compare sales growth with changes in order volume and discount levels.
* Investigate possible reasons for unusually strong or weak performance.

**Recommendations:**

* Investigate the factors contributing to October's strong performance.
* Review demand, inventory availability, and promotional activity during July.
* Use historical trends to plan inventory and monthly sales targets.
* Schedule campaigns based on validated seasonal patterns.
* Compare performance across years when sufficient historical data is available.

**Expected impact:** Better sales forecasting, inventory planning, and resource allocation.

### Insight 3: Discount Effectiveness

**Observation:** Higher discount bands appear to be associated with lower profit margins in the analyzed data. This relationship should be validated before concluding that discounts directly cause lower profitability.

**Analysis:**

* Group transactions into discount bands.
* Compare net sales, profit, and profit margin across bands.
* Evaluate whether higher discounts produce sufficient additional sales volume.
* Compare discount effectiveness across products and customer segments.

**Recommendations:**

* Establish discount limits based on product profitability.
* Require approval for discounts above predefined thresholds.
* Use targeted discounts rather than applying the same discount to every product.
* Measure the incremental profit generated by promotional campaigns.
* Avoid promotions that increase revenue but reduce overall profit without a compensating business benefit.

**Expected impact:** Better discount control and improved profit margins.

### Insight 4: High- and Low-Performing Products

**Observation:** Products differ in their contributions to total sales and profit.

**Recommendations:**

* Promote products that consistently generate strong sales and healthy margins.
* Investigate low-selling products to understand demand, pricing, and availability issues.
* Review products with both low sales and low profitability.
* Consider profitable product bundles where appropriate.
* Monitor changes in product performance over time.

**Expected impact:** A stronger product portfolio and improved sales effectiveness.


### Insight 5: Data Quality

**Observation:** Missing values, duplicate records, inconsistent categories, and incorrect calculations can affect sales reporting.

**Recommendations:**

* Investigate duplicate transactions before removing them.
* Resolve missing customer, product, and salesperson details where possible.
* Standardize product names, regions, and sales-channel values.
* Validate quantity, price, cost, discount, net sales, and profit calculations.
* Monitor data-quality errors through a dedicated report.

**Expected impact:** More reliable reporting and better management decisions.

## 6. Recommended Power BI Visuals

| Analysis                         | Recommended Visual     |
| -------------------------------- | ---------------------- |
| Total Net Sales                  | KPI Card               |
| Total Profit                     | KPI Card               |
| Profit Margin (%)                | KPI Card               |
| Monthly Sales Trend              | Line Chart             |
| Monthly Profit Trend             | Line Chart             |
| Product Revenue vs Profit Margin | Scatter Chart          |
| Top Products by Net Sales        | Bar Chart              |
| Profit by Product                | Bar Chart              |
| Profit Margin by Discount Band   | Clustered Column Chart |
| Sales by Region                  | Bar Chart or Map       |
| Sales by Salesperson             | Bar Chart              |
| Customer Profit Contribution     | Bar Chart              |
| Data-Quality Issues              | Table or KPI Cards     |

## 7. Suggested KPIs

* **Net Sales:** Sales revenue after discounts, according to the defined business calculation.
* **Total Profit:** Net sales minus the applicable cost of goods sold and other included costs.
* **Profit Margin (%):** Total Profit divided by Net Sales, multiplied by 100.
* **Average Order Value (AOV):** Net Sales divided by the number of distinct valid orders.
* **Discount Percentage:** Discount Amount divided by Gross Sales, multiplied by 100, when these fields follow the stated business definitions.
* **Monthly Sales Growth (%):** Current Month Net Sales minus Previous Month Net Sales, divided by Previous Month Net Sales, multiplied by 100.

All measures should use consistent definitions and validated source data.


## 8. Final Business Recommendations

The organization should prioritize protecting profit margins, controlling discounts, and improving data reliability before expanding sales promotions.

Product-level profitability reviews should guide pricing decisions, while monthly sales analysis should support inventory planning and sales target setting. Discount policies should be evaluated using both incremental sales and incremental profit rather than revenue alone.

Management should monitor net sales, total profit, profit margin, average discount percentage, and data-quality error rates regularly to evaluate the effectiveness of implemented actions.

## 9. Conclusion

This project demonstrates how data analytics can transform raw sales data into actionable business insights. By combining data cleaning, data modeling, KPI development, visual analysis, and business recommendations, the organization can better understand its sales performance and identify opportunities for profitable growth.



