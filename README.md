# Sequelize-crud-workshop

A workshop on basic CRUD operations using Sequelize- ORM tool for NodeJs and it supports the dialects PostgreSQL, MySQL, SQLite and MSSQL. This application uses Node vexrsion 5.6.0, Express.js to build API, Sequelize version 3.24.3 and PostgreSQL 6.1.0 version as the dialect.

## Installation

#### Installing Git – the easy way

##### Installing Git on Windows

Download Git from Git for Windows- https://gitforwindows.org/ and install it.

##### Installing Git on Mac


Copy & paste the following into the terminal window and hit Return.

ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor

You will be offered to install the Command Line Developer Tools from Apple. Confirm by clicking Install. After the installation finished, continue installing Homebrew by hitting Return again.

=======
# Sequelize-crud-worksop

A workshop on basic CRUD operations using Sequelize- ORM tool for NodeJs and it supports the dialects PostgreSQL, MySQL, SQLite and MSSQL. This application uses Node vexrsion 6, Express.js to build API, Sequelize version 3.24.3 and PostgreSQL 6.1.0 version as the dialect.

## Installation

#### NodeJS
Download from this link: https://nodejs.org/en/download/ (Links to an external site.)Links to an external site.

Note: Please make sure you download the LTS version.

#### PostgreSQL
You can download PostgreSQL from this link: https://www.postgresql.org/download/ (Links to an external site.)Links to an external site.

In case you have any issues, please follow this tutorial for installation:

http://www.postgresqltutorial.com/install-postgresql/ (Links to an external site.)Links to an external site.

#### Postman- API Testing Tool

https://www.getpostman.com/ (Links to an external site.)Links to an external site.

 
## Getting Started

First fork the repository into your github profile and later clone the project using the command:

#### git clone https://github.com/SrideviAkondi/Sequelize-crud-workshop.git 

Now move to project directory and use the git commands

#### git checkout CRUD

#### git fetch 

You can now see the project structure. Next open pgAdmin4 and connect to the database server at port number 5432. Later create a database that has been mentioned in the env.js file located in the config of the server folder.

### List of commands after installing npm and postgreSQL

#### npm install --save sequelize

#### npm install --save pg pg-hstore body-parser express morgan sequelize-cli nodemon

#### npm run dev

### Sample JSON Data

#### To insert an owner 

Json Input: 
[{
	"name": "Carol",
	"role": "admin"
},

{
	"name": "Adam",
	"role": "user"
}]

#### To update an owner with owner_id

Json Input: 

{
  "updates": {
    "name": "Loren Stewart",
    "role": "user"
  }
}

#### To get an owner using owner_id

Pass the owner_id as a param to the URI

#### To insert a pet where owner_id becomes the foreign key

Json Input: 

[{
	"name":"Becky",
	"owner_id": "",
	"type": "cat"
},

{
	"name":"Marley",
	"owner_id": "",
	"type": "dog"
},

{
	"name":"Becky",
	"owner_id": "",
	"type": "cat"
},

{
	"name":"Bruno",
	"owner_id": "",
	"type": "dog"
}]

#### To delete an owner using owner_id

Results in 1 or 0. 1 indicates sucessful deletion where parnoid is true.
