# Introduction to Relational Databases and Tables

## Relational Database Concepts

## SQL Statements (DDL x DML)

## `CREATE` Statement
The `CREATE` command in SQL is used to create new tables, indexes, views or other objects in the database.

The basic syntax for creating a table is:

    CREATE TABLE table (column1 type, column2 type, ...);

The example below creates a new table called "customers" with columns for "id", "name" and "age".

    CREATE TABLE customers (id INT, name VARCHAR(100), age INT);


## `ALTER` Statement
The `ALTER` command in SQL is used to modify the structure of an existing table in the database. It allows you to add, delete or modify columns, in addition to changing other table attributes.

The example below adds a new column called "email" to the "customers" table. 

    ALTER TABLE customers ADD email VARCHAR(100);
    
Another example is 

    ALTER TABLE customers DROP COLUMN age;

Which removes the "age" column from the "customers" table.

## `DROP` Statement

The `DROP` command in SQL is used to completely delete a table or a database from the database management system (DBMS). When used, it removes the structure and stored data, making the action irreversible.

Its syntax is:

    DROP TABLE table;

The example below will delete the "customers" table and all its data.

    DROP TABLE customers;

In the same way,

    DROP DATABASE my_bank;

will delete the database "my_bank" and all its contents.


## `TRUNCATE` Statement
The `TRUNCATE` command in SQL is used to remove all records from a table but leaves the table structure intact. Unlike the DELETE command, TRUNCATE does not allow the specification of conditions and is generally faster, as it does not record each removal individually.

The basic syntax is:

TRUNCATE TABLE table;

The example below will erase all data from the "customers" table efficiently.

TRUNCATE TABLE customers;
