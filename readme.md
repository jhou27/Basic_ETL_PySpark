This repo contains scripts to perform ETL operations using PySpark
We use two types of sources, MySQL as a database and CSV file as a filesystem, We divided the code into 3 major parts- 1. Extract 2. Transform 3. Load.//
There are 4 python scripts:
job.py — Execute ETL operations stepwise (Extract Transform and Load)
constant.py — To store all the constant details like columns, spark instance, and columns related to joins.
extract.py — Extract the source data by creating dataframe.
transform.py — All transformation logic is present here. We will use extracted dataframes to do all the transformations.
load.py — Store cleaned data into a database or filesystem
