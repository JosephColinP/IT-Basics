# Funciones



- [Estructura](#Estructura)
- [Parámetros](#Parámetros)
- [Parámetros opcionales](#Parámetros opcionales)
- [Return](#Return)
- [Funciones, Parametro, Parametro Opcional y Return](#Funciones, Parametro, Parametro Opcional y Return)
- [Función dentro de otra función](#Función dentro de otra función)
- [Variables globales y Locales](#Variables globales y Locales)
- [Funciones pre-definidas](#Funciones pre-definidas)
- [Curiosidades y Recomendaciones ](#Curiosidades y Recomendaciones )



## Estructura

Una función es un grupo de instrucciones agrupadas bajo un nombre en concreto y pueden utilizarse las veces que se quiera. 

Estructura:

“”
def  "nombre de funcion" (parametros):
			bloque / conjunto de instrucciones.

nombre de funcion (parametro)
“”

Ejemplo:

```python
def muestra_nombres():
    print("Jose")
    print("Paco")
    print("Manue")
    print("Alan")
    print("Viktor")
    print("\n")
muestra_nombres()
```



## Parámetros

Modifican todo el interior de una función

```python
def mostrartunombre(nombre):
    print(f"Tu nombre es: {nombre}")

nombre = input("introduce tu nombre: ")

mostrartunombre(nombre)

###### Doble parametro ###### 

def mostrartunombre(nombre, edad):
    print(f"Tu nombre es: {nombre}")
    
    if edad >= 18:
        print("Eres mayor de edad")
    else:
        print("eres menor de edad")

nombre = input("introduce tu nombre: ")
edad = int(input("introduce tu edad: "))

mostrartunombre(nombre, edad)
```



Otro ejemplo

```python
def tabla(numero):
    print(f"#### TABLA DEL {numero} ####")

    for contador in range (0, 11):
        operacion = numero*contador
        print(f"{numero} x {contador} = {operacion}")
    
    print("\n")
numero= int(input("introduce la tabla de multiplicar que deseas: "))

tabla(numero)
```



## Parámetros opcionales

Es para decidir si un parámetro es obligatorio o no

```python
def empleado(nombre, ine = None):
    print("Empleado")
    print(f"Nombre: {nombre}")

    if ine != None:
        print(f"INE: {ine}")

empleado("Joselito")
```



## Return

Regresa el dato que está adentro de la función.

```python
def saludame(nombre):
    saludo = f"Hola {nombre}"

    return saludo

print(saludame("Joselito"))
```



## Funciones, Parametro, Parametro Opcional y Return

```python
print("###### CALCULADORA ######")

def calculadora(numero1, numero2, basicas = False):

    suma = numero1 + numero2
    resta = numero1 - numero2
    multi = numero1 * numero2
    divi = numero1 / numero2

    cadena =""

    if basicas != False:
        cadena += "Suma: " + str(suma)
        cadena += "\n"
        cadena += "Resta: " + str(resta)
        cadena += "\n"
    else:
        cadena += "Multiplicacion: " + str(multi)
        cadena += "\n"
        cadena += "Division: " + str(divi)

    return cadena
numero1 = int(input("numero 1: "))
numero2 = int(input("numero 2: "))


print(calculadora(numero1, numero2, False))
```



## Función dentro de otra función

Esto sirve para que una sola funcion llame a todas las demás funciones que hagan falta.

```python
def getnombre(nombre):
    texto = f"el nombre es: {nombre}"
    return texto

def getapellidos (apellidos):
    texto = f"los apellidos son: {apellidos}"
    return texto

def devuelvetodo(nombre, apellidos):
    texto = getnombre(nombre) + "\n" + getapellidos(apellidos)
    return texto

print(devuelvetodo("Joselito", "perez"))

```



## Función Lambda

Funciones que no necesitan definirse para tareas pequeñas y repetitivas.

```python
tell_year = lambda year: f"el año es {year}"
print(tell_year(2022))
```





## Variables globales y Locales



### Locales

se definen dentro de la función y no se pueden usar fuera de ella, solo están disponibles dentro. A no ser que hagamos un return.

```python
def varlocal():
    frase = "variable local"
    print(frase)
varlocal()
```



### Globales

Son las que se declaran fuera de una función y están disponibles dentro y fuera de ellas.

```python
frase = "variable global"
print(frase)
```



Si se quiere usar una variable que se encuentra dentro de una función afuera de ella se tiene que utilizar el comando global, ejemplo:

```python
def varlocal():
    frase = "variable local"
    print(frase)

    global ejemplo
    ejemplo = "variable global"

varlocal()

print(ejemplo)
```



## Funciones pre-definidas

```python
Nombre = "Joselito"

# print: imprime el contenido.
print(Nombre)

# type: devuelve el tipo de datos.
print(type(Nombre))

# isinstance: Detecta el tipado
comprobar = isinstance(Nombre, str)
if comprobar: # El if por defecto comprueba si es true.
    print("esta variable es un string")
else:
    print("no es un string")

# strip: limpiar espacios

frase = "           joselito                "
print(frase.strip())

# del: eliminar variable
year = 2021
print(year)
del year

#len: comprobar variable vacia
texto = "joselitooo"
if len(texto) <=0:
    print("la variable estÃ¡ vacia")
else:
    print("la variable tiene contenido: ",len(texto))

#find: encontrar caracteres
frase = "la vida es bella"
print(frase.find("bella"))

#replace: reemplazar palabras
frasenueva = frase.replace("vida", "mujer")
print(frasenueva)

#Lower & Upper: mayusculas y minusculas
print(Nombre)
print(Nombre.lower())
print(Nombre.upper())
```



## Curiosidades y Recomendaciones 

1- Siempre ten las funciones arriba del fichero.

2- Las funciones siempre deben devolver un dato.

```python
def mifuncion():
    return  "hola que tal?"

print(mifuncion())
```



3- Se pueden acceder a variables globales dentro de las funciones aunque se encuentren arriba del fichero. Siempre y cuando el comando de print esté después de las variables definidas.

```python
def mifuncion():
    return  "hola que tal?" + " " + nombre


nombre = "Joselito"

print(mifuncion())
```



4- Las variables deben de tener los valores como parametros salvo que inpriman algo en concreto

```python
def mifuncion(nombre):
    return  "hola que tal?" + " " + nombre


nombre = "Joselito"

print(mifuncion(nombre))

```





[Back to top](#Funciones)
