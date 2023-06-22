# E-Commerce Back End: Example Demo

## Desccription

&emsp; This is an example of back end functionality of e-commerce site that could be used in building an e-commerce platform or building understanding of basic back end functionality. 

&emsp; With this functional Express.js API, a user must add their own database name, MySQL username, and MYSQL password to an environment variable file (.env). The database name will be the same as in the schema file, unless the user wishes to change it.
Then, the user will able to connect to the database through Sequalize. When a user creates the database with the schema file, they are able to seed the database and then run the application with the newly deployed database.

&emsp; Once the user starts the application, the server starts and Sequalize models are synced to the MySQL database. When testing the api routes with a program like Insomnia, the user is able to GET routes for categories, products, and tags. The user is also able to test API's POST, PUT, and DELETE routes for those as well.
This allows the user to create, update, and delete data for their database.

 ## Table of Contents

  * [Installation](#installation)
  * [Usage](#usage)
  * [Contribution](#contribution)
  * [Tests](#test)
  * [Questions](#questions)
  * [License](#license)

## Installation

  1. To install just clone this repo:
  ```
  git clone git@github.com:hculp/note-taker.git
  ```
  2. Install all required packages through the cloned package.json:
  ```
  npm i
  ```
  3. Create and enviromental variable file to connect to the database and include the database name, your MySQL username, and MySQL password. Similar to this example:
  ```
  DB_NAME='ecommerce_db'
  DB_USER='root'
  DB_PASSWORD='1234'
```
 
  4. Initiate MySQL and then create the database:
  ```
  mysql -u [your username] -p [your password]
  mysql> source db/schema.sql;
  mysql> use ecommerce_db;
  mysql> quit;
  ```
  5. Then seed the database in the terminal using node:
  ```
  node seeds/index.js
  ```
  ## Usage

  All that's need to do to start is to run:
  ```
  npm start
  ```
  Then you can test the API endpoints for each route with a program like Insomnia.
  <br> Here is a [walkthrough video](https://drive.google.com/file/d/1QYbDIWxUMM7JyixoAHrNR7gv7quCLK2F/view) demoing the installation process and route testing. 
  ## Contribution

  Contribution falls under open ISC license.

  ## Tests

  N/A

  ## Questions

  Send any questions or feedback to the following contacts:

  * GitHub: [https://github.com/hculp](https://github.com/hculp)
  * Email: [howacul@gmail.com](mailto:howacul@gmail.com)
  
  ## License

    Copyright (C) 2023 Houston Culpepper.     
    
    Distributed under the ISC License.
  [Link to ISC license](https://choosealicense.com/licenses/isc)