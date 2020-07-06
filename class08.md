# reading 8 : SQL

SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

Select Query

To retrieve data from a SQL database, we need to write **SELECT** statements, which are often colloquially refered to as queries

Queries with constraints

If we had Too many rows, weuse **WHERE**

Filtering and sorting Query results
We use **DISTINCT**

Inserting rows

When inserting data into a database, we need to use an **INSERT** statement
```
INSERT INTO mytable
VALUES (value_or_expr, another_value_or_expr, …),
       (value_or_expr_2, another_value_or_expr_2, …),
       …;
```

Updating rows

In addition to adding new data, a common task is to update existing data, which can be done using an UPDATE statement. 

Deleting rows

To delet data we use **DELETE** with **WHERE**

Creating tables

When you have new entities and relationships to store in your database, you can create a new database table using the **CREATE TABLE** statement.

Altering tables

By using the **ALTER TABLE** statement to add, remove, or modify columns and table constraints.


Dropping tables
In some rare cases, you may want to remove an entire table including all of its data and metadata, and to do so, you can use the **DROP TABLE** statement<br>
DROP TABLE is differs fron DELETE which it removes the table schema from the database entirely.
