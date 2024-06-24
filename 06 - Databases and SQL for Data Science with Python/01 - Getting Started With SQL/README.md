# Getting Started With SQL

### What is SQL?
SQL, or Structured Query Language, is a language used for relational Databases to query or obtain data from a database.

### What is Data?
Data is a collection of facts, in the form of numbers, words or images, and is one of the most critical aspects of business. Giving examples of banks, there are data such as name, documentary data, monetary values, etc.

### What is a Database?
It is a data repository, a place where data is stored, and has functions such as adding, modifying and searching for data.

### Relational Database
When data is stored in tabular form, the data is organized in tables like in a spreadsheet, which is columns and rows, that's relational database. The columns contain properties about the item such as LastName, FirstName, e-mail address, city. A table is a collection of related things, like a list of employees or a list of book authors. In a relational database, you can form relationships between tables.

### DBMS
DBMS, or Database Management System, is software that allows the creation, management and manipulation of databases. It provides an interface for users and applications to interact with data in an organized and efficient manner, ensuring data integrity, security, and consistency. Examples of DBMS include MySQL, PostgreSQL, Oracle Database and Microsoft SQL Server.

### RDBMS
RDBMS, or Relational Database Management System, is a specific type of DBMS that organizes data into tables related to each other using primary and foreign keys. RDBMS serves as the backbone of applications in many industries, including banking, transportation, health, and so on. Examples are: MySQL, Oracle Database, IBM DB2, etc.

### Basic SQL Commands
For the majority of people using a database, there are five simple commands:
  - Create a Table
  - Insert data to a table
  - Select data from the table
  - Update the data in the table
  - Delete data from the table


## `SELECT` Statement
The 'SELECT' Statement is used in SQL to retrieve data from a database. It allows you to specify which columns of a table should be returned.

    SELECT column1 FROM TABLE;
 
If multiple columns are selected, the columns will be returned in the order in which they were called.
    
    SELECT column1, column2, column3 FROM TABLE;

If you select all available columns in a given database, "*" will be used for this.

    SELECT * FROM TABLE;

### Filtering Results
The `SELECT` clause can be combined with other clauses, such as `WHERE`, to filter the desired results. It allows you to specify which rows should be included in the query result, based on criteria such as equality, inequality, or other comparisons. 

The basic syntax is:

    SELECT column1, column2 FROM TABLE WHERE condition;

In the example below, there will be selected all the columns from the table "CUSTUMERS" where their respective ages are above 30 years

    SELECT * FROM CUSTUMERS WHERE age > 30;

### Comparsions Criteria
Some of the comparison criteria are:
 - Equal to (`=`)
 - Not equal to (`<>`)
 - Greater than (`>`)
 - Less than (`<`)
 - Greater than or equal to (`>=`)
 - Less than or equal to (`<=`)

    
## `COUNT` Statement

## `DISTINCT` Statement

## `LIMIT` Statement

## `INSERT` Statement

## `UPDATE` Statement

## `DELETE` Statement
