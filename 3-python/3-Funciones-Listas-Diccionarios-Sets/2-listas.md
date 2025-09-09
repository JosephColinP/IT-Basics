# Listas o Arrays



- [Definir Listas](#Definir Listas)
- [Utilización de los datos de la lista](#Utilización de los datos de la lista)
- [Multilistas](#Multilistas)
- [Funciones y métodos para listas](#Funciones y métodos para listas)

Listas o arrays son un conjunto de datos o valores bajo un único nombre, para acceder a ellos se puede utilizar un índice numerico. 



## Definir Listas



### Ejemplo 1 "Corchetes"

```python
peliculas = ["batman", "spiderman", "capitan america"]
print(peliculas)
```



### Ejemplo 2 "funciones list y tupla"

```python
peliculas = list(("batman", "spiderman", "capitan america"))
print(peliculas)
```



### Ejemplo 3 "Funcion List y Range"

```python
numeros= list(range(0, 100))
print(numeros)
```



### Ejemplo 4 "Las listas no están obligadas a un solo formato"

```python
variada = ["victor", 30, 20, True]
print(variada)
```



## Utilización de los datos de la lista



### Acceder a los datos de la lista

Para acceder a los indices se indica el nombre de la lista y el número del indice.

```python
peliculas = ["superman", "spiderman", "wolverine"]
print(peliculas[1])
```



### Imprimir Indices

Para imprimirlos se utiliza el print, el nombre de la lista y los valores.

```python
peliculas = ["superman", "spiderman", "wolverine"]
print(peliculas[1:3])
```



### Modificar Indices

Para modificarlos solo se pasa la lista y el valor a modificar.

```python
peliculas = ["superman", "spiderman", "wolverine"]
peliculas[1] = "Venom"
print(peliculas)
```



### Agregar un nuevo Dato

Para agregarlo solo basta con poner la lista “.append” y agregar el nuevo dato.

```python
peliculas = ["superman", "spiderman", "wolverine"]
peliculas.append("X-Men")
print(peliculas)
```



### Recorrer la lista verticalmente

Se pone “for” para pelicula, “in” adentro iran peliculas. 

```python
peliculas = ["superman", "spiderman", "wolverine"]
for pelicula in peliculas: #esto significa que se irán guardando los elementos en la variable peliculas
    print(pelicula)
```



### Enumerar datos

 Se utiliza "for" para pelicula, “in” adentro irán peliculas.  y peliculas “.index” para que regrese el primer valor + 1 ya que siempre se empieza de 0 y se quiere que empieze de 1.

```python
peliculas = ["superman", "spiderman", "wolverine"]
for pelicula in peliculas: 
    print(f"{peliculas.index(pelicula)+1}. {pelicula}")
```



### Agregar películas, imprimirlas verticalmente y enumerarlas

Se agrega la lista peliculas con datos. Se agrega una nueva variable con valor vacío. Se agrega un bucle “while”, cuando la nueva pelicula sea diferente “!=” a “parar” se va a introducir una nueva pelicula con “input”, cuando sea el dato diferente “!=” a “parar” se va a agregar “.append”  para que la nueva pelicula se incorpore al final de la lista. 

```python
peliculas = ["superman", "spiderman", "wolverine"]

nueva_pelicula =""

while nueva_pelicula != "parar":
    nueva_pelicula = input("Introduce una pelicula: ")
    if nueva_pelicula != "parar":
        peliculas.append(nueva_pelicula)

print("####### Peliculas #######")

for pelicula in peliculas: 
    print(f"{peliculas.index(pelicula)+1}. {pelicula}")
```



## Multilistas

Multilistas son listas dentro de otras listas. Se agrega la lista y dentro varios corchetes para indicar varias listas.

```python
contactos = [
    ["Salvador", "4491513667"],
    ["Jose Luis", "4491513668"],
    ["Victor", "4491513678"],
]

print(contactos)
```



### Extraer elemento específico

Se selecciona el número de la lista y el número del valor o dato.

```python
contactos = [
    ["Salvador", "4491513667"],
    ["Jose Luis", "4491513668"],
    ["Victor", "4491513678"],
]

print(contactos[1][0])
```



### Extraer Lista de Elemento

Se agrega un bucle for. Este bucle se llamará contacto, hará vueltas en  la lista "contactos". Finalmente se imprimirá contacto, pero en específico el valor "0".

```python
contactos = [
    ["Salvador", "4491513667"],
    ["Jose Luis", "4491513668"],
    ["Victor", "4491513678"],
]

for contacto in contactos:
    print(contacto[0])
```



### Imprimir lista con los datos clasificados

Se agrega una lista, posteriormente “for” para contacto, “in” adentro irán contactos y  "for" para elemento, adentro iran "in" contacto. "If" si contacto ".index" regresa el primer valor, elemento = 0. I, prime el nombre más el elemento, si no, “else” imprime el numero + elemento.

```python
contactos = [
    ["Salvador", "4491513667"],
    ["Jose Luis", "4491513668"],
    ["Victor", "4491513678"],
]

for contacto in contactos:
    for elemento in contacto:
        if contacto.index(elemento) == 0:
            print("Nombre: " + elemento)
        else:
            print("Numero: " + elemento)
    print ("\n")

```



## Funciones y métodos para listas



### Ordenar 

".sort" ordena los datos de manera ascendente y regresa nada.

```python
numeros = [1, 3, 5, 2, 9, 7]
numeros.sort()
print(numeros)
```



### Agregar Datos

Se puede con el .append que lo agregará automáticamente al último de la lista. También se puede hacer con .insert pero se tendrá que agregar el número donde se va a añadir el dato.



#### .append

```python
cantantes= ["Bad bunny", "Arcangel", "Myke Towers"]
cantantes.append("Sech")

print(cantantes)
```



#### .insert

```python
cantantes= ["Bad bunny", "Arcangel", "Myke Towers"]
cantantes.insert(1, "Sech")

print(cantantes)
```



### Eliminar Datos

Se agrega el metodo ".pop" que eliminará el dato y regresará al index y el número del dato a eliminar. También se podrá hacer con el metodo “.remove” pero se tendrá que poner el nombre exacto.



#### .pop

```python
cantantes= ["Bad bunny", "Arcangel", "Myke Towers"]
cantantes.pop(1)

print(cantantes)
```



#### .remove

```python
cantantes= ["Bad bunny", "Arcangel", "Myke Towers"]
cantantes.remove("Myke Towers")

print(cantantes)
```



### Invertir la lista

se agregará el metodo “.reverse” para invertir la lista

```python
cantantes= ["Bad bunny", "Arcangel", "Myke Towers"]
cantantes.reverse()

print(cantantes)
```



### Buscar un dato

Para saber si un dato está en la lista se usa print "dato" dentro "in" de la lista “cantantes” en caso de que esté la consola botará un "True"

```python
cantantes= ["Bad bunny", "Arcangel", "Myke Towers"]
print("Arcangel" in cantantes)
```



### Contar los datos

 Le regresa los numeros de objetos en un contenedor.

```python
cantantes= ["Bad bunny", "Arcangel", "Myke Towers"]
print(len(cantantes))
```



### Contar cuantas veces aparece un dato

Con el método “.count" regresa cuantas veces está un dato en la lista.

```python
numeros = [1, 2, 5, 6, 6, 7, 0]
print(numeros.count(6))
```



### Conseguir indice

Para saber en donde está un dato se usa el método “.index” que consigue el indice dentro de las listas.

```python
cantantes= ["Bad bunny", "Arcangel", "Myke Towers"]
print(cantantes.index("Arcangel"))
```



### Unir listas

Las listas se unen con el método “.extend” que añade elementos de otra lista.

```python
cantantes= ["Bad bunny", "Arcangel", "Myke Towers"]
numeros = [1, 2, 5, 6, 6, 7, 0]

cantantes.extend(numeros)
print(cantantes)
```



[Back to top](#Listas o Arrays)