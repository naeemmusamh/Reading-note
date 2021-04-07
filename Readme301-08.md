# SQL

What is SQL?

SQL (Structured Query Language) is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database.

There are many popular SQL databases including SQLite, MySQL, Postgres, Oracle and Microsoft SQL Server.

Relational databases

Before learning the SQL syntax, it's important to have a model for what a relational database actually is. A relational database represents a collection of related tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns and any number of rows of data.

|Id|Make/Model|# Wheels|# Doors|Type|
|--|----------|--------|-------|----|
|1|Ford Focus|4|4|Sedan|
|2|Tesla Roadster|4|2|Sports|
|3|Kawakasi Ninja|2|0|Motorcycle|
|4|McLaren Formula 1|4|0|Race|
|5|Tesla S|4|4|Sedan|

Since most users will be learning SQL to interact with an existing database, the lessons begin by introducing you to the various parts of an SQL query. The later lessons will then show you how to alter a table and create new tables from scratch.

# SQL Lesson 1: SELECT queries 101

To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially refered to as queries. A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned. It has a specific syntax though, which is what we are going to learn in the following exercises.

Select query for a specific columns
SELECT column, another_column, …
FROM mytable;

Select query for all columns
SELECT * 
FROM mytable;

Exercise

We will be using a database with data about some of Pixar's classic movies for most of our exercises. This first exercise will only involve the Movies table, and the default query below currently shows all the properties of each movie. To continue onto the next lesson, alter the query to find the exact information we need for each task.

# SQL Lesson 2: Queries with constraints (Pt. 1)

Now we know how to select for specific columns of data from a table, but if you had a table with a hundred million rows of data, reading through all the rows would be inefficient and perhaps even impossible.

In order to filter certain results from being returned, we need to use a WHERE clause in the query. The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not.

Select query with constraints
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;

More complex clauses can be constructed by joining numerous AND or OR logical keywords (ie. num_wheels >= 4 AND doors <= 2). And below are some useful operators that you can use for numerical data

# SQL Lesson 3: Queries with constraints (Pt. 2)

When writing WHERE clauses with columns containing text data, SQL supports a number of useful operators to do things like case-insensitive string comparison and wildcard pattern matching. We show a few common text-data specific operators

Select query with constraints
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;

    