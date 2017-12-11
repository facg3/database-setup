# database-setup

A build script is collection of ``` SQL commands ``` separated by semi-colons - in some database systems - that creates or adds table within your database.

## Some of the most important SQL commands
| Command | Description |
| :---: | :---: |
| AND | an operator that combines two conditions. Both conditions must be true for the row to be included in the result set |
| OR | an operator that combines two conditions. One of them must be true for the row to be included in the result set |
| AS | keyword in SQL that allows you to rename a column or table using an alias |
| AVG | an aggregate function that returns the average value for a numeric column |
| SUM | is a function that takes the name of a column as an argument and returns the sum of all the values in that column |
| BETWEEN | is used to filter the result set within a certain range. The values can be numbers, text or dates |
| UPDATE | statements allow you to edit rows in a table |
| WHERE | is a clause that indicates you want to filter the result set to include only rows where the following condition is true |
| SELECT | statements are used to fetch data from a database. Every query will begin with SELECT|
| ORDER BY | is a clause that indicates you want to sort the result set by a particular column either alphabetically or numerically |
| LIMIT | is a clause that lets you specify the maximum number of rows the result set will have | 
## what is database migration?
 Just like you use Git to manage changes in your source code, you can use migrations to keep track of changes to database. With migrations you can transfer your existing database into another state: Those state transitions are saved in migration files, which describe the way how to get to the new state and how to revert the changes in order to get back to the old state.
there are at least three (3!) things people mean when they talk about database migrations:
### 1.Schema Migrations
Upgrading (or potentially rolling back) an application and database schema version for each new version of app deployed.
### 2.Server Migrations
Moving your database from 1 server to another
### 3.Version Migration
Upgrading from one major version of PostgreSQL to another
### 4.DBMS Migration
Switching from MySQL or Oracle to PostgreSQL
…
## Creating Migration
```js
$ npm install db-migrate
```
## Running Migrations
```js
$ node node_modules/db-migrate/bin/db-migrate
```
## Undoing Migrations
With migration you can revert to old state by just running a command
```js
$ node_modules/.bin/sequelize db:migrate:undo
```
