# Condiciones



## Limit

The `LIMIT` clause is used to specify the number of records to return.

The `LIMIT` clause is useful on large tables with thousands of records. Returning a large number of records can impact performance.

```sql
select * from user limit 1;
```



Eso limitará a uno, es decir que te retornará el primer registro.



## Where

The `WHERE` clause is used to filter records. It is used to extract only those records that fulfill a specified condition.



## Operators

| Operator | Description                                                  |
| -------- | ------------------------------------------------------------ |
| =        | Equal                                                        |
| >        | Greater than                                                 |
| <        | Less than                                                    |
| >=       | Greater than or equal                                        |
| <=       | Less than or equal                                           |
| <>       | Not equal. **Note:** In some versions of SQL this operator may be written as != |
| BETWEEN  | Between a certain range                                      |
| LIKE     | Search for a pattern                                         |
| IN       | To specify multiple possible values for a column             |





### AND, OR and  NOT operators

The `WHERE` clause can be combined with `AND`, `OR`, and `NOT` operators.

The `AND` and `OR` operators are used to filter records based on more than one condition:

- The `AND` operator displays a record if all the conditions separated by `AND` are TRUE.
- The `OR` operator displays a record if any of the conditions separated by `OR` is TRUE.

The `NOT` operator displays a record if the condition(s) is NOT TRUE.



### Between

A este se le tienen que indicar dos argumentos y nos votará toda la información que se encuentre entre los dos argumentos, por ejemplo:

```sql
select * from user where edad between 15 and 30;
```



### Order by

Ordenará todos los resultados de una columna. Posteriormente se le indicará el orden ya sea ascendente o descendente,

```sql
select * from user order by edad asc;
select * from user order by edad desc;
```



## Other conditionals

| Symbol | Description    |
| ------ | -------------- |
| %      | any characters |
|        |                |
|        |                |



## Conditional Functions



| Function | Description                             |
| -------- | --------------------------------------- |
| max()    | Máximo                                  |
| min()    | Mínimo                                  |
| as       | para indicar como queremos que se llame |



```sql
select max(edad) as mayor from user;
```





