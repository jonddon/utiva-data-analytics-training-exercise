

# Getting Started

Create a new database on Postgress pgAdmin
Right click on the new database 
Click restore and upload the dvdrental.tar.


# Basic Operation using SQL

1. Select the every column in the customer table

SELECT * FROM customer 

2. Select first 100 customer first name and last name 

  SELECT 
    first_name, last_name 
  FROM 
    customer
  LIMIT 100
  
3. Select the first 50 customer name and starting from the 21st customer

SELECT 
  first_name, last_name    
FROM 
   customer
LIMIT 50 OFFSET 20
