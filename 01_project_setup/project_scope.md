# UK River & Flood Monitoring Data Pipeline

## Project Overview

This project will build an end-to-end data engineering pipeline using real public data from the Environment Agency Real-Time Flood Monitoring API.

The project will use Python to extract and process data from the API and SQL Server to store, query and transform the data.

The project will initially focus on a small geographical area so that the pipeline can be developed and tested using a manageable amount of data. The scope can then be expanded as the pipeline develops.

## Phase 1 Objectives

The initial phase will:

* Connect to the Environment Agency Flood Monitoring API using Python.
* Retrieve monitoring station data for a selected geographical area.
* Retrieve measures and readings associated with those stations.
* Understand and parse the JSON returned by the API.
* Store the original API responses as raw JSON files.
* Validate important fields before loading the data.
* Create SQL Server staging tables.
* Load validated data into SQL Server.
* Query and explore the loaded data using SQL.

## Initial Pipeline

Environment Agency API → Python Extraction → Raw JSON → Python Validation → SQL Server Staging → SQL Queries

## Learning Objectives

The project will provide practical experience with:

* Python fundamentals.
* Working with REST APIs.
* JSON, dictionaries and lists.
* Python functions and modules.
* Exception handling.
* SQL database and table design.
* Primary and foreign keys.
* SQL joins and transformations.
* Data validation.
* ETL/ELT concepts.
* Git branching and collaborative development.

## Future Scope

Later phases may introduce:

* Incremental data loading.
* Larger geographical coverage.
* Automated data quality checks.
* Logging and error handling.
* Historical river-level analysis.
* Analytical/data warehouse modelling.
* Indexing and query optimisation.
* Pipeline orchestration.
* Automated testing.
* CI/CD.
