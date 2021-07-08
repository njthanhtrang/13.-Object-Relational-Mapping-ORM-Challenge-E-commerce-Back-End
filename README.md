# 13. Object-Relational Mapping (ORM) Challenge: E-commerce Back End

# Purpose
This application serves as the backend of an e-commerce site, which uses a functional Express.js API and uses Sequelize to interact with a MySQL database.

When the user adds their database name, MySQL username, and MySQL password to an environmental variable file, the user is able to connect to a database using Sequelize. When entering schema and seed commands, a development database is created and is seeded with test data. When the application is invoked, the server is started and Sequelize models are synced to the MySQL database, with API GET routes for categories, products, and tags display a formatted JSON using Insomnia Core or Postman. When testing API POST, PUT, and DELETE routes in Insomnia Core, users can create, update, and delete data in the database.

MySQL2 and Sequelize packages connect the Express.js API to a MySQL database. The dotenv package uses environmental variables to store sensitive data, such as the user's MySQL username, password, and database name. On server start, the application syncs Sequelize models of Category, Product, Tag, and ProductTag to a MySQL database and includes associations between these models.

The associations are as follows:

* Product belongs to Category, as a category can have multiple products but a product can only belong to one category.

* Category has many Product models.

* Product belongs to many Tag models. Using the ProductTag through model, allow products to have multiple tags and tags to have many products.

* Tag belongs to many Product models.

In the future, this project may be refactored for improved efficiency and readability.

# Built With
* JavaScript
* HTML
* CSS
* Express.js
* MySQL2 https://www.npmjs.com/package/mysql2
* Sequelize https://www.npmjs.com/package/sequelize
* dotenv package

# Usage
Clone the repository, navigate to the project folder in your CLI and use the ```npm run seed``` to seed data to the database and test CRUD routes.

Video Demonstration: https://youtu.be/YqHXCVwpIE8

<img width="953" alt="Screen Shot 2021-07-07 at 8 14 31 PM" src="https://user-images.githubusercontent.com/77700824/124856750-f2017100-df5f-11eb-813b-8dc7bcd7ac40.png">
<img width="1131" alt="Screen Shot 2021-07-07 at 8 15 04 PM" src="https://user-images.githubusercontent.com/77700824/124856796-05acd780-df60-11eb-88b4-fea157e1bc70.png">
<img width="1126" alt="Screen Shot 2021-07-07 at 8 15 25 PM" src="https://user-images.githubusercontent.com/77700824/124856819-12313000-df60-11eb-809a-8d306396205e.png">
<img width="1137" alt="Screen Shot 2021-07-07 at 8 15 44 PM" src="https://user-images.githubusercontent.com/77700824/124856845-1cebc500-df60-11eb-971f-875adeccdaff.png">
<img width="1133" alt="Screen Shot 2021-07-07 at 8 16 25 PM" src="https://user-images.githubusercontent.com/77700824/124856901-3725a300-df60-11eb-8d7f-0c1af888caf2.png">

# Credits
Created by Jennifer Nguyen. Starter code retrieved from https://github.com/coding-boot-camp/fantastic-umbrella.

# Questions
For additional questions and information, please go to github.com/njthanhtrang/
or reach out via email at njthanhtrang@gmail.com.

# License
Copyright 2019 Horiseon Social Solution Services, Inc.
© 2021 Trilogy Education Services, LLC, a 2U, Inc. brand. Confidential and Proprietary. All Rights Reserved.


