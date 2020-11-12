# SQL

- ### Lesson 1:
- To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially refered to as queries. A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned
- Think of a table in SQL as a type of an entity, each row in that table is a specific instance of that type. This means that the columns would then represent the common properties shared by all instances of that entity.
- Given a table of data, the most basic query we could write would be one that selects for a couple columns (properties) of the table with all the rows (instances) *ex: SELECT column, another_column, ... FROM mytable;*
- The result of this query will be a two-dimensional set of rows and columns, effectively a copy of the table but only with the columns we requested. If you wanted to retrieve absolutely all the columns of data from a table, we use (*) shorthand instead of listing individually. *ex: Select * FROM mytable;* this is a simple way to inspect a table by dumping all the data at once.
### Lesson 2:
- When dealing with tables with millions of rows of data, reading through all the rows would be inefficient and probably impossible. This is where we filter certain results from being returned, by using *WHERE* clause in the query. The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not.
- *EX: SELECT column, another_column, ...
- FROM mytable
- WHERE condition
- AND/OR another_condition
- AND/OR ...;
- More complex clauses can be constructed together by joining numerous *AND* or *OR* logical keywords. 
- **Useful Operators**:
- *Operator*: =, !=, < <=, >, >=	*Condition*: Standard numerical operators	*Ex:* col_name != 4
- *Operator*: BETWEEN … AND …	*Condition*: Number is within range of two values (inclusive)	*Ex:* col_name BETWEEN 1.5 AND 10.5
- *Operator*: NOT BETWEEN ... AND ... *Condition*: Number is not within range of two values (inclusive) *Ex:* col_name NOT BETWEEN 1 AND 10
- *Operator*: IN (...) *Condition*: number exists in a list *Ex:* col_name IN (2, 4, 6)
- *Operator*: NOT IN (...) *Condition*: Number does not exist in a list *Ex:* col_name NOT IN (1, 3, 5)
- In addition to making results more manageable to understand writing clauses to constrain the set of rows returned also allows the query to run faster due to the reduction of unnecessary data being returned.
### Lesson #3:
- *Operator*: =	 *Condition*: Case sensitive exact string comparison (notice the single equals)	*Ex:* col_name = "abc"
- *Operator*: != or <>	*Condition*: Case sensitive exact string inequality comparison	*Ex:* col_name != "abcd"
- *Operator*: LIKE	*Condition*: Case insensitive exact string comparison	*Ex:* col_name LIKE "ABC"
- *Operator*: NOT LIKE	*Condition*: Case insensitive exact string inequality comparison	*Ex:* col_name NOT LIKE "ABCD"
- *Operator*: %	*Condition*: Used anywhere in a string to match a sequence of zero or more characters (only with LIKE or NOT LIKE)	*Ex:* col_name LIKE "%AT%" (matches "AT", "ATTIC", "CAT" or even "BATS")
- *Operator*: _	*Condition*: Used anywhere in a string to match a single character (only with LIKE or NOT LIKE)	*Ex:* col_name LIKE "AN_" (matches "AND", but not "AN")
- *Operator*: IN (…)	*Condition*: String exists in a list	*Ex:* col_name IN ("A", "B", "C")
- *Operator*: NOT IN (…)	*Condition*: String does not exist in a list	*Ex:* col_name NOT IN ("D", "E", "F")
### Lesson 4: Filtering and sorting Query Results:
- Even though the data in a database may be unique, the results of any particular query may not be.Take our Movies table for example, many different movies can be released the same year. In such cases, SQL provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword.
- Ex: SELECT DISTINCT column, another_column, …
- FROM mytable
- WHERE condition(s);
- **ORDER BY** provides a way to sort your results by a given column in ascending or descending order using this clause.
- EX: SELECT column, another_column, …
- FROM mytable
- WHERE condition(s)
- ORDER BY column ASC/DESC;
- When an **ORDER BY** clause is specified, each row is sorted alpha-numerically based on the specified column's value.
- Another clause which is commonly used with the **ORDER BY** clause are the **LIMIT** and **OFFSET** clauses, which are a useful optimization to indicate to the database the subset of the results you care about.
- **LIMIT** will reduce the number of rows to return 
- **OFFSET** while optional, will specify where to begin counting the number rows from.
- EX: SELECT column, another_column, …
- FROM mytable
- WHERE condition(s)
- ORDER BY column ASC/DESC
- LIMIT num_limit OFFSET num_offset;
### Lesson 13: Inserting Rows
- **Database schema** describes the structure of each table and the datatypes that each column of the table can contain. 
- **INSERT** inserts data into a database, which declares which table to write into, the columns of data that we are filling and one or more rows of data to insert. 
- EX: INSERT INTO mytable
- VALUES (value_or_expr, another_value_or_expr, …),
-(value_or_expr_2, another_value_or_expr_2, …),
- …;
### Lesson 14: Updating Rows
- In addition to adding new data, a common task is to update existing data, which can be done using an **UPDATE** statement. Similar to the **INSERT** statement, you have to specify exactly which table, columns, and rows to update.
- EX: UPDATE mytable
- SET column = value_or_expr, 
- other_column = another_value_or_expr, 
- …
- WHERE condition;
- The statement works by taking multiple column/value pairs, and applying those changes to each and every row that satisfies the constraint in the WHERE clause.
### Lesson 15: Deleting Rows
- Use **DELETE** statement to delete data from a table and the rows on the table that needed to be deleted in the **WHERE** clause.
- EX: DELETE FROM mytable
- WHERE condition;
- If you leave out the WHERE constraint, ALL rows are removed.
### Lesson 16: Creating Tables
- When you have new entities and relationships to store in your database, you can create a new database table using the CREATE TABLE statement.
- Ex: CREATE TABLE IF NOT EXISTS mytable (
- column DataType TableConstraint DEFAULT default_value,
- another_column DataType TableConstraint DEFAULT default_value,
- …
- );
- The structure of the new table is defined by its table schema, which defines a series of columns. Each column has a name, the type of data allowed in that column, an optional table constraint on values being inserted, and an optional default value.
### Lesson 17: Altering Tables
- As your data changes over time, SQL provides a way for you to update your corresponding tables and database schemas by using the ALTER TABLE statement to add, remove, or modify columns and table constraints.
- The syntax for adding a new column is similar to the syntax when creating new rows in the CREATE TABLE statement. You need to specify the data type of the column along with any potential table constraints and default values to be applied to both existing and new rows. In some databases like MySQL, you can even specify where to insert the new column using the FIRST or AFTER clauses, though this is not a standard feature.
- *EX: ALTER TABLE mytable
- ADD column DataType OptionalTableConstraint 
- DEFAULT default_value;*
### Lesson 18: Dropping Tables
- In some rare cases, you may want to remove an entire table including all of its data and metadata, and to do so, you can use the DROP TABLE statement, which differs from the DELETE statement in that it also removes the table schema from the database entirely.
- *Ex: DROP TABLE IF EXISTS mytable;*


