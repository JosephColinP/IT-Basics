# Create Database



## Creation of a data base

First we got to create the database with the command "create database". Then we create de table with the command "CREATE TABLE anyname();". 

| Command                 | Description                                |
| ----------------------- | ------------------------------------------ |
| create database "name"; | Crea una base de datos.                    |
| show databases;         | List data bases.                           |
| use "database name";    | To specify which database should.          |
| CREATE TABLE "name" (); | Crea una tabla dentro de la base de datos. |



After that inside the table command we specify our table data types. Example:

```sql
CREATE TABLE animales(
	id int,
	tipo varchar(255),
    estado varchar (255),
    PRIMARY KEY (id)
);
```



In the previous example we first specify the column name, example:

```sql
CREATE TABLE animales(
	id,
	tipo,
    estado,
);
```



After that we specify what type of data should the column store. For example "int" for numbers or "varchar" for strings.

```sql
CREATE TABLE animales(
	id int,
	tipo varchar(),
    estado varchar (),
);
```



Inside the varchar parenthesis we specify how many characters should store, in this example is 255.

```sql
CREATE TABLE animales(
	id int,
	tipo varchar(255),
    estado varchar (255),
);
```



Lastly we specify which column is the primary key:

```sql
CREATE TABLE animales(
	id int,
	tipo varchar(255),
    estado varchar (255),
    PRIMARY KEY (id)
);
```



### Primary Key

A primary key is a field in a table which uniquely identifies each row/record in a database table. Primary keys must contain unique values. A primary key column cannot have NULL values.



### Data types

| Name    | Ejemplo       | Description               |
| ------- | ------------- | ------------------------- |
| Int     | 1             | Número entero.            |
| Float   | 5.7           | Números con decimales.    |
| varchar | 'Hello World' | Una cadena de carácteres. |



