# Introduction to Data Engineering

## 1. What is Data Engineering?

Data Engineering is the discipline of designing, building and maintaining systems that collect, transport, store, transform and deliver data

## 2. The Data Engineering Lifecycle

I've broken the data engineering cycle into 5 parts

- ### Data generation

  This is where raw data is produced. Some sources include; Sensors, Applications, Websites, etc  
  In my repository DC Power Monitor, The ESP32 generates voltage and current readings. That process falls in this category

- ### Data ingestion

  Data ingestion is the process of collecting data from different sources and bringing it into a system for storage or processing. Data can be ingested through protocols such as MQTT, HTTP and file transfers.

- ### Data storage

  It is the process of saving data in dedicated storage sites. Examples are; Cloud storage, PostgreSQL, etc.  
  In the repository.

- ### Data Processing

  It's the manipulation of data to generate desired information. Manipulation is done by following specific set of rules.  
  In the repository, Python receives and processes the data

- ### Data Consumption
  It's the desired visible output generated once processing is done.  
  In the repository, A dashboard displays the results obtained.

## 3. Types of Data

### 1. Structured

### 1. Structured Data

This is data organised according to a predefined structure. They are commonly stored in rows and columns.

Example: A PostgreSQL table containing voltage, current
and timestamp measurements.

### 2. Semi-structured

JSON data form an API or MQTT message

### 3. Unstructured

They include photographs or audio messages

## 4. Batch Processing vs Stream Processing

Batch processing is collection of data over a specific period of time and processing it all together.

Streaming is processing incoming data continuously or in real time as it arrives, usually in low latency

## 5. ETL vs ELT

ETL transforms data before loading it to the desired destination  
ELT loads raw data first then transforms it within the desired destination system.

## 6. Practical Application: DC Power Monitoring

My DC Power Monitoring project provides a practical example
of a data pipeline.

1. Data generation: ESP32 measures voltage and current.
2. Data ingestion: MQTT transports measurements.
3. Data storage: Measurements can be stored in a database.
4. Data processing: Python processes the received measurements.
5. Data consumption: A dashboard displays the information.

This demonstrates how embedded systems can act as data
sources in a larger data engineering system.

_By Elvis K_
