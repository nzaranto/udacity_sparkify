# Data Engineer Nanodegree - Project 1: Data Modeling with Postgres

## PROJECT DESCRIPTION
This project aims at the creation of a Postgres database and ETL pipeline to optimize queries for a startup called Sparkify that wants to analyze the data they've been collecting on songs and user activity on their new music streaming app.
The data resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

(sparkifydb_erd.png)

### SCHEMA DESIGN
The star schema have one fact table (songplays) and four dimension tables (users, songs, artists, time).

### FILES DESCRIPTION

- `sql_queries.py` contains the CREATE, DROP and SELECT queries
- `create_tables.py` drops and creates the tables
- `etl.ipynb` reads and processes a single file from song_data and log_data and loads the data into the tables
- `etl.py` reads and processes all files from song_data and log_data and loads them into the tables
- `sanity-test.ipynb` run tests to evaluate if there are any mistake on the design of the database

### HOW TO RUN THE SCRIPTS
For the correct output the follow steps must be followed:
- Run `create_tables.py` to create the database
- [OPTIONAL] Run `etl.ipynb` to verify the ETL process step by step
- Run `etl.py` to read and load the data
- Run the `test.ipnyb` to verify if the correct output was achieved
