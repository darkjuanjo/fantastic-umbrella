# E-commerce Back End Starter Code

## Description 

The purpose of this app is to view and manage employees,roles and deparments using MYSQL.

## Challenge Requirements 
 * Use MYSQL
 * Use Sequelize
 * Model: Category
       1. id: Integer, no null values, primary key, autoincrement
       2. category_name: String, no null values
 * Model: Product
       1. id: Integer, no null values, primary key, autoincrement
       2. product_name: String, no null values
       3. price: Decimal, no null values, validate decimal
       4. stock: integer, no null values, default value of 10, validate numeric
       5. category_id: integer, references category_id
 * Model: Tag
       1. id: Integer, no null values, primary key, autoincrement
       2. tag_name: String
 * Model: ProductTag
       1. id: Integer, no null values, primary key, autoincrement
       2. product_id: integer, reference product_id
       3. tag_id: integer, refercnes tag_id
 * Associations
       1. Product belongs to Category 
       2. Category has many Product models
       3. Tag belongs to many Products models
 
## Table of Contents

* [Installation Manual](#installation-manual)
* [Usage-Manual-INSOMNIA](#usage-manual-insomnia)
* [Screenshots](#screenshots)
* [License](#license)

## Installation-Manual

1. Download/Clone app from github repository
2. Open terminal and navigate to the root folder of the app (It should contain the app.js file).
3. Run the `npm install` command to automatically install all the required dependencies.
4. Create a new MYSQL database with the name management;
5. Once the dependencies finish installing and the MYSQL database was created run the `node server.js` to launch the application.

## Usage-Manual-INSOMNIA

1. Open terminal and navigate to the root folderof the application.
2. Once you are in the root folder run the command `node server.js`
3. One the server runs open INSOMNIA and try the GET/POST/PUT/DELETE 
    * http://localhost:3001/api/products
    * http://localhost:3001/api/categories
    * http://localhost:3001/api/tags

## Screenshots

### Video Preview
https://watch.screencastify.com/v/aADBQNBa8f9mzlCYT2ba


## License

ISC
    
