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
- `INT`
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
