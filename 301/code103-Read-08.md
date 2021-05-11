# SQL
### What is SQL?
Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

### Relational databases:
represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns and any number of rows of data.

### SQL command:
* To retrieve data from a SQL database : write **SELECT** statements.
* To filter certain results from being returned: use a **WHERE** clause in the query.
    * SQL operators:

    ![operator1](https://mk0softwaretest02r6g.kinstacdn.com/wp-content/uploads/2017/04/sql-comparison-operators.png)

    ![operator2](https://mk0softwaretest02r6g.kinstacdn.com/wp-content/uploads/2017/04/sql-logical-operators.png)

* To remove duplicate rows : use **DISTINCT** keyword
* To sort the column in an ascending or descending manner : use **ORDER BY** clause.
* To reduce the number of rows to return: use **LIMIT** clause.
* To specify where to begin counting the number rows from: use **OFFSET** clause.

### Inserting rows
***Schema***: what describes the structure of each table, and the datatypes that each column of the table can contain.

- When inserting data into a database, we need to use an **INSERT statement**, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert. 
- To update existing data: use **UPDATE** statement. 
- To delete data from a table in the database: use a **DELETE** statement.


### CREATE TABLE:
use the **CREATE** TABLE statement. 
The structure of the new table is defined by its table schema, which defines a series of columns. Each column has a name, the type of data allowed in that column, an optional table constraint on values being inserted, and an optional default value.

- To update your corresponding tables and database schemas: **ALTER TABLE** statement.
- To delete an entire table: use the **DROP TABLE** statement.

