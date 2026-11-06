# Introduction to Data Engineering

## 1. What is Data Engineering?

Data Engineering is the discipline of designing, building and maintaining systems that collect, transport, store, transform and deliver data.

A Data Engineer ensures that data is accessible, reliable, organised and available when needed.

## 2. The Data Engineering Lifecycle

I have broken the Data Engineering lifecycle into five main stages.

### 2.1 Data Generation

This is where raw data is produced. Some sources include sensors, applications, websites and other digital systems.

In my DC Power Monitoring project, the ESP32 generates voltage and current readings. This is an example of data generation.

### 2.2 Data Ingestion

Data ingestion is the process of collecting data from different sources and bringing it into a system for storage or processing.

Data can be ingested through protocols and methods such as MQTT, HTTP and file transfers.

In my DC Power Monitoring project, MQTT transports the measurements from the ESP32 to the Python receiver.

### 2.3 Data Storage

Data storage involves saving collected data in dedicated storage systems for future access and processing.

Examples include:

- Relational databases such as PostgreSQL.
- Cloud storage.
- Data warehouses.
- Data lakes.

In my project, measurements are currently stored in JSON and CSV files. A database could be introduced as a future improvement.

### 2.4 Data Processing

Data processing involves manipulating raw data according to specific rules to produce useful information.

Examples include:

- Removing duplicate records.
- Handling missing values.
- Correcting inconsistent data.
- Calculating totals and averages.
- Converting data into suitable formats.

In my project, Python receives and processes the measurements.

### 2.5 Data Consumption

Data consumption is the stage where processed data is made available to users or other systems for use.

Examples include dashboards, reports and analytical applications.

In my project, a Streamlit dashboard displays the measurements and their trends.

## 3. Types of Data

Data can be classified according to how it is organised.

### 3.1 Structured Data

This is data organised according to a predefined structure, commonly in rows and columns.

Example: A PostgreSQL table containing voltage, current and timestamp measurements.

### 3.2 Semi-structured Data

This data does not follow a strict tabular structure but contains identifiable organisation through tags, keys or other metadata.

Example: JSON data from an API or an MQTT message.

### 3.3 Unstructured Data

This is data that does not follow a predefined data model or tabular structure.

Examples include photographs, audio recordings and videos.

## 4. Data Warehouses and Data Lakes

### 4.1 Data Warehouse

A data warehouse stores processed and organised data, mainly for reporting, analysis and business intelligence.

### 4.2 Data Lake

A data lake stores large amounts of data in its original or raw form. It can accommodate structured, semi-structured and unstructured data.

## 5. Data Catalog

A data catalog is an organised inventory of available datasets.

It helps users discover datasets and understand their contents, structure, meaning and origin.

## 6. Data Processing Approaches

### 6.1 ETL vs ELT

ETL and ELT are two approaches used to move and transform data.

**ETL (Extract, Transform, Load)**

Data is extracted from its source, transformed into the required format and then loaded into its destination.

**ELT (Extract, Load, Transform)**

Data is extracted and loaded into the destination first. Transformation is then performed within the destination system.

The main difference is when the transformation takes place.

### 6.2 Batch Processing vs Stream Processing

**Batch Processing**

Batch processing involves collecting data over a specific period and processing it together as a group.

Example: Collecting electricity consumption readings throughout a day and processing them at the end of the day.

**Stream Processing**

Stream processing involves processing incoming data continuously as it is generated or received, usually with low latency.

Example: Monitoring voltage and current readings from an ESP32 system as they arrive.

## 7. Scheduling Data

Data scheduling involves organising tasks to run automatically at specific times or intervals.

For example, a pipeline can be scheduled to collect and process data every hour or every day.

Scheduling helps automate repetitive tasks and ensures that data processing takes place consistently.

## 8. Parallel Computing

Parallel computing involves dividing a large task into smaller tasks that can be processed simultaneously using multiple computing resources.

It helps improve processing speed and efficiency for suitable workloads.

## 9. Cloud and Multicloud Computing

### 9.1 Cloud Computing

Cloud computing involves using computing resources such as storage, databases and processing power over the internet.

Instead of maintaining all infrastructure locally, organisations can use resources provided by cloud service providers.

### 9.2 Multicloud Computing

Multicloud computing involves using services from more than one cloud provider.

Organisations may adopt this approach to access different services, improve flexibility or avoid depending entirely on one provider.

## 10. Practical Application: DC Power Monitoring System

My ESP32-C3 DC Power Monitoring System provides a practical example of how an embedded system can form part of a larger data engineering pipeline.

The system follows these stages:

1. **Data generation:** The ESP32 measures voltage and current.
2. **Data ingestion:** MQTT transports the measurements to a Python receiver.
3. **Data storage:** Measurements are stored in JSON and CSV files.
4. **Data processing:** Python receives and processes the measurements.
5. **Data consumption:** A Streamlit dashboard displays the information.

This project demonstrates how embedded systems can act as data sources in a larger data engineering system.

Possible improvements include introducing a database, implementing data validation and developing more structured data processing operations.

## 11. Key Takeaways

- Data Engineering makes data available, reliable and useful.
- Data pipelines connect data sources to destinations through different stages.
- Data can be structured, semi-structured or unstructured.
- Data warehouses and data lakes serve different storage purposes.
- Data processing improves the quality and usefulness of raw data.
- ETL and ELT differ in when data transformation takes place.
- Batch and stream processing handle data differently.
- Scheduling automates recurring data tasks.
- Parallel computing allows suitable tasks to be processed simultaneously.
- Cloud computing provides access to scalable computing resources.

---

**Course completed:** Understanding Data Engineering  
**Learning path:** Associate Data Engineer in SQL  
**Learning approach:** Theoretical foundation followed by practical implementation.

_By Elvis K_
