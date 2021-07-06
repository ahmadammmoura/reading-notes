# What is MySQL?

![img](https://miro.medium.com/max/1400/1*TTM5AleQfFJ-mItttJROdg.jpeg)

##### MySQL is a relational database management system developed by the Swedish company MySQL AB and is an Oracle product.

##### MySQL is a relational database management system. Relational databases store data in different tables instead of putting all data in a large warehouse, which results in an increase of speed and flexibility.

##### The SQL language used by MySQL is the most commonly used standardized language for accessing databases. MySQL software adopts a dual authorization policy, divided into community version and commercial version. Small and medium-sized website development choose MySQL as the website database of choice, due to its small size, high speed, low total cost of ownership, and characteristics of open source,


### Database & Table Creation

##### A MySQL server can have multiple databases and each database can have multiple tables. Type the following the printout the existing databases.
`show databases;`

![img](https://miro.medium.com/max/673/1*NYVIa33kNJJbtPojRorjCw.png)

##### We can see there are four databases by default. Now we will see how to create a new database.

`CREATE DATABASE new;`

![img](https://miro.medium.com/max/640/1*hBiGeqxSUkbO_wTSGabbVg.png)

##### We can see the ‘new’ database has been successfully created.
* In order to work in a database, we have to type in USE <database_name>;, where ‘database_name’ is the name of the database we intend to work on. Let’s create a table by the following syntax.
* CREATE TABLE <table_name> ( column1 datatype, column2 datatype2, ....);

##### Let’s create a table name ‘first_table’ with five columns — ‘id’, ‘movie’, ‘director’, ‘genre’ as follows.

![img](https://miro.medium.com/max/675/1*eY7OLpw0jFHdeALvak9gCw.png)

##### Here the first column is an integer datatype and by ‘NOT NULL’ means the values in the column should not be a null value, that a value should be present in the column for all rows of the table. Second column’s datatype is VARCHAR(), that it is a string data type with the length inside the parenthesis. The last one ‘PRIMARY KEY’ is not a column but it determines which of all columns should be a primary key, that each row for that column should be unique. One table should contain only one primary. Here ‘id’ is the primary key.