## About
It is basically a Phone Book Web Application using Node Express and MySQL as its Database.

## Install All the Dependencies
```
npm i
```

## Connect to the Database
You must have to connect this application to your MySQL Database using environment variables

## Create Tables
You have to create two tables. I have added the commands below so that yoy can create those tables yourself
### User Table:
```
CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(100) NOT NULL,
  password VARCHAR(100) NOT NULL
);
```
### Phones Table:
```
CREATE TABLE phones (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(250) NOT NULL,
  phone VARCHAR(100) NOT NULL,
  user_id INT NOT NULL,
  FOREIGN KEY(user_id) REFERENCES users(id)
);
```

## Run development server
```
npm run dev
```

## Thanks
Thanks!
```
