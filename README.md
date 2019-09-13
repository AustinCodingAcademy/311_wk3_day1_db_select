# SELECT Practice

## Setup

You should have created a Google Cloud account, installed MySQL Workbench and made a connection to your database. In this lesson we will practice querying data.

* Open MySQL Workbench

## Part 1 - Initialize data

* Make sure you've selected the "admin" database

* Create a new query tab
  * Click the button on the top left that has a SQL file with a "plus" icon on it

* Click the folder icon in your query tab to open a new file

* Select the "initialize.sql" script that lives in this repo

* Click the lightning bolt icon to run the query

* If you refresh your schemas you should see a "users" table

## Part 2 - Query data

We are going to run a couple SQL queries and put the answers in the "Query Responses" section of this README. The query instructions are intentionally written in plain english. It's up to you to translate that in a SELECT statement.

1. Select all fields from users where the city equals Chicago
<!-- answer -->
'7', 'Mitsue', 'Tollner', 'Morlong Associates', '7 Eads St', 'Chicago', 'Cook', 'IL', '60632', '773-573-6914', '773-924-8565', 'mitsue_tollner@yahoo.com', 'http://www.morlongassociates.com'
'79', 'Viva', 'Toelkes', 'Mark Iv Press Ltd', '4284 Dorigo Ln', 'Chicago', 'Cook', 'IL', '60647', '773-446-5569', '773-352-3437', 'viva.toelkes@gmail.com', 'http://www.markivpressltd.com'
'137', 'Marti', 'Maybury', 'Eldridge, Kristin K Esq', '4 Warehouse Point Rd #7', 'Chicago', 'Cook', 'IL', '60638', '773-775-4522', '773-539-1058', 'marti.maybury@yahoo.com', 'http://www.eldridgekristinkesq.com'
'140', 'Valentin', 'Klimek', 'Schmid, Gayanne K Esq', '137 Pioneer Way', 'Chicago', 'Cook', 'IL', '60604', '312-303-5453', '312-512-2338', 'vklimek@klimek.org', 'http://www.schmidgayannekesq.com'
'182', 'Carmela', 'Cookey', 'Royal Pontiac Olds Inc', '9 Murfreesboro Rd', 'Chicago', 'Cook', 'IL', '60623', '773-494-4195', '773-297-9391', 'ccookey@cookey.org', 'http://www.royalpontiacoldsinc.com'
'381', 'Erick', 'Nievas', 'Soward, Anne Esq', '45 E Acacia Ct', 'Chicago', 'Cook', 'IL', '60624', '773-704-9903', '773-359-6109', 'erick_nievas@aol.com', 'http://www.sowardanneesq.com'
'414', 'Nichelle', 'Meteer', 'Print Doctor', '72 Beechwood Ter', 'Chicago', 'Cook', 'IL', '60657', '773-225-9985', '773-857-2231', 'nichelle_meteer@meteer.com', 'http://www.printdoctor.com'



2. Select the "state" field for users with a first name of "Glory"
<!-- answer -->
MD, TX

3. Select all fields from users who's phone1 starts with "773"
<!-- answer -->
6

## Query Responses

1.
  * How many rows were returned:
  * First name of the first user:
  <!-- answer -->
1 rows,
"james Butt"

2.
  * How many rows were returned:
  * What states do they live in:
<!-- answer -->
 rows,
32
3.
  * How many rows were returned:
  * What's the last email on the list:
<!-- answer -->
'zona@hotmail.com'

  ## Summary

  Think about how this data is laid out. Feel free to look in the initialize.sql file to see the raw data. Do you think it would be easier or harder to search through this data manually or using SQL? What about when the dataset gets larger?