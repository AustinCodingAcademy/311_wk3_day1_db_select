# SELECT Practice

## Setup

You should have created a Google Cloud account, installed MySQL Workbench and made a connection to your database. In this lesson we will practice querying data.

- Open MySQL Workbench

## Part 1 - Initialize data

- Make sure you've selected the "admin" database

- Create a new query tab

  - Click the button on the top left that has a SQL file with a "plus" icon on it

- Click the folder icon in your query tab to open a new file

- Select the "initialize.sql" script that lives in this repo

- Click the lightning bolt icon to run the query

- If you refresh your schemas you should see a "users" table

## Part 2 - Query data

We are going to run a couple SQL queries and put the answers in the "Query Responses" section of this README. The query instructions are intentionally written in plain english. It's up to you to translate that in a SELECT statement.

1. Select all fields from users where the city equals Chicago

2. Select the "state" field for users with a first name of "Glory"

3. Select all fields from users who's phone1 starts with "773"

## Query Responses

1.

- How many rows were returned: 7 rows
- First name of the first user: Mitsue

- Query:

- Query: select count(\*) from users where city = 'chicago'
- Query: select \* from users where city = 'chicago'
- Query: select first_name from users where city = 'chicago' order by id ASC limit 1; (yes, I know I didn't need to do this. I couldn't let it go)

2.

- How many rows were returned: 7
- What states do they live in: MD, TX

- Query: select state from users where first_name = 'glory'

3.

- How many rows were returned: 6
- What's the last email on the list: nichelle_meteer@meteer.com

-Query: select count(\*) from users where phone1 like "773%"
-Query: select email from users where phone1 like "773%" ORDER BY id DESC LIMIT 1; (and another moment)

## Summary

Think about how this data is laid out. Feel free to look in the initialize.sql file to see the raw data. Do you think it would be easier or harder to search through this data manually or using SQL? What about when the dataset gets larger?

//
