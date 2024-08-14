# Data Analytics Project

## Overview

This repository contains code for a data analytics project that spans multiple technologies: Python, SQL, and C#. The project demonstrates how to process, analyze, and manipulate sales data using Python, SQL Server, and C#. The Python script handles data preparation, SQL script performs the analysis, and the C# program integrates with the SQL Server database.

## Files

### 1. `Data Analytics.py`
This Python script performs the following tasks:
- **Data Loading**: Reads a CSV file containing sales data using pandas.
- **Data Cleaning and Transformation**:
  - Renames columns to follow a consistent format.
  - Handles missing values and performs calculations to create new columns (`discount`, `sale_price`, `profit`).
  - Converts date columns from string to datetime format.
  - Drops unnecessary columns that are not needed for analysis.
- **Database Interaction**: 
  - Establishes a connection to a local SQL Server instance.
  - Creates a table in the SQL Server database and loads the processed data into this table.

### 2. `SQL.sql`
This SQL script includes:
- **Table Creation**: SQL statements to create tables in the SQL Server database.
- **Data Insertion**: Queries to insert data into the tables.
- **Data Analysis**:
  - Aggregates sales data by region and product.
  - Compares sales across different years to identify trends.
  - Uses Common Table Expressions (CTEs) and window functions to perform more complex queries.

### 3. `Program.cs`
This C# program performs the following tasks:
- **Database Connection**: Establishes a connection to the SQL Server database.
- **SQL Query Execution**: Executes SQL queries against the database, possibly for further data manipulation or fetching results.
- **Error Handling**: Manages exceptions that may occur during database operations.
- **Integration**: Can be used to integrate the results of SQL queries into a .NET application, or to perform additional business logic on the data.

## How to Use

### Prerequisites
- Python 3.x
- Pandas library
- SQLAlchemy library
- Microsoft SQL Server
- ODBC Driver 17 for SQL Server
- .NET SDK (for running the C# program)

### Steps to Run the Project

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your_username/your_repository.git
    ```

2. **Run the Python Script**:
   - Ensure the path to the CSV file is correct in the script.
   - Execute the script to load the data into your SQL Server database.

3. **Execute SQL Queries**:
   - Run the SQL script (`SQL.sql`) in SQL Server Management Studio (SSMS) or using SQLCMD to create the necessary tables and perform the analyses.

4. **Run the C# Program**:
   - Ensure that the connection string in the `Program.cs` file points to your SQL Server database.
   - Compile and run the C# program to execute any additional SQL operations or integrate the data into a .NET application.

## Project Insights
- This project showcases how to integrate Python, SQL, and C# for a full-stack data analytics solution.
- Python is used for data cleaning and preparation.
- SQL is used for complex queries and analysis.
- C# can be used for application integration or further processing of the data.

