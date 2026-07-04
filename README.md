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

1. create a .env file 
2. load the env variables
3. connect to sql server (pyodbc)
4. connect to postgres db (psycopg2)
5. audit the data
6. for each table
7. get row count
8. extract all rows
9. transform the columns names to lowercase
10. convert the datatypes
11. create tables in PGDB
12. laod tables in PGDB
13. Run post migration checks
14. Generate validation report
