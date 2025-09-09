# Joins

Esto es cuando se une una tabla con otra tabla.





### Tabla 1

```sql
create table user (
	id int not null auto_increment,
    name varchar(50) not null,
    primary key(id)
);
```





### Tabla 2

```sql
create table product (
	id int not null auto_increment,
    name varchar(50) not null,
    created_by int not null,
    marca varchar(50),
    primary key(id),
    foreign key (created_by) references user(id)
);
```



"created_by" sería el id del user de la tabla uno. Para esto tenemos que asignarle que sea una llave foranea con "foreign key" y agregar la referencia con la palabra "references", posteriormente agregar la tabla de referencia "user" y finalmente la columna de id.



## Insertar varios registros a la vez

Para esto vamos a indicar donde vamos a insertar los valores:

```sql
insert into product (name, created_by, marca)
```



Posteriormente se agrega la palabra clave value y se agregan los registros que se quieren agregar.

```sql
insert into product (name, created_by, marca)
values 
	('ipad', 1, 'apple'),
	('iphone', 1, 'apple');
```



## Left join

Left join funciona de la siguiente manera. Si estamos en una tabla, en este caso la tabla 2. Haremos una unión hacia la izquierda, es decir, hacia la tabla 1. De esta manera la tabla 2 pedirá todos los registros de la tabla 1 y se quedará con aquellos que hagan efectos sobre la tabla 2.



### ¿Como funciona?

Se utiliza la letra "u" para entregarle un alias a la tabla de usuario.



```sql
select u.id, u.email from user u
```



De esta manera le agregamos el alias a la tabla de la cual queremos traer la información. Posteriormente ponemos "u" seguido de un punto ponemos la columna que queremos traer.



Luego tenemos que indicarle que queremos hacer un left join con las palabras claves "left join" y posteriormente indicamos la tabla de donde queremos hacer el left join. Finalmente le agregamos una alias a la tabla, en este caso será "p".

```sql
select u.id, u.email from user u left join product p;
```



Por último agregaremos que producto queremos ver:

```sql
select u.id, u.email, p.name from user u left join product p;
```



Por último tenemos que indicarle que la columna de created_by en la tabla 2 está relacionado con la columna id de la tabla 1

```sql
select u.id, u.email, p.name from user u left join product p on u.id = p.created_by;
```



## Right join

Sería lo mismo que el left join. Pero traerá todos los datos de la tabla de la derecha. En este ejemplo sería desde la tabla 1 leer todos los elementos de la tabla 2 y traer aquellos que tengan relación con la tabla 1.



```sql
select u.id, u.email, p.name from user u right join product p on u.id = p.created_by;
```



## Inner Join

Nos traerá la intersección de las dos tablas.

```sql
select u.id, u.email, p.name from user u inner join product p on u.id = p.created_by;
```



## Cross Join

Nos trae el producto carteseano de las dos tablas

```sql
select u.id, u.name, p.id, p.name from user u cross join product p;
```





## Change name

```sql
rename table products to product;
```

