# SCD-2-Implementation
![alt_text](https://images.unsplash.com/photo-1511984804822-e16ba72f5848?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=580&q=80)


## Introduction
A company X wants to keep its employee data up to date in their central database. Since, over the time, many employees prefer to change their base location, it is essential to update the employee information in the company's central database. 

## Problem statement
The field 'Location' is a Slowly changing Dimension (  a dimension whose attribute or attributes for a record (row) change slowly over time). We will be using SCD-2 type implementation to keep a full history of dimension data in the table. The Type 2 Dimension mapping filters source rows based on user-defined comparisons and inserts both new and changed dimensions into the target. Changes are tracked in the target table by looking up the primary key and creating a version number for each dimension in the table called a surrogate key.  

## ETL Process
We are sourcing the data from MS SQL Server, transforming it using Informatica and loading it to Oracle server. 

## Source Database
![alt_text](https://github.com/faraaznx/SCD-2-Implementation-/blob/main/Source.png)

## Target Database
![alt_text](https://github.com/faraaznx/SCD-2-Implementation-/blob/main/Target.png)

## Source Table
![alt_text](https://github.com/faraaznx/SCD-2-Implementation-/blob/main/Souce_table.png)

## Target Table
![alt_text](https://github.com/faraaznx/SCD-2-Implementation-/blob/main/Oracle_Result.png)

## ETL Pipeline
![alt_text](https://github.com/faraaznx/SCD-2-Implementation-/blob/main/Mapping.png)
