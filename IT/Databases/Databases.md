# Database types
- Relational
- Documental
# Database Schemas
The structure of the database
## Touples
A touple is identified by an Unique Identifier and it represents the data row inside an SQL database row. The UID is also a Primary key used to relation tables between eachother.
## DBMS
DataBase Management System
# Database graphical representation
## Underlined key:
UID
## Double underlined key
External key
# SQL
SQL is a **Data Definition Language** that defines a set of instructions to work upon a database. It can create, delete, update and drop data schemas.
It's also a **Data Manipulation Language** which is like the Data Definition Language but allows instead to fill, edit and delete touples.
Then we have a **Query Language** which is how you query requests from the database.
Lastly, the **Data Control Language** allows to check access permissions for tables.
## SQLite
SQLite has only one file for multiple tables. It has whatever extension you want.
### SQLite GUI
SQLite Browser
## Schema structure
Follows an example (SQL Lite)
```sql
CREATE TABLE students(id TEXT PRIMARY KEY, name TEXT, surname TEXT, age INT);
```
Here's another example on how a schema is defined:
```sql
CREATE TABLE grades(id INT PRIMARY KEY,
						  subject TEXT,
						  grade INT,
						  student_id TEXT,
						  FOREIGN KEY(student_id) REFERENCES students(id),
						  CHECK voto > 0 AND voto < 11);
```
An integer primary key is always automatically defined by SQL Lite sequentially.
To define a field as primary key it's also possible to do as follows:
```sql
I DONT KNOW
```
### Data types
In SQL Lite:
- `INT` / `INTEGER`
- `TEXT`
## Commands
- Create:
  ```sql
  CREATE TABLE tableName(schema);
```
- Drop:
  ```sql
  DROP TABLE tableName;
```
- Alter:
  ```sql
  ALTER TABLE tableName ADD COLUMN newColumn DATATYPE;
```
- Insert
  ```sql
  INSERT INTO tableName VALUES(value1, value2, value3);
```
If `null` is used instead of a value, the automatic value will be used.
- Check
  ```SQL
  CHECK(query)
```
- Select
  ```SQL
  SELECT * FROM table;
  ```
	Selects everything
	```SQL
	SELECT column, column FROM table;
	```
	Selects specific columns
- Where:
  ```sql
  ... WHERE column CONDITION
	```
- Set foreign key enforcement:
```sql
PRAGMA FOREIGN_KEYS = "ON";
	```
- Delete
	```sql
	DELETE FROM table WHERE ...
	```
- Join
	Selects all rows across multiple tables making a joined thing and shows only the stuff that matches a condition
	```sql
	SELECT studenti.*, voti.* FROM voti INNER JOIN studenti;
	```
	Joins all columns no matter what. To select all the touples that share an attribute:
	```sql
	SELECT studenti.*, voti.* FROM voti INNER JOIN studenti 
		ON studenti.matricola = voti.matricola;
	```
- Select multiple
	```sql
	SELECT table1.*, table2.* FROM table1,table2 WHERE ...;
	```
