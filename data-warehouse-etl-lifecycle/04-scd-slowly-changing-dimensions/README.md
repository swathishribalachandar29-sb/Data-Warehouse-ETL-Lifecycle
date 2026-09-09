# Module 4 — Slowly Changing Dimensions (SCD)

📹 **Video walkthrough:** [https://youtu.be/-uZ1fGv41mQ]

> Demonstrated how a data warehouse can preserve historical context when source-system attributes change over time.

## Summary

Implemented Slowly Changing Dimension strategies for product data using Pentaho Data Integration. I worked with Type 1, Type 2, and hybrid approaches, using surrogate keys, versioning, effective date ranges, and current-record indicators to manage changing dimensional attributes and preserve historical information.

## What I did

I worked with product data containing changes over time and implemented different Slowly Changing Dimension strategies using Pentaho.

I worked with **SCD Type 1**, where changes to dimensional attributes are updated directly rather than maintaining historical versions.

I then implemented **SCD Type 2**, where changes are preserved as historical records. The dimension uses fields such as:

- `product_sk` — surrogate/technical key
- `version`
- `date_from`
- `date_to`
- `is_current`

This allows the warehouse to maintain multiple versions of a product and determine which version was valid during a particular period.

I also worked with a **hybrid dimension** implementation, configuring the dimension lookup/update process and working with fields such as `ProductName`, `Category`, and `Brand`.

I used product source data containing changes across transaction dates — for example, product attributes changing over time — and loaded those changes into the dimensional tables.

Finally, I queried the resulting tables in SQLyog to inspect the stored versions and verify the SCD implementation.

## Concepts demonstrated

- Slowly Changing Dimensions
- SCD Type 1
- SCD Type 2
- Hybrid SCD
- Historical data tracking
- Surrogate keys
- Effective dates
- Versioning
- Current-record flags
- Dimension lookup/update
- Pentaho Data Integration
- MySQL
- Data warehouse dimensional modeling
