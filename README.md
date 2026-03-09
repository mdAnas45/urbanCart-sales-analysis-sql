🛒 UrbanCart E-Commerce Data Analysis (SQL)
📌 Overview

This project presents a comprehensive E-Commerce Data Analysis performed using PostgreSQL on the UrbanCart retail dataset.

The analysis explores key aspects of an online retail business including:

Customer behavior

Sales performance

Product demand

Payment patterns

Cross-selling opportunities

Using structured SQL queries, the project transforms raw transactional data into business insights that can support data-driven decision making.

🎯 Project Purpose

The purpose of this analysis is to help businesses:

Understand customer purchasing behavior

Identify top performing products and categories

Measure sales and revenue performance

Analyze customer demographics and geographic trends

Detect cross-selling opportunities between products

🛠 Tech Stack

PostgreSQL – Data analysis and querying

Joins – Combining multiple tables for analysis

Aggregation Functions – Revenue, order counts, averages

CTEs (Common Table Expressions) – Structured query building

Date Functions – Time-based trend analysis

Self Joins – Product co-occurrence analysis

📂 Dataset Structure

The dataset follows a Star Schema design.

Fact Tables

Fact_orders – Order level information

FactOrderItem – Product level order details

FactPayments – Payment transactions

Dimension Tables

DimCustomers – Customer demographic data

DimProducts – Product details and inventory

This structure enables efficient business intelligence style analysis.

🧠 Business Problems Addressed

This project answers several key business questions such as:

How many orders and customers does the platform have?

Which cities generate the most orders?

What is the total revenue and average order value?

Which products and categories perform best?

Which customers generate the highest revenue?

Which payment methods are most popular?

Which products are frequently purchased together?

📊 Analysis Areas
1️⃣ Customer & Order Fundamentals

Basic business metrics were analyzed including:

Total number of orders

Unique customers

Repeat customer percentage

Monthly order trends

Example metric:

COUNT(DISTINCT Order_id)

This helps measure customer activity and platform growth.

2️⃣ Sales & Revenue Analysis

Revenue was calculated using:

quantity * unit_price

Key insights analyzed:

Total revenue

Revenue by product category

Top revenue-generating products

Average Order Value (AOV)

Average basket size

These metrics help evaluate overall business performance.

3️⃣ Customer Insights

Customer purchasing patterns were analyzed using:

Customer lifetime revenue

City-level order performance

Gender-based purchasing behavior

Customer activity over time

Example insight:

SUM(quantity * unit_price)

This helps identify high-value customers and target audiences.

4️⃣ Inventory & Product Demand

Products were analyzed to detect potential stock-out risks based on:

High sales volume

Low inventory levels

This helps businesses improve inventory management.

5️⃣ Payment Behavior Analysis

Payment data was used to analyze:

Most frequently used payment methods

Relationship between payment methods and order status

Payment preferences by city

Average order size by payment method

These insights help improve checkout optimization and payment strategy.

6️⃣ Market Basket Analysis (Product Co-Occurrence)

Self-joins were used to identify products frequently purchased together.

Example concept:

f1.order_id = f2.order_id
AND f1.product_id < f2.product_id

This analysis identifies:

Product bundles

Cross-selling opportunities

Frequently paired products

📈 Example Business Insights

The analysis can reveal insights such as:

Certain cities contribute significantly more orders

A small group of customers generates large portions of revenue

Some products show high demand and stock risk

Specific products are frequently purchased together

Payment method preferences vary by customer location

💡 Business Value

This project helps businesses:

Improve customer understanding

Optimize inventory management

Identify high-value customers

Design product bundling strategies

Improve marketing and sales strategies

📌 SQL Concepts Demonstrated

This project demonstrates several important SQL techniques:

Multi-table joins

CTEs

Aggregations

Date manipulation

Window functions

Self joins

Conditional filtering

Business KPI calculations

🚀 Conclusion

This project demonstrates how SQL can be used as a powerful analytical tool to transform raw e-commerce data into meaningful business insights.

By analyzing customers, orders, products, and payments, businesses can make better decisions to improve revenue, customer retention, and operational efficiency.

👤 Author

Anas
Aspiring Data Analyst

Skills:
Excel | Power BI | SQL | Python
