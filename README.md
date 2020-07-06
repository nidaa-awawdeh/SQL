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

`INSERT INTO products (name, price, can_be_returned) VALUES ('chair',44.00,false);`

5. Add a product to the table with the name of "stool", price of 25.99, and can_be_returned of true.

`INSERT INTO products (name, price, can_be_returned) VALUES ('stool',25.99,true);`

6. Add a product to the table with the name of "table", price of 124.00, and can_be_returned of false.

`INSERT INTO products (name, price, can_be_returned) VALUES ('table',124.00,false);`

7. Display all of the rows and columns in the table.
 `\d+  products`

8. Display all of the names of the products.
 `SELECT name FROM  products ;`
 
9. Display all of the names and prices of the products.
`SELECT (name , price)  FROM  products  ;`

10. Add a new product - make up whatever you would like!
`INSERT INTO products (name, price, can_be_returned) VALUES ('make up',25.99,true);`

11. Display only the products that can_be_returned.

 `SELECT * FROM products WHERE can_be_returned IN (true) ;`

 12. Display only the products that have a price less than 44.00

`SELECT * FROM  products WHERE  price < 44.00 ;`

13. Display only the products that have a price in between 22.50 and 99.99
`SELECT * FROM  products WHERE  price > 22.50  AND   price < 99.99 ;`


<hr>
<h3> Part 2 - Codewars </h3>

 - 1code.png
 - 2code.png 
