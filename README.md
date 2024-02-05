# Project 2 - ETL Pipline
## Group 2

This project will extract and transform crowdfunding data from excel workbooks for the creation of a PostgreSQL crowdfunding database.
Data was sourced from two excel files; [crowdfunding.xlsx](Resources/crowdfunding.xlsx) and [contacts.xlsx](Resources/contacts.xlsx), located in this repository's 'Resources' folder.  
The script for data extraction and transformation is located in the [ETL_Mini_Project](ETL_Mini_Project_AAfolabi_MKhan_EMaksimova_SLaBelle.ipynb) jupyter notebook file. 

### Extraction and Transformation:

Four CSV files were exported for database construction:
1. [category.csv](Resources/category.csv)
2. [subcategory.csv](Resources/subcategory.csv)
3. [campaign.csv](Resources/campaign.csv)
4. [contacts.csv](Resources/contacts.csv)
   
#### Category and Subcategory DataFrames
The category.csv file was contructed from the "category & sub-category" column in the crowdfunding.xlsx file.  Categories were extracted and given a unique ID designated as "category_ID".  
The subcategory.csv file was contructed from the "category & sub-category" column in the crowdfunding.xlsx file.  Subcategories were extracted and given a unique ID designated as "subcategory_ID".  

#### Campaign DataFrame
The campaign.csv file was constructed from the crowdfuncing.xlsx file and utilized the category.csv and subcategory.csv files for populating category and subcategory IDs.  

#### Contacts DataFrame
The contacts.csv file was extracted and transformed from the contacts.xlsx file.  

### Loading to Crowdfunding Database:

An [ERD](Resources/ERD) was constructed with the [QuickDBD](https://www.quickdatabasediagrams.com/) app, and the schema was saved as a Postgres file named [crowdfunding_db_schema](crowdfunding_db_schema.sql).
The crowdfunding schema was used to construct a PostgreSQL database named [crowdfunding_db](crowdfunding_db.sql).  The 4 previously constructed csv files were successfully imported and each table can be displayed with a SELECT statement.

