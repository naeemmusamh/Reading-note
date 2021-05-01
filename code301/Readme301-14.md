# DATABASE NORMALIZATION

Database normalization is a process used to organize a database into tables and columns, and that a table should be about a specific topic and that only those columns which support that topic are included.

limiting a table to one purpose:

1. you reduce the number of duplicate data that is contained within your database.

2. helps eliminate some issues stemming from database modifications.

# Normalization Stages

The stages of organization are called normal forms

First Normal Form 1NF:

Data is stored in tables with rows uniquely identified by a primary key

Data within each table is stored in individual columns in its most reduced form.

There are no repeating groups

Second Normal Form 2NF:

Only data that relates to a table’s primary key is stored in each table

Third Normal Form 3NF:

There are no in-table dependencies between the columns in each table