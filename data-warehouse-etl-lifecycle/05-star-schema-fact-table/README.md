# Module 5 — Building a Sales Star Schema & Fact Table

📹 **Video walkthrough:** [https://youtu.be/nHwJ_NIy8Wo]

## Summary

Built a sales data warehouse using a Star Schema with date, customer, and product dimensions and a central sales fact table. Developed the ETL workflow from staging data into dimensional tables and the fact table, applied surrogate-key and effective-date lookups, and validated the warehouse through source-to-target row and quantity reconciliation.

## What I did

I designed and implemented a sales data warehouse using a **Star Schema**.

I created dimensional structures including:

- `dim_date`
- `dim_customer`
- `dim_product`

and a central:

- `fact_sales`

table.

The fact table contains measures and transactional information such as:

- Quantity
- Unit Price
- Discount
- Tax Amount
- Shipping Cost
- Transaction ID
- Line Number

I also worked with surrogate keys such as `DateSkey`, `CustomerSkey`, and `product_key` to connect transactional data to the appropriate dimensions.

For customer and product dimensions, I used effective date ranges so that the fact records could be associated with the correct historical dimension version.

The ETL process included staging source sales data and then building the final fact table by joining the staged data with the relevant dimensions.

One particularly important part of the implementation was the fact-table SQL:

- Join sales to the date dimension
- Lookup the customer dimension
- Lookup the product dimension
- Match records based on their effective date ranges
- Handle missing dimension keys using default values

I then validated the resulting warehouse using SQL queries. For example, I compared `COUNT(*)` and `SUM(Quantity)` between the staging source and the resulting fact table to verify that the data loaded correctly.

I also checked distinct product keys and inspected the contents of the fact and dimension tables.

## Concepts demonstrated

- Data warehouse architecture
- Star schema
- Fact tables
- Dimension tables
- Staging tables
- Surrogate keys
- Date dimension
- Customer dimension
- Product dimension
- Historical dimension lookup
- Effective date ranges
- ETL orchestration
- Data validation
- Source-to-target reconciliation
- Pentaho
- MySQL / SQLyog
- MySQL Workbench
