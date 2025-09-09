# Group By



Group by se usa con instrucciones que tienden a agrupar ciertos registros.

 

```sql
select count(id), marca from product group by marca:
```



En este ejemplo se agruparán por marcas.



Ahora se hará un left join partiendo de la tabla 2.

```sql
select count(p.id), u name from product p left join user u on u.id = p.created_by group by p.created_by
```



Tambien podemos filtrarlos dependiendo de el número de id utilizados.

```sql
select count(p.id), u name from product p left join user u on u.id = p.created_by group by p.created_by
having count (p.id) >= 2; 
```



## Drop table



De esta forma se borrarán las tablas.



```sql
drop table product
```

