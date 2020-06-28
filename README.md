# Movies-ETL

## Objective
- Create an automated ETL pipeline 
  - Extract data from multiple sources
  - Clean and transform the data automatically using Pandas and regular expressions
  - Load new data into PostgreSQL

### Technologies
- Write Python script that performs all three ETL steps on Wikipedia and Kaggle dataset

This project involves extracting, transforming, and loading into a database.  Extraction was made from Wikipedia and Kaggle.  Transformation involves cleaning and joining relevant datasets.  Loading the data involves loading cleaned dataset into a SQL database.

## Assumptions
1. Due to the large amount of data, only first 5 and last 5 records were observed.  We're assuming the rest of the data is intact and usable.
2. There are no hidden duplicates entries that could not be dropped by dropping duplicates.
3. Any entries that are dropped due to NA are worthed the same as any other entries.  We hope that we're not dropping important entries.
4. Try-Except blocks were used to help automate ETL script by not halting or producing corrupt data during ETL process.
5. Data connection through pgAdmin is functional.
