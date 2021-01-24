# Intro to ERDs

## Database Schema:
1.) *Do some research on what a Database Schema is: 

- **What is a schema?** 
- A database schema is the "skeleton" structure that represents the logical view of the entire database. It defines how data is organized and how the relations among them are associated, along with formulating all constraints that are applied on the data. It is designed when the database doesn't exist at all. Once the database is operational, it is very difficult to apply changes, a database schema does not contain any data or information. 
- **Why do we use them?**
- Primarily to handle organization and structure of the database, as well as establish permissions throughout. 
- **What do they look like?**
- Schemas contain objects such as: tables, columns, data types, views, stored procedures, relationships, primary keys, foreign keys. etc. 
- **Source**: https://www.tutorialspoint.com/dbms/dbms_data_schemas.htm 

2.) *What are the different types of Database keys?*

- **What is a Primary Key?**: 
- The most important key in the database, there can only be one primary key in a table. It will NOT accept duplicate or null values. Contains unique values (EX: Select * from Employee where employee_Id is 203)
- **What is a Foreign key?**:
- This can be a common key in two database tables. Using a foreign key, we can identify records from multiple tables. It accepts duplicate and null values. Also helps reduce data redundancy.
- **What is a Composite key?**: 
- A composite key is composed of two or more attributes that collectively uniquely identify each record. A combination of two keys. 
- **How are they different? When do you use 1 over the others?**:
- Foreign keys are used to tie together two tables, a primary key is the standard across the board for most tables, sort of like an index, it should really be used for standard tables that need a simple, exact unique identifier. Composite keys are really to be used when two pieces of information are needed to uniquely identify items.
- Source: https://www.csestack.org/different-types-database-keys-example/ 
- Source: https://www.techopedia.com/7/32101/storage/what-is-the-difference-between-a-composite-key-primary-key-and-foreign-key 

3.) *What are relationships in a relational database?*
- **What is a 1:1 relationship?**:
- A relationship where one row of a table is linked to ONLY one row in another table, vice versa. It is created by using a Primary key and Unique foreign key relationship.
- **What is a Many:Many relationship?**:
- It is a relationship where a parent row in one table contains several child rows in a second table, and vice versa. 
- **How about a 1:Many or a Many:1?**:
- These both are relationships between two seperate tables where a row from one table can have several matching rows in another table. It is created by using a Primary Key and Foreign key relationship.
- Source: https://www.tech-recipes.com/rx/56738/one-to-one-one-to-many-table-relationships-in-sql-server/ 
- Source: https://condor.depaul.edu/gandrus/240IT/accesspages/relationships.htm 


