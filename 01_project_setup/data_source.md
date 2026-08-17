# Data Source

## Source

Environment Agency Real-Time Flood Monitoring API

The Environment Agency provides public access to real-time flood monitoring information for England.

API documentation:

https://environment.data.gov.uk/flood-monitoring/doc/reference

## Data Format

The API returns data in JSON format.

Python will be used to request the data, inspect the API response and extract the required information.

## Authentication

The API is publicly accessible and does not require an API key for the endpoints initially used by this project.

## Initial Data

Phase 1 will focus primarily on three related types of data:

### Stations

Monitoring stations identify locations where environmental measurements are collected.

Examples of useful attributes include:

* Station reference
* Station name
* River name
* Town
* Catchment
* Latitude
* Longitude

### Measures

Measures describe what is being measured at a monitoring station.

Examples include:

* Parameter
* Parameter name
* Qualifier
* Unit
* Measurement period

### Readings

Readings contain observations recorded for a particular measure.

Important attributes include:

* Measure
* Date/time
* Value

## Initial Geographical Scope

The project will initially retrieve data for a limited geographical area or subset of monitoring stations.

This will allow the ingestion and database pipeline to be developed using a manageable dataset before expanding the geographical coverage in later phases.

## Data Storage

Raw API responses will initially be retained as JSON files before validated data is loaded into SQL Server.

This provides a raw copy of the source data and separates extraction from downstream processing.

## Future Considerations

As the project develops, the data source may be used to explore:

* Historical readings.
* Incremental API extraction.
* Additional monitoring stations.
* Larger geographical coverage.
* Flood warnings.
* Data quality issues.
* Changes in river levels over time.
