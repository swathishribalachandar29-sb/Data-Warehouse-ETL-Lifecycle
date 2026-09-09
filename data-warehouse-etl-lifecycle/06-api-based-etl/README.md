# Module 6 — API-Based Data Extraction & ETL

📹 **Video walkthrough:** [https://youtu.be/wE0wSW5s4Dw]

## Summary

Built an API-driven ETL workflow using Pentaho Data Integration to extract professional profile data from an external API. Processed JSON responses, selected relevant attributes such as experience and education, transformed the semi-structured data into usable records, and validated the extracted data in MySQL.

## What I did

I built an ETL workflow in Pentaho Data Integration (Spoon) to extract professional profile data from an external API and convert the API responses into structured data that could be processed further.

I used the Enrich Layer API to retrieve profile information. I created a workflow that first built a set of profile URLs and then called the API for the profiles individually.

The API response was returned in JSON format, so I configured Pentaho to process the JSON response and extract relevant fields. I worked with different pieces of profile information such as demographics, experience, education, and language-related data.

The workflow included steps for:

- Preparing profile URLs
- Calling the external API
- Receiving JSON responses
- Parsing the JSON
- Selecting the required fields
- Writing the processed output to files

I also configured the API authentication using an API key and executed the Pentaho transformation to verify that the pipeline successfully processed the data.

Finally, I checked the resulting data in MySQL to confirm that the extracted information was available in a structured form.

## Concepts demonstrated

- API-based data extraction
- ETL pipeline development
- REST API integration
- JSON processing
- Data transformation
- Data extraction from semi-structured data
- API authentication
- Pentaho Data Integration
- MySQL
- Data validation
- External data-source integration

## Why this one stands out

Module 1 shows: **File/JSON → Transform → Database**.
Module 6 shows: **External API → JSON → Transform → Structured Data**.

That distinction is worth highlighting — real data engineering often involves pulling data from APIs, not just static files.
