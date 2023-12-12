
# Inventory Management and Billing Website using NodeJS and Javascript 

 In this project, we made a dynamic website for managing inventory with features like Billing, Adding, Removing Inventory/Stock and Analysis of Sales and Stocks with custom filters for a retail client
  
## Authors

- [@Rohit](https://github.com/rohit-gore).
  
## Features

- Stock Inventory
- Billing
- Sales Analysis
- Stock Analysis
- Generation of Bill in printable format
  
## Tech Stack

**Client:** Javascript, Bootstrap, Semantic-UI

**Server:** Node, Express

## Install node dependencies and run server locally

Go to the project directory

```bash
  cd Inventory-Management-and-Billing-Website
```

Install dependencies

```bash
  npm install
```

Start the server (Please set up the environment variables before starting the server)

```bash
  npm run start
```

Type this is your browser to open the local version of the website

```bash
  http://localhost:5000/
```
 
## Environment Variables

To run this project, you will need to add the following environment variables to your `.env` file (Create a file named `.env` at the root of your project directory, i.e., in **Inventory-Management-and-Billing-Website** folder)

```bash
SESSION_SECRET=secret

port=5000

db_host=localhost

db_name=warehousedb

db_user_name=<database_user_name>

db_password=<database_password>

login_id=<login_email_address>

login_password=<password_for_login>
```

Here `db_host` is the port number for hosting the server.js file, `login_id` and `login_password` are the login credentials for the website. Similarly `db_user_name` and `db_password` are the credenials for the MySQL database which was configured during installation of MySQL. So please change all the credentials accordingly. 
Leave `SESSION_SECRET=secret` and `db_name=warehousedb` as it is.

Folowing is an example with actual values in a .env file:-

```bash
SESSION_SECRET=secret

port=5000

db_host=localhost

db_name=warehousedb

db_user_name=root

db_password=root1234

login_id=admin@xyz.com

login_password=admin1234
```
  
In the `.env` file, don't use double quotes for values and there should be no space before or after `=`. Also you can edit the shop name and other details on the bill pdf generated by simply going to **views/bill.ejs** and editing lines `488` to `494` in the file

  
