# SQL

# Introduction to SQL with Postgres :

Write the SQL commands necessary to do the following:

1. Create a database called first_assignment

- create database first_assignment;

2.  Connect to that database

- \c ;

3. Create a table called products with columns for:

- id, which should be a unique auto-incremementing integer
- name, which should be text, and not nullable
- price, which should be a floating point number, and greater than zero
- can_be_returned, which should be a boolean, and not nullable

```
CREATE TABLE products (

 ID int,
 name TEXT ,
 price REAL CHECK (price > 0) ,
 can_be_returned BOOLEAN
)
```

4. Add a product to the table with the name of "chair", price of 44.00, and can_be_returned of false.
