# Introduction to Data Engineering

## 1. What is Data Engineering?

Data Engineering is the discipline of designing, building and maintaining systems that collect, transport, store, transform and deliver data

## 2. The Data Engineering Lifecycle

I've broken data engineering cycle into 5 parts

- ### Data generation

  This is where raw data is produced. Some sources include; Sensors, Applications, Websites, etc  
  In my repository DC Power Monitor, The ESP32 generates voltage and current readings. That process falls in this category

- ### Data ingestion

  This is the transmission of data from the source to the dedicated destination via specific protocols. Example MQTT.  
  In the repository, MQTT broker transports the readings. That process falls in this category.

- ### Data storage

  It the process of saving data in dedicated storage sites. Examples are; Cloud storage, PostgreSQL, etc.  
  In the repository, a database stores the measurements.

- ### Data Processing

  It's the manipulation of data to generate desired information. Manipulation is done by following specific set of rules.  
  In the repository, python receives and processes the data

- ### Data Consumption
  It's the desired visible output generated once processing is done.  
  In the repository, A dashboard displays the results obtained.

## 3. Types of Data

### 1. Structured

These are data organised in rows and columns.

### 2. Semi-structured

JSON data form an API or MQTT message

### 3. Unstructured

They include photographs or audio messages

## 4. Batch Processing vs Stream Processing

Batch processing is collection of data over a specific period of time and processing it all together.

Streaming is processing incoming data continuously or in real time

## 5. ETL vs ELT

ETL transforms data before loading it to the desired destination  
ELT loads raw data first then transforms it withing the desired destination system.

_By Elvis K_
