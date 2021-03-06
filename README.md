# GoFinance - Back-end

This project is a very simple cash flow app made for me with the purpose of learning the tech involved. It was an exercise on Rocketseat's Bootcamp.

### Features:
  - List, add and remove financial transactions
  - Import a transaction csv file 

### Tech:

  - Node.js
  - TypeScript
  - Postgres via docker
  - TypeORM

### Setup:
  - Install Postgres or a container of Postgres in Docker
  - Configure the file ormconfig.json properly (database connection config) and start the database
  - Run the command to install all dependencies
  ```  
yarn
```
  - Run the typeorm script to create the tables:
  ```
  yarn typeorm migration:run
```
  - Run the project:
  ```
  yarn dev:server
```
  
### Endpoints
/transactions   </br>
/transactions/:id  </br>
/transactions/import  </br>

### CSV file example
```
title, type, value, category
Loan, income, 1500, Others
Website Hosting, outcome, 50, Others
Ice cream, outcome, 3, Food
```

### JSON post example
```json
{ 
	"title": "salario",
	"value": 10, 
	"type": "income",
	"category": "Radical"
}
```
### ReactJS Front-end for this project:
[gofinance-reactjs](https://github.com/rlovatto/gofinance-reactjs)
