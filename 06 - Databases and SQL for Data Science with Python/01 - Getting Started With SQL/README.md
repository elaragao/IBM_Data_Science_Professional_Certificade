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

In the example below, there will be selected all the columns from the table "CUSTOMERS" where their respective ages are above 30 years.

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
The `COUNT` function in SQL is used to return the number of rows that match a specific criteria. It is often used to count how many entries there are in a table or how many entries meet a certain condition.

The basic syntax is:

    SELECT COUNT(column) FROM table;

In the example below, will be returned the number of customers from the table "CUSTOMERS" where their respective ages are above 30 years.

    SELECT COUNT(*) FROM customers WHERE age > 30;
    

## `DISTINCT` Statement
The `DISTINCT` clause in SQL is used to remove duplicates from a result set. It only returns distinct (different) values ​​in the query.

The basic syntax is:

    SELECT DISTINCT column FROM table;

For example, it returns a list of unique cities present in the customer table, without repetitions.

    SELECT DISTINCT city FROM customers;

    
## `LIMIT` Statement
The `LIMIT` clause in SQL is used to specify the maximum number of records that the query should return. This is useful when you only want to get a portion of the result set.

The basic syntax is:

    SELECT column FROM table LIMIT number;

The example below it only returns the first 10 records from the customers table.

    SELECT * FROM customers LIMIT 10;

    
## `INSERT` Statement
The `INSERT` command in SQL is used to add new records to a table in a database.

The basic syntax is:

    INSERT INTO table (column1, column2, ...) VALUES (value1, value2, ...);

For example, add a new record to the customer table with the name "John" and age 30.

    INSERT INTO customers (name, age) VALUES ('John', 30);


## `UPDATE` Statement
The `UPDATE` command in SQL is used to modify existing records in a database table.

The basic syntax is:

    UPDATE table SET column1 = value1, column2 = value2, ... WHERE condition;

The example below updates the age to 31 in the record where the name is "John". The WHERE clause is crucial for specifying which records should be updated; otherwise, all rows in the table will be modified.

    UPDATE clients SET age = 31 WHERE name = 'John';


## `DELETE` Statement
The `DELETE` command in SQL is used to remove records from a database table.

The basic syntax is:

    DELETE FROM table WHERE condition;

The example below removes all records where the age is less than 18. The WHERE clause is essential to specify which records should be deleted; without it, all records in the table will be removed.

    DELETE FROM customers WHERE age < 18;
