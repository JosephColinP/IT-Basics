# Curiosidades extras de strings y variables en Python



### Creación de variables

Al crear una variable no se puede iniciar con números ni tampoco se pueden utilizar caracteres raros como signos.



### Comillas dentro de un Str

Para utilizar comillas dentro de los strings se pueden hacer de la siguiente forma.

```python
texto = """ Master en "python" """
texto = " Master en 'python' "
texto = " Master en \"python\" "
```



### Creación de espacios entre strings concatenados

Para crear espacios dentro de una concatenación se puede utilizar las comillas y un espacio.

```python
name = "Joseph"
greeting = "Hola"
print(greeting + " " + name)
```



### Split string

El código \n hará un espacio aparte en el string.

```python
#Código \n
splitstring = ("Hola\n¿Cómo estas?")
print(splitstring)
print()
```

También se podrá separar los strings por medio de triple comillas

```python
# Otra manera de dividir los strings
anothersplitstring = """Hola
¿Cómo estás?"""
print(anothersplitstring)
print()
```



### Tab en strings

El código \T generará un tab en el string.

````python
#Código \t
tabbedstring = "1\t2\t3\t4"
print(tabbedstring)
print()
````



### Selección de carácteres específicos

 Para seleccionar un carácter específico se podrá poner corchetes y el número del carácter.

```python
# caracteres específicos
parrot = "Peppa Pig"
print(parrot)
print(parrot[3])
```



### Borrar una parte anterior del string

para esto se utilizará el comando \r para poder borrar el texto anterior de un string.

```python
texto1 = "Master"
texto2 = "Python"
texto_unido = texto1 + "\r " + texto2
 
print(texto_unido)
```





