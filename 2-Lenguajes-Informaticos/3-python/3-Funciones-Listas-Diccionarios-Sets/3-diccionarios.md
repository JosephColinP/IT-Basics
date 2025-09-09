# Diccionarios y sets



- [Sets](#Sets)
- [Diccionario](#Diccionario)



## Sets

Son una colección de datos, para tener una colección de valores, pero que no tienen un orden o un indice.

```python
personas = {
    "Alan",
    "Dave",
    "Jose"
}

print(type(personas))
print(personas)

```



### Agregar elemento

Para agregar un índice se puede utilizar el método “.add” e indicar cual índice será añadido.

```python
personas = {
    "Alan",
    "Dave",
    "Jose"
}

personas.add("Pepe")

print(type(personas))
print(personas)
```



### Remover Elemento

Para remover un indice se puede utilizar el método “.remove” e indicar cual será removido.

```python
personas = {
    "Alan",
    "Dave",
    "Jose"
}

personas.add("Pepe")
personas.remove("Jose")

print(type(personas))
print(personas)
```





## Diccionario

Es un tipo de dato que almacena un conjunto de valores, en vez de tener índices numéricos, almacena índices alfanuméricos. Es parecido a un array asociativo o un objeto json.

```python
personas = {
    "Nombre": "Victor",
    "Apellidos": "Robles",
    "Web": "Victorrobles.es"
}

print(type(personas))
print(personas)
```



### Acceder a un indice en específico 

Se utilizará el valor, “personas” posteriormente entre corchetes se pone el indice al cual se quiere acceder “Nombre”.

```python
personas = {
    "Nombre": "Victor",
    "Apellidos": "Robles",
    "Web": "Victorrobles.es"
}

print(type(personas))
print(personas["Nombre"])
```



### Diccionario dentro de listas

Las listas se utilizan con corchetes, sin embargo, dentro de estas se pueden poner diccionarios con llaves.

```python
contactos = [
    {
        "nombre": "Antonio",
        "email": "Antonio@gmail.com"
    },   
    {
        "nombre": "Juan",
        "email": "Juan@gmail.com"
    },
    {
        "nombre": "Pedro",
        "email": "Pedro@gmail.com"
    }
    
]

print(contactos)
```



### Seleccionar un dato en específico

Para seleccionar un dato en específico se pone entre corchetes el número de diccionario al cual se quiere acceder “0” y al índice el cual se quiere acceder “nombre”.

```python
contactos = [
    {
        "nombre": "Antonio",
        "email": "Antonio@gmail.com"
    },   
    {
        "nombre": "Juan",
        "email": "Juan@gmail.com"
    },
    {
        "nombre": "Pedro",
        "email": "Pedro@gmail.com"
    }
    
]

print(contactos[0]["nombre"])
```



### Seleccionar varios valores

Para seleccionar varios valores se puede utilizar el "for" para “contacto” adentro irán "contactos" posteriormente a esto se puede seleccionar la variable “contacto” y entre corchetes seleccionar el índice.

```python
contactos = [
    {
        "nombre": "Antonio",
        "email": "Antonio@gmail.com"
    },   
    {
        "nombre": "Juan",
        "email": "Juan@gmail.com"
    },
    {
        "nombre": "Pedro",
        "email": "Pedro@gmail.com"
    }
    
]

print("\nLista de contactos: ")

for contacto in contactos:
    print(f"Nombre del contacto: {contacto['nombre']}")
    print(f"Email del contacto: {contacto['email']}")
    print()
```



[Back to top](#Diccionarios y sets)



