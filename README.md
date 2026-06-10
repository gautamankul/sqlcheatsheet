# MySQL Cheat Sheet
This cheat sheet provides a quick reference to commonly used MySQL commands for database management, data manipulation, user management, and more.

## Basic Commands
- Connect to MySQL: `mysql -u username -p`
- Show databases: `SHOW DATABASES;`
- Use a database: `USE database_name;`
- Show tables: `SHOW TABLES;`
- Describe a table: `DESCRIBE table_name;`
- Exit MySQL: `EXIT;`

## Data Manipulation
- Insert data: `INSERT INTO table_name (column1, column2) VALUES (value1, value2);`
- Update data: `UPDATE table_name SET column1 = value1 WHERE condition;`
- Delete data: `DELETE FROM table_name WHERE condition;`
- Select data: `SELECT column1, column2 FROM table_name WHERE condition;`
- Select all data: `SELECT * FROM table_name;`

## Data Definition
- Create database: `CREATE DATABASE database_name;`
- Create table: `CREATE TABLE table_name (column1 datatype, column2 datatype);`
- Alter table: `ALTER TABLE table_name ADD column_name datatype;`
- Drop table: `DROP TABLE table_name;`
- Drop database: `DROP DATABASE database_name;`

## User Management
- Create user: `CREATE USER 'username'@'host' IDENTIFIED BY 'password';`
- Grant privileges: `GRANT ALL PRIVILEGES ON database_name.* TO 'username'@'host';`
- Revoke privileges: `REVOKE ALL PRIVILEGES ON database_name.* FROM 'username'@'host';`
- Show users: `SELECT User, Host FROM mysql.user;`
- Delete user: `DROP USER 'username'@'host';`

## Backup and Restore
- Backup database: `mysqldump -u username -p database_name > backup.sql`
- Restore database: `mysql -u username -p database_name < backup.sql`

## Miscellaneous
- Show MySQL version: `SELECT VERSION();`
- Show current date and time: `SELECT NOW();`
- Show current database: `SELECT DATABASE();`
- Show server status: `SHOW STATUS;`
- Show process list: `SHOW PROCESSLIST;`
- Show variables: `SHOW VARIABLES;`
- Show indexes: `SHOW INDEX FROM table_name;`
- Show foreign keys: `SHOW CREATE TABLE table_name;`
- Show stored procedures: `SHOW PROCEDURE STATUS;`
- Show triggers: `SHOW TRIGGERS;`
- Show events: `SHOW EVENTS;`
- Show views: `SHOW FULL TABLES WHERE TABLE_TYPE = 'VIEW';`
- Show functions: `SHOW FUNCTION STATUS;`
- Show grants: `SHOW GRANTS FOR 'username'@'host';`
- Show character sets: `SHOW CHARACTER SET;`
- Show collations: `SHOW COLLATION;`

# Note: Replace `username`, `password`, `database_name`, `table_name`, `column1`, `column2`, `value1`, `value2`, and `condition` with your actual values when executing the commands.