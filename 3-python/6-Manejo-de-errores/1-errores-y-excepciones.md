Este es un codigo suseptible a errores, debido a que si no se introduce un nombre, generará un error en la terminal para el usuario

```python
nombre = input("Cual es tu nombre?: ")

if len(nombre) > 1:
    nombre_usuario = "Nombre: " + nombre

print(nombre_usuario)
```



### Solución

De esta forma botará un texto con el error y no dejará el codigo visible

```python
try:
    nombre = input("Cual es tu nombre?: ")

    if len(nombre) > 1:
        nombre_usuario = "Nombre: " + nombre

    print(nombre_usuario)

except:
    print("ha ocurrido un error, mete bien el nombre")
```



Otras maneras para controlar errores

```python
try:
    nombre = input("Cual es tu nombre?: ")

    if len(nombre) > 1:
        nombre_usuario = "Nombre: " + nombre

    print(nombre_usuario)

except:
    print("ha ocurrido un error, mete bien el nombre")

else:
    print("Funciona correctamente")

finally: 
    print("Fin de la interacción")

```



### Múltiples errores

En este tenemos 2 errores, un type error si no se pone el "int" y un ValueError si cuando se pone “int” el usuario pone un número.

```python
try:
    numero = int(input("Numero para elevarlo al cuadrado: "))
    print("el cuadrado es: "+str(numero*numero))
except TypeError:
    print("Debes convertir tus cadenas a enteros")
except ValueError: 
    print("Introduce un numero")
```



Esta es otra manera en la cual se puede ver el tipo de error

```python
try:
    numero = int(input("Numero para elevarlo al cuadrado: "))
    print("el cuadrado es: "+str(numero*numero))
except TypeError:
    print("Debes convertir tus cadenas a enteros")

except Exception as e:
    print("Ha ocurrido un error: ", type(e).__name__)
```



Excepciones personalizadas

```python
try:
    nombre = input("introduce nombre: ")
    edad = int(input("introduce edad: "))

    if edad < 5 or edad > 110:
        raise ValueError("La edad introducida no es real")
    elif len(nombre) <= 1:
        raise ValueError("El nombre no estÃ¡ completo")
    else:
        print(f"Bienvenido {nombre}")
except ValueError:
    print("Introduce los datos correctamente")
```

