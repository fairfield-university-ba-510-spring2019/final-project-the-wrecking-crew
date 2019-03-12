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
    - CSV files were imported using the SQLite3 tool
    - We imported the CSV file data into tables with the prefix `import_` to indicate that the table contains raw source data.  Then we dropped the CSV files upon completion of CourseData.db from the terminal. 
    - We used SQL to create and populate the tables from our **[CourseDataERD.PDF](Docs/CourseDataERD.PDF)**. 
    - We captured all of our SQL DDL and DML code in a new notebook called **[CourseDataETL.ipynb](Docs/CourseDataETL.ipynb)** 
- We tested the integrity of our `CourseData.db` database. Queries can be found in **[CourseDataTests.ipynb](Docs/CourseDataTests.ipynb)** notebook
- Write queries to ensure that  ...
    - Each column has a sensible data type (Domain integrity); are there truncation or translation errors?   
    - Each row describes a unique entity (Entity integrity); just having a PK is not enough: you will need to look for duplicate a data records
    - Each relationship is implemented correctly (Relational integrity); are the FKs JOIN-compatible with the PKs? does each mandatory relationship have a corresponding NOT NULL constraint?
    - Annotate your queries in Markdown so we know what you are testing and why.
        - We designed and built a data warehouse called `CourseDataWarehouse.db`based on a star schema design. 
        - Each fact table (and associated dimensions) can be seen on the ERD named **[COURSEFACTS_TableERD.pdf](Docs/COURSEFACTS_TableERD)** 
- We tested our `CourseDataWarehouse.db` for data integrity.  Queries can be found in **[CourseDataWarehouseTest.ipynb](Docs/CourseDataWarehouseTest.ipynb)** notebook 
- Demo your results with useful queries.
    - Create yet another new notebook called **[CourseDataWarehouseDemo.ipynb](Docs/CourseDataWarehouseDemo.jpynb)** that illustrates the usefulness of the data warehouse with a few informative queries.
        - Number the queries so we can refer to them by number later. (In other words, make sure your queries have entity integrity.)
        - In your Markdown include remarks about why, when, and how the query might be used in practice. If your query results suggest anything insightful, then include a cell below the query results with Markdown-formatted remarks.
- Walkthrough presentation
