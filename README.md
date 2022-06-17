# SELECT Practice

## Setup

You should have created a Google Cloud account, created a project, created and instance, created a database in that instance called 'admin', installed MySQL Workbench and made a connection to that database. In this lesson we will practice querying data.

Start by opening MySQL Workbench

## Part 1 - Initialize data

In this repo you'll see another file called `initialize.sql`. This file contains SQL scripts to create a table called users and populate it with data. Follow these instructions to run the script in MySQL Workbench so that you populate data in your GoogleCloud Database!!

* In MySQL Workbench, make sure you've selected the "admin" database as your default schema (as per the name of the DB you created following the textbook.)

* Create a new query tab
  * Click the button on the top left that has a SQL file with a "plus" icon on it

* Click the folder icon in your query tab to open a new file

* Search for "311_wk3_day1_db_select" in your file explorer/finder window and select the "initialize.sql" script that lives in this repo

* When you do you'll see the scripts from this 'initialize.sql' file populate in your MySQL Workbench!!!!

* Click the lightning bolt icon to run the query

* If you get an error: `1046: Error Code: 1046. No database selected Select the default DB to be used by double-clicking its name in the SCHEMAS list in the sidebar.` Select your 'admin' schema as your default so MySQL workbench knows what connection to use.

* If you refresh your schemas you should see a "users" table

## Part 2 - Query data

We are going to run a couple SQL queries. As you do, copy/paste the query as the answers to the following questions.

Also, put the answers in the "Query Responses" section of this README.

> *NOTE: The query instructions are intentionally written in plain english. It's up to you to translate that into a SELECT statement.*

1. Select all fields from users where the city equals Chicago

2. Select the "state" field for users with a first name of "Glory"

3. Select all fields from users whose phone1 starts with "773"

## Query Responses

1.
  * How many rows were returned: 7
  * First name of the first user: Mitsue

2.
  * How many rows were returned: 2
  * What states do they live in: MD, TX

3.
  * How many rows were returned: 6
  * What's the last email on the list: nichelle_meteer@meteer.com

## Summary

Think about how this data is laid out. Feel free to look in the `initialize.sql` file to see the raw data.

* Do you think it would be easier or harder to search through this data manually or using SQL?
* What about when the dataset gets larger?
