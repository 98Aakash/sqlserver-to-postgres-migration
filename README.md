# preface 

This project is about migrating enterprise data from SQL Server to Postgres.

We'll be using  

- Sql
- Python
- Jupyter Notebook 


# Pseudocode

## High Level

1. Audit the data in Sql Server (Before Migration)
2. Extract the data from Sql Server (Ssms)
3. Transform the data 
4. Load The data in Postgres
5. Validate the data (Post Migration)
6. Generate a validation report 

## Low Level 

- create a .env file 
- load the env variables
- connect to sql server (pyodbc)
- connect to postgres db (psycopg2)
- audit the data
- for each table
    - get row count
    - extract all rows
    - transform the columns names to lowercase
    - convert the datatypes
    - create tables in PGDB
    - laod tables in PGDB
- Run post migration checks
- Generate validation report
