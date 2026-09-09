# Module 7 — AI-Assisted SQL & Data Warehouse Analytics

📹 **Video walkthrough:** [https://youtu.be/pkAxV79C5CE]

## Summary

Analyzed the AdventureWorks data warehouse using SQL to answer business questions around product pricing, salesperson revenue, product-category performance, and sales territories. I also explored AI-assisted database querying through an MCP-connected AI assistant, using natural-language questions to generate analytical results and validating the results against direct SQL queries.

## What I did

I worked with the AdventureWorks data warehouse and used SQL to answer business-oriented analytical questions from the warehouse.

I queried the database to analyze areas such as:

- Top 10 most expensive products
- Salespeople generating the highest revenue
- Product categories contributing to Internet Sales
- Sales by territory
- Regional sales performance

For example, I queried product information and ordered products based on their list price to identify the most expensive products in the warehouse.

I also analyzed salesperson performance by aggregating sales revenue and ranking salespeople from highest to lowest total revenue.

For Internet Sales, I joined the appropriate product/category and sales information to determine which product categories contributed the most revenue and visualized the results.

I also analyzed sales territory data to determine which territories generated the highest sales.

### AI component

A particularly useful part of this assignment was using an AI assistant connected to the database through an MCP server.

Instead of manually writing every query from scratch, I could ask questions in natural language such as:

> "What are the top 10 most expensive products in the data warehouse?"

The AI assistant used the database connection to work with the underlying AdventureWorks data and return the results.

I then compared/validated the AI-generated results against SQL queries executed directly against the database.

So the workflow demonstrated:

**Natural-language question → AI → SQL/database → analytical result**

rather than simply using AI as a chatbot with no connection to actual data.

## Concepts demonstrated

- SQL analytics
- Data warehouse querying
- Aggregations
- GROUP BY / ORDER BY
- Joins
- Ranking
- Business intelligence questions
- Sales analysis
- Product analysis
- Customer/territory analysis
- AdventureWorks data warehouse
- AI-assisted SQL
- MCP (Model Context Protocol)
- Natural-language database interaction
- Result validation
- Data visualization

## Bridge to Data Analysis

This module bridges Data Engineering into Business Analysis: **Data Engineering → Data Warehouse → SQL → Business Analysis → AI-assisted analytics.**
