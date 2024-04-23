# MySQL Cheatsheet

## Connect to MySQL Server
- Connect to MySQL: `mysql -u <username> -p`

## Database Operations
- Show databases: `SHOW DATABASES;`
- Create database: `CREATE DATABASE <database_name>;`
- Use database: `USE <database_name>;`
- Drop database: `DROP DATABASE <database_name>;`

## Table Operations
- Show tables: `SHOW TABLES;`
- Describe table: `DESCRIBE <table_name>;`
- Create table: 
  '''
  CREATE TABLE <table_name> (
      column1 datatype constraints,
      column2 datatype constraints,
      ...
  );
  '''
- Drop table: `DROP TABLE <table_name>;`

## Data Manipulation
- Insert data into table:
  '''
  INSERT INTO <table_name> (column1, column2, ...)
  VALUES (value1, value2, ...);
  '''
- Select data from table: `SELECT * FROM <table_name>;`
- Update data in table:
  '''
  UPDATE <table_name>
  SET column1 = value1, column2 = value2, ...
  WHERE condition;
  '''
- Delete data from table: `DELETE FROM <table_name> WHERE condition;`

## User and Privilege Management
- Show users: `SELECT User, Host FROM mysql.user;`
- Create user: `CREATE USER '<username>'@'localhost' IDENTIFIED BY '<password>';`
- Grant privileges: `GRANT ALL PRIVILEGES ON <database_name>.* TO '<username>'@'localhost';`
- Flush privileges: `FLUSH PRIVILEGES;`

## Backup and Restore
- Backup database: `mysqldump -u <username> -p <database_name> > backup.sql`
- Restore database: `mysql -u <username> -p <database_name> < backup.sql`

## Exit MySQL
- Exit MySQL: `exit;`

