# Introduction to SQL

## Course Information

- **Platform:** DataCamp
- **Learning Path:** Associate Data Engineer in SQL
- **Course:** Introduction to SQL
- **Status:** Completed
- **Level:** Beginner

## 1. What is SQL?

SQL (Structured Query Language) is a language used to communicate with relational databases.

It allows users to retrieve, organise, filter and manipulate data stored in database tables.

SQL is an important skill in Data Engineering because data engineers work with databases to store, process and retrieve data.

## 2. Relational Databases

A relational database organises information into tables.

A table consists of:

- **Rows:** Individual records in a table.
- **Columns:** Attributes or properties describing each record.
- **Data types:** Define the kind of information a column can store.

For example, an employees table could contain employee IDs, names, departments and salaries.

## 3. Database Schemas

A schema describes the organisation and structure of a database.

It defines how database objects, such as tables and views, are organised.

Schemas help maintain order and make databases easier to manage.

## 4. Naming Rules

Database objects should have meaningful and consistent names.

Good naming practices include:

- Using descriptive names.
- Avoiding unnecessary spaces.
- Maintaining consistency.
- Avoiding reserved SQL keywords as object names.
- Using underscores where appropriate.

Example:

`employee_records` is clearer than `table1`.

## 5. Data Types

Data types specify the kind of data that can be stored in a database column.

Common SQL data types include:

| Data type | Purpose                           | Example      |
| --------- | --------------------------------- | ------------ |
| INTEGER   | Whole numbers                     | 25           |
| DECIMAL   | Decimal numbers                   | 125.50       |
| NUMERIC   | Exact decimal values              | 125.50       |
| FLOAT     | Approximate floating-point values | 125.56789    |
| VARCHAR   | Variable-length text              | 'Elvis'      |
| DATE      | Calendar dates                    | '2026-11-09' |
| BOOLEAN   | True or false values              | TRUE         |

Choosing appropriate data types helps maintain data consistency and accuracy.

## 6. Basic SQL Query Structure

SQL uses keywords to communicate instructions to a database.

### SELECT

Specifies the columns to retrieve.

```sql
SELECT name, department
FROM employees;
```

### FROM

Specifies the table from which data is retrieved.

```sql
SELECT *
FROM employees;
```

The asterisk (`*`) selects all columns.

### AS

Creates an alias for a column or table in a query result.

```sql
SELECT salary AS employee_salary
FROM employees;
```

### DISTINCT

Returns unique values, eliminating duplicates from the query result.

```sql
SELECT DISTINCT department
FROM employees;
```

### VIEW

A view is a virtual table based on a saved SQL query.

It allows users to access selected data without repeatedly writing the same query.

Example:

```sql
CREATE VIEW employee_departments AS
SELECT DISTINCT department
FROM employees;
```

## 7. SQL Keywords

SQL keywords are reserved words that perform specific functions in a query.

Examples include:

- SELECT
- FROM
- AS
- DISTINCT
- CREATE
- VIEW

SQL keywords are generally written in uppercase for readability, although SQL is commonly case-insensitive for keywords.

## 8. Why SQL Matters in Data Engineering

SQL is essential in Data Engineering because it helps engineers:

1. Retrieve information from databases.
2. Organise and manage structured data.
3. Filter and analyse records.
4. Transform data for further processing.
5. Support data pipelines and reporting systems.

## 9. Practical Application to My DC Power Monitoring Project

The concepts learned in this course will help me extend my existing DC Power Monitoring System.

Instead of relying only on CSV files, I can eventually store electrical measurements in a relational database.

A possible measurements table could contain:

| Column    | Data type      |
| --------- | -------------- |
| id        | INTEGER        |
| voltage   | NUMERIC        |
| current   | NUMERIC        |
| power     | NUMERIC        |
| timestamp | DATE/TIMESTAMP |

SQL queries could then retrieve measurements, calculate summaries and identify unusual readings.

## 10. Key Takeaways

- SQL is used to communicate with relational databases.
- Databases organise information into tables.
- Tables contain rows and columns.
- Schemas describe database organisation.
- Data types determine what information columns can store.
- SQL keywords perform specific operations.
- SELECT and FROM form the foundation of basic data retrieval.
- AS creates aliases, while DISTINCT retrieves unique values.
- Views provide reusable, virtual representations of query results.

**Learning milestone:** Successfully completed the Introduction to SQL course on DataCamp.

_By Elvis K_
