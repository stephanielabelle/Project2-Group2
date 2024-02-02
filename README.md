# Project 2 - ETL Pipline
## Group 2

This project will extract and transform crowdfunding data from excel workbooks for the creation of a PostgreSQL crowdfunding database.
Data was sourced from two excel files; [crowdfunding.xlsx](Resources/crowdfunding.xlsx) and contacts.xlsx(Resources/contacts.xlsx), located in this repository's 'Resources' folder.  
The script for data extraction and transformation is located in the [ETL_Mini_Project](ETL_Mini_Project_AAfolabi_MKhan_EMaksimova_SLaBelle.ipynb) jupyter notebook file. 

Four CSV files were exported for database construction (???new folder???):
1. category.csv
2. subcategory.csv
3. campaign.csv
4. contacts.csv

### Category and Subcategory DataFrames

### Campaign DataFrame

### Contacts DataFrame

### Crowdfunding Database
An [ERD](add link) was constructed with the [QuickDBD](https://www.quickdatabasediagrams.com/) app, and the schema was saved as a Postgres file named [crowdfunding_db_schema](crowdfunding_db_schema.sql).
The crowdfunding schema was used to construct a PostgreSQL database named [crowdfunding_db](crowdfunding_db.sql).  The 4 previously constructed csv files were successfully imported and each table can be displayed with a SELECT statement.

