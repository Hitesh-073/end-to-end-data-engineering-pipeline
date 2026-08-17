# Pipeline Architecture

## Phase 1 Architecture

The initial pipeline will follow the following data flow:

Environment Agency Flood Monitoring API

↓

Python API Request

↓

JSON Response

↓

Raw JSON Storage

↓

Python Validation

↓

SQL Server Staging Tables

↓

SQL Queries and Transformations

## Components

### Source

Environment Agency Real-Time Flood Monitoring API.

### Extraction

Python will make HTTP requests to the API and retrieve JSON responses.

### Raw Layer

The original API responses will be stored in the `02_ingestion/raw_data/` directory.

### Validation

Python will validate required fields and basic data structures before data is loaded into SQL Server.

### Staging Layer

SQL Server staging tables will receive data extracted from the API.

### Transformation

SQL will be used to clean, transform and prepare the staged data for analysis.

## Future Architecture

Additional components such as incremental loading, logging, orchestration, automated testing and analytical models will be introduced in later phases.
