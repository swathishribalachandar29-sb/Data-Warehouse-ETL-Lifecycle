# Module 1 — ETL: Extracting and Loading Employee/Project Data

📹 **Video walkthrough:** [https://youtu.be/Rm64VGg9euI]

## Summary

Built an ETL workflow using Pentaho Data Integration to extract employee and project data from JSON sources, transform the data, and load it into MySQL. Created reusable transformations and an orchestrating job while validating the pipeline through execution logs and output records.

## What I did

I built an ETL workflow in Pentaho Data Integration (Spoon) to extract employee and project information from JSON sources and load the processed data into a MySQL data warehouse.

I created separate transformations for employee/project data and used steps such as JSON Input and Select Values to read and prepare the source data. I then loaded the transformed records into MySQL tables such as `raw_emp_projects`.

I also created a main job to coordinate the individual extraction workflows and verified the execution through Pentaho's logging and transformation results.

The recording shows the transformation processing 6 employee/project records and successfully writing them to the database.

## Concepts demonstrated

- ETL pipeline development
- Data extraction from JSON
- Data transformation
- Data loading into MySQL
- Pentaho Data Integration / Spoon
- Job orchestration
- Database connectivity
- ETL validation and execution monitoring
