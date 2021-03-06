# Using the exam playground

This project is for testing code samples and implementations in an environment used in the Code Fellows 301 curriculum

## Installation

To install the project, navigate to this directory in your terminal and install all project dependencies:
```
npm install
```

## Using Postgres

If you are using a Postgres database create a file title `.env` and add one of the following environment variables:
```
# linux / mac users
DATABASE_URL=postgres://localhost:5432/exam_playground

# Windows Users
DATABASE_URL=postgres://USERNAME:PASSWORD@localhost:5432/exam_playground
```

## Configuring Postgres

Create a Database for the playground
```sql
CREATE DATABASE exam_playground
```

Add any tables you want to test
```sql
CREATE TABLE tableName(
  columnName TYPE,
  columnName TYPE
);
```

### Optional

You can add the above to a schema.sql file and initialize your databse with psql:

```
psql -d exam_playground -f path/to/file.sql
```

## Running the playground

Use npm script to either start the server or watch files with nodemon:

```
npm start
```
or
```
npm run watch
```

Happy Hacking!
