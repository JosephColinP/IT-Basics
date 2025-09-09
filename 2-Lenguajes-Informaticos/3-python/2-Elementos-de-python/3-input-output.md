# Input / Output



## Input

Input() permite al programa obtener información del usuario.

```python
greet ="Hola"

#Código input
name=input("Please enter your name: ")


```

El input() nos permite guardar datos extraídos del usuario en una variable.



## Output

Para poder ver los datos introducidos en python se utiliza "print(dato a imprimir)" y dentro del print se pasará el dato que se quiera ver.

```python
greet ="Hola"

#Código input
name=input("Please enter your name: ")
print(greet + " " + name)     

```



Habrá diferentes formas de desplegar el output. Por ejemplo si se ponen comillas simples y se escribe dentro, te desplegará el string puesto. a continuación veremos algunos ejemplos de como se puede hacer un print.

```python
name="Juan"

#print string
print("hola")

#print int
print(12)

#print variable
print(name)

#print string concatenada con variable
print("hola" + " " + name)

#print string concatenada con variable utilizando f
print(f"Hola {name}")
```

