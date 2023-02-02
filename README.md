# E-commerce Back End Starter Code

## Coding Badges
![alt text](https://img.shields.io/badge/Node.js-modules-green)
![alt text](https://img.shields.io/badge/JavaScript-.js-yellowgreen)

# Description 
A back-end server that uses Express.js API to run, and Sequelize to store and maintain the information being put into the backend server. You can use insomnia to configure the information stored inside the database and keep your e-commerce retail database all up to date.

# requirements 
first and create a .env folder and add the follow to it replacing the words in the quotes with your Username and Password
```
DB_NAME ="ecommerce_db"
DB_USER ="DB_USER"
DB_PW ="DB_PW"
```
then run

```
npm i 
```
to install all modules for this application to work.
From there login into mysql and source the data base
```
SOURCE schema.sql
```

From there run
```
node server.js
```
and it will create the server
from there launch insomnia and you can view, update, add or/add delete the database using
```
http://localhost:3001/api/tags/
http://localhost:3001/api/products/
http://localhost:3001/api/categories/
```
Example of get call for all tags

<img src="assets/images/Screenshot%20of%20insomnia%20get%20call%20for%20the%20tags%20222552.png" width="1250" alt="Insomnia get call for all tags">

example of GET call for Categories by ID
<img src="assets/images/Screenshot%20of%20GET%20call%20for%20one%20Categories%20by%20ID223102.png" width="1250" alt="Insomnia get call for one Category">

# DEMO VIDEO

[Demo of using setting up database and using Insomnia to view and edit it](https://clipchamp.com/watch/hp93mtOUc7N)


# Acceptance Criteria
```
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia Core for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete data in my database
```