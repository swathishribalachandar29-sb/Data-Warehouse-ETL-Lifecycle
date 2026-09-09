# Data Warehouse & ETL Lifecycle 

End-to-end, hands-on implementation of the data warehousing lifecycle - from raw source extraction to AI-assisted business analytics - built using **Pentaho Data Integration**, **MySQL**, and **MySQL Workbench / SQLyog**.

## The story

My hands-on work here covers the end-to-end data lifecycle - from extracting data from files and APIs, transforming and loading data into relational databases, designing dimensional models, managing historical changes with SCD strategies, building star schemas, validating data, and using AI-assisted interfaces to query data warehouses for business insights.

## Lifecycle overview

| # | Module | What it demonstrates | Flow |
|---|--------|----------------------|------|
| 1 | [ETL: JSON → MySQL](./01-etl-json-to-mysql) | File-based extraction & load | JSON source → Transform → MySQL |
| 2 | [Data Modeling & Relational Design](./02-data-modeling-relational-design) | Conceptual → relational → schema | Business requirements → Conceptual model → Relational model → Schema |
| 3 | [SQL Validation & Reverse Engineering](./03-sql-validation-reverse-engineering) | Querying & schema verification | Database → SQL joins → Validation → Reverse-engineered ER model |
| 4 | [Slowly Changing Dimensions](./04-scd-slowly-changing-dimensions) | Historical data tracking | Changing source data → SCD Type 1 / 2 / Hybrid → Historical dimension data |
| 5 | [Star Schema & Fact Table](./05-star-schema-fact-table) | Dimensional warehouse design | Staging → Dimensions → Fact table → Star schema → Source-to-target validation |
| 6 | [API-Based ETL](./06-api-based-etl) | Semi-structured/API extraction | External API → JSON response → Transformation → MySQL |
| 7 | [AI-Assisted SQL Analytics](./07-ai-assisted-sql-analytics) | NL-to-SQL business analysis | Natural-language question → AI/MCP → SQL/Database → Business insight |

## Why these fit together

- **Modules 1–3** cover the fundamentals: getting data in, modeling it properly, and validating it.
- **Modules 4–5** move into real data warehousing concepts - historical tracking and dimensional modeling - the parts of the lifecycle that separate basic ETL from data warehouse engineering.
- **Module 6** shows the same ETL discipline applied to a different source type (API/JSON vs. file).
- **Module 7** bridges data engineering into business analysis, using an AI assistant connected to the warehouse via MCP to answer natural-language questions - validated against direct SQL.

## Tech stack

`Pentaho Data Integration (Spoon)` · `MySQL` · `MySQL Workbench` · `SQLyog` · `SQL DDL/DML` · `REST API integration` · `AI-assisted SQL via MCP`

## Video walkthroughs

Each module folder links to a short recorded walkthrough demonstrating the pipeline running end to end.
