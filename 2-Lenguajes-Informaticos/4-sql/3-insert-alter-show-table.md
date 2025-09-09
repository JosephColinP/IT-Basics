# Inset alter and show table



## INSERT INTO



Continuando con la tabla anterior:

```sql
CREATE TABLE animales(
	id int,
	tipo varchar(255),
    estado varchar (255),
    PRIMARY KEY (id)
);
```



To insert values we use "INSERT INTO"

```sql
INSERT INTO animales (tipo, estado)
```



Then we specify the values:

```sql
INSERT INTO animales (tipo, estado) VALUES ('chanchito', 'feliz');
```



## ALTER TABLE

Now it will appear an error because we didn't specify an auto increment in the id column. So we have to modify the id column. To do this we use "ALTER TABLE ... MODIFY"



```sql
ALTER TABLE animales MODIFY COLUMN id int auto_increment;
```



*Note: We have to specify once again which type of date goes inside the id Column.*



To avoid this we can create this from the beginning:

```sql
CREATE TABLE animales (
	id int NOT NULL auto_increment
);
```

 This says that id's values are int, the column is not null and it will auto increment.



## List Elements

For this we use "SELECT". We first need to specify which column and then which table.

```sql
SELECT * FROM animales;
```



The " * " symbol, is used to select all the columns in a table. If we want to specify one row we use the following instruction:

```sql
SELECT * FROM animales WHERE id = 1;
```



So is going to show us the row with id 1. If we want to filter many values with a common register we use:

```sql
SELECT * FROM animales WHERE estado = feliz;
```



En este ejemplo anterior podemos tener varios registros de animales donde sus estados sean felices, por lo que nos aparecerán todos los animales con un estado feliz.



We also can add a condition, example:

```sql
SELECT * FROM animales WHERE estado = feliz AND tipo = 'chanchito';
```



En este ejemplo solo nos dará los resultados que tengan un estado feliz y sean tipo chanchito.



### Seleccionar una columna en específico

También se puede seleccionar una columna en específico por ejemplo:

```sql
select id, name from user;
```

Seleccionará el nombre de la columna de "id", ahora tenemos la "," porque queremos darle la instruccion de seleccionar tambien la columna de "name". Por ultimo estas dos columnas se seleccionarán de la tabla "user".



### Cabmiar el nombre de la columna retornado

Este se puede cambiar de la siguiente manera:

```sql
select id, name as nombre from user;
```





## Update Register

Para hacer un update de un registro utilizamos el key word "UPDATE" y "SET". Ejemplo:

```sql
UPDATE animales SET estado = 'feliz' where id = 3;
```



En este ejemplo vamos a hacer un update a la tabla animales, vamos a utlizar la palabra "SET" para establecer nuevos valores. En este caso seleccionamos la columna estado y establecimos el valor a "feliz". Posteriormente con "where" indicamos el id donde se realizará este update.





## Delete Registers

```sql
DELETE from animales where estado = 'feliz'
```



En este ejemplo el comando "DELTE" es para borrar, "from" indica de donde, "where" la condición, la cual es que se borrará los estados que contengan el valor "feliz".



Nota: En MySQL existe un safe mode, en el que no nos deja borrar datos con where y necesitaríamos obligatoriamente indicarle un ID. Esto es para evitar borrar registros indeseados. Por lo que quedaría de la siguiente forma: DELETE from animales where id = 3; 

Por último este error anterior también pasará en MySQL en caso de los "DELETE" y "UPDATE".





## Comments

You add comments with double dash.



