

# Getting Started

Create a new database on Postgress pgAdmin
Right click on the new database 
Click restore and upload the dvdrental.tar.


# Basic Operation using SQL

1. Select the every column in the customer table

SELECT * 

FROM 

customer 

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


4. Select first 100 customer first name and last name and arrange first name in descending order

SELECT 

    first_name, last_name 

FROM 

customer

LIMIT 100

ORDER BY first_name DESC

  
5. Get the title and release year for films that its rental_rate equals 4.99

SELECT 

title, release_year

FROM 

film 

WHERE rental_rate = 4.99


6. Get the title, year of release and rating of film for films with rental fee less than $4 and rating is general or Parental Guidance


SELECT title, release_year, rating 

FROM film 

WHERE rental_rate < 4 AND rating ='G' OR rating = 'PG'

  
7. Get the title, year of release and rating of film for films with rental fee less than $4 and rating is general or Parental Guidance. Also Rename the column

SELECT 

title "Movie Title", 

release_year "Year",

rating "Rating"

FROM 

film 

WHERE rental_rate < 4 AND rating ='G' OR rating = 'PG'




  
