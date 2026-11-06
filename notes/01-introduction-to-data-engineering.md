# Understanding Data Engineering

## 1. Introduction

Data Engineering is the field concerned with designing, building and maintaining systems that collect, store, process and deliver data for analysis and decision-making.

A Data Engineer ensures that data is accessible, reliable, organised and available when needed.

## 2. Data Pipelines

A data pipeline is a sequence of processes through which data moves from a source to a destination.

Typical stages include:

1. Data generation or collection.
2. Data ingestion.
3. Data storage.
4. Data processing and transformation.
5. Data delivery for analysis.

Pipelines can be automated to ensure that data moves efficiently and consistently.

## 3. Data Structures

Data structures describe how data is organised and stored.

Common examples include:

- Structured data: organised into rows and columns.
- Semi-structured data: has some organisation but does not follow a strict tabular structure, e.g. JSON.
- Unstructured data: does not follow a predefined structure, e.g. images, audio and videos.

## 4. Data Warehouses and Data Lakes

### Data Warehouse

A data warehouse stores processed and organised data, mainly for reporting, analysis and business intelligence.

### Data Lake

A data lake stores large amounts of data in its original or raw form. It can accommodate structured, semi-structured and unstructured data.

## 5. Data Catalog

A data catalog is an organised inventory of available datasets.

It helps users discover datasets and understand their contents, structure, meaning and origin.

## 6. Data Processing

Data processing involves transforming raw data into a useful and meaningful form.

Examples include:

- Removing duplicate records.
- Handling missing values.
- Correcting inconsistent data.
- Calculating totals and averages.
- Converting data into suitable formats.

Two common approaches are:

- ETL (Extract, Transform, Load): data is transformed before being loaded into its destination.
- ELT (Extract, Load, Transform): data is loaded first and transformed within the destination system.

## 7. Scheduling Data

Data scheduling involves organising tasks to run automatically at specific times or intervals.

For example, a pipeline can be scheduled to collect and process data every hour or every day.

## 8. Batch and Stream Processing

### Batch Processing

Data is collected over a period and processed in groups at scheduled intervals.

Example: Processing all electricity consumption readings collected during a day.

### Stream Processing

Data is processed continuously as it is generated or received.

Example: Monitoring voltage and current readings from an ESP32 system in real time.

## 9. Parallel Computing

Parallel computing involves dividing a large task into smaller tasks that can be processed simultaneously using multiple computing resources.

It helps improve processing speed and efficiency for suitable workloads.

## 10. Cloud and Multicloud Computing

### Cloud Computing

Cloud computing involves using computing resources such as storage, databases and processing power over the internet.

### Multicloud Computing

Multicloud computing involves using services from more than one cloud provider.

## 11. Application to My DC Power Monitoring Project

My ESP32-C3 DC Power Monitoring System provides a practical example of a data pipeline.

The system:

1. Generates voltage and current readings.
2. Publishes measurements through MQTT.
3. Uses a Python receiver to collect incoming data.
4. Stores measurements in JSON and CSV files.
5. Uses a Streamlit dashboard to display readings and trends.

This project demonstrates data generation, ingestion, storage and visualisation.

A possible improvement is to introduce a database, data validation and structured processing to develop it into a more complete Data Engineering pipeline.

## 12. Key Takeaways

- Data Engineering makes data available and useful.
- Data pipelines connect data sources to destinations.
- Data lakes and warehouses serve different storage purposes.
- Data processing improves data quality and usability.
- Batch and stream processing handle data in different ways.
- Scheduling automates recurring data tasks.
- Cloud computing provides scalable computing resources.

**Course completed:** Understanding Data Engineering  
**Learning path:** Associate Data Engineer in SQL  
**Learning approach:** Theoretical foundation followed by practical implementation.

_By Elvis K_
