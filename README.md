# E-commerce Back End

## Description
Build the backend for an e-commerce platform using Express.js API and configure it to use Sequelize to interact with a MySQL database.

## User Story
AS A manager at an internet retail company  
I WANT a back end for my e-commerce website that uses the latest technologies  
SO THAT my company can compete with other e-commerce companies

## Acceptance Criteria
- GIVEN a functional Express.js API
- WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
- THEN I am able to connect to a database using Sequelize
- WHEN I enter schema and seed commands
- THEN a development database is created and is seeded with test data
- WHEN I enter the command to invoke the application
- THEN my server is started and the Sequelize models are synced to the MySQL database
- WHEN I open API GET routes in Insomnia Core for categories, products, or tags
- THEN the data for each of these routes is displayed in a formatted JSON
- WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
- THEN I am able to successfully create, update, and delete data in my database

## Mock-Up
The following animations show examples of the application's API routes being tested in Insomnia Core.

The first animation shows GET routes to return all categories, all products, and all tags being tested in Insomnia Core:

![](./assets/images/13-orm-homework-demo-01.gif)

The second animation shows GET routes to return a single category, a single product, and a single tag being tested in Insomnia Core:

![](./assets/images/13-orm-homework-demo-02.gif)

The final animation shows the POST, PUT, and DELETE routes for categories being tested in Insomnia Core:

![](./assets/images/13-orm-homework-demo-03.gif)

## Github Repository
All files and changes made are located on github at the following location:

https://github.com/htang2021/orm-ecommerce

## Walk-Thru Video Link


## Deploy Your Project
This instruction below assumes that a project and repo were already created on github and that they are already linked as appropriate.
(https://github.com/htang2021/orm-ecommerce).

1. From the local CLI at the root of the project repo, do a git clone or git pull
2. Install the appropriate NPM packages dependencies, $ npm install
3. Verify, or create if needed, that .gitignore include node_modules/, .DS_Store, package-lock.json, and .env entries
4. Perform git add, commit, and push as appropriate to baseline the deployment repository
5. Log into a local database via MySQL2 client
6. Once at SQL> interface, create a database 'ecommerce_db':
 - SQL> source db/schema.sql;
7. Verify that the database has been created successfully:
 - SQL> show databases; (should should 'ecommerce_db' as a listed entry)
8. Exit out of SQL connection by typing 'exit' from the SQL> prompt.
9. Run $ npm run seed to insert seed tables and data into the schema created.
10. Issue command 'npm start' to run the application.
11. Using Insomnia with pre-populated calls and verify each of the endpoints for GET, POST, PUT, and DELETE operations are updated and returned correctly in the database tables, for Category, Product, Tag, and ProductTag.
12. Reference the walk-thru video for each of the supported RESTful operations.


## Questions
Feel free to reach out to [me](mailto:hungtang@hotmail.com).

README.md - updated by Hung Tang on 5/2/21