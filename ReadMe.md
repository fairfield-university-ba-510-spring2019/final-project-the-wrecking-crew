# Charles F. Dolan School of Business

# BA 510 – Databases, SP 2019

__Final Project__

Stuart Weinstein

Thomas Moroski

Sean Bernard

## Process


- We designed a normalized to BCNF a relational database that can contains all of the CSV data in our SourceData repository. 
    - ERD Design: **[CourseDataERD.PDF](Docs/CourseDataERD.PDF)** and **[CourseDataDictionary.md](Docs/CourseDataDictionary.md)**
- We created a SQLite database called CourseData.db and populated the database with data from the CSV files from our SourceData repository. 
    - CSV files were imported within the notebook 
    - We imported the CSV file data into tables with the prefix `import_` to indicate that the table contains raw source data.  Then we dropped the CSV files upon completion of CourseData.db from the terminal. 
    - We used SQL to create and populate the tables from our **[CourseDataERD.PDF](Docs/CourseDataERD.PDF)**. 
    - Capture all of your SQL DDL and DML code in a new notebook called `CourseDataETL.ipynb` in this project folder. Use Markdown to annotate your work as you go along. Also, make sure you can re-run your code from scratch to rebuild the database when needed.
- We tested the integrity of our `CourseData.db` database. Queries can be found in **[CourseDataTests.ipynb](Docs/CourseDataTests.ipynb)** notebook
- Write queries to ensure that  ...
    - Each column has a sensible data type (Domain integrity); are there truncation or translation errors?   
    - Each row describes a unique entity (Entity integrity); just having a PK is not enough: you will need to look for duplicate a data records
    - Each relationship is implemented correctly (Relational integrity); are the FKs JOIN-compatible with the PKs? does each mandatory relationship have a corresponding NOT NULL constraint?
- Annotate your queries in Markdown so we know what you are testing and why.

