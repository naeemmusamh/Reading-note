# Data Modeling

## SQL AND NoSQL

SQL = Structure Query Language that language allow us to write Database.

1. can execute queries against a database
2. can retrieve data from a database
3. can insert records in a database
4. can update records in a database
5. can delete records from a database
6. can create new databases
7. can create new tables in a database
8. can create stored procedures in a database
9. can create views in a database
10. can set permissions on tables, procedures, and views

EX:
SELECT id, name, price FROM products;

SELECT = Method that used to select some keyword from the table you are create.

id, name, price = parameters that you write it in the table you create in the Database.

FROM = Method that used to select the specific table from the Database

products = parameters that you write for the name of the table.

|method|used|
|-----|----|
|SELECT|to select specific parameters|
|CREATE|to create new rows in the table|
|UPDATE|to update specific parameters|
|DELETE|to update specific parameters|
|||

## relation between the table in the schema
1. one to one : when store one id to the user with specific id for product

![one to many](https://i1.wp.com/coding-examples.com/wp-content/uploads/2019/09/One-To-Many-Relation.png?fit=481%2C211&ssl=1)

2. one to many : when store many product id to the user with specific user

![many to one](https://docs.magento.com/mbi/images/one-to-many_001.png)

3. many to many : when store many user for many product

![many to many](https://www.relationaldbdesign.com/database-design/module6/images/composite.gif)

# SQL VS NoSQL

|SQL|NoSQL|
|----|----|
|called as Relational Databases (RDBMS)|non-relational|
|table based databases|document based, key-value pairs|
|predefined schema|dynamic schema for unstructured data|
|vertically scalable|horizontally scalable|
|scaled by increasing the horse-power of the hardware| scaled by increasing the databases servers in the pool of resources to reduce the load|
|for defining and manipulating the data|focused on collection of documents|
|||

## types of SQL

1. MySql
2. Oracle
3. Sqlite
4. Postgres 
5. MS-SQL

## TYPES OF NoSQL

1. MongoDB
2. BigTable
3. Redis
4. RavenDb
5. Cassandra