# Módulos



- [Tipos de Módulos](#Tipos de Módulos)



Módulos son funcionalidades ya hechas para reutilizar. Se puede conseguir predeterminados en el lenguaje, modulos hechos en internet o crearlos tu mismo.

Para crear un módulo simplemente se abrirá un archivo .py se realizará la linea de comandos y en tu linea de comandos principal se pondrá “import” y nombre del módulo.



#### Módulo 1

```python
def hola(nombre):
    return f"Hola, como estás? {nombre}"
```



##### Programa principal

```python
import Modulo
print(Modulo.hola("Jose"))
```



### Importar una variable a un módulo con varias variables.



#### Módulo 1

```python
def hola(nombre):
    return f"Hola, como está? {nombre}"

def holamundo(name):
    return f"Hello, How are you? {name}"
```



##### Programa Principal

```python
from Modulo import holamundo

print(holamundo("Robles"))
```



*Note: “Si existe un error de (No se puede importar) puede que simplemente tengas que guardar y abrir y cerrar de nuevo el visual studio".*



### Importar todas las variables



#### Módulo 1

```python
def hola(nombre):
    return f"Hola, como está? {nombre}"

def holamundo(name):
    return f"Hello, How are you? {name}"
```



##### Programa Principal

```python
from Modulo import *

print(hola("Jose"))
print(holamundo("Joseph"))
```



## Tipos de Módulos



### Módulo de fechas

El modulo de fechas viene por defult y nos dice la fecha, en este caso se accede con “import datetime" y para imprimir  la fecha "date.date.today()"

```python
import datetime

print(datetime.date.today())
```



Para sacar la fecha completa se puede utilizar el comando “datetime.datetime.now”

```python
import datetime

fecha = datetime.datetime.now()

print(fecha)
```



Para sacar un dato en específico se puede indicar en el print que dato se quiere sacar.

```python
import datetime

fecha = datetime.datetime.now()


print(fecha.year)
```



Para personalizar tu fecha lo haces con el codigo “.strftime” y entre parentesis indicas que queires que se muestre.

```python
import datetime

fecha = datetime.datetime.now()

fecha_personalizada = fecha.strftime("%d/%m/%Y, %H:%M:%S")
print(fecha_personalizada)
```



### Modulo de matemáticas 

Para importar el módulo se tiene que utilizar el comando “import” y el módulo “math”.

```python
import math
```



#### Módulo de Ríz cuadrada

```python
print("Raiz cuadrada de 10: ", math.sqrt(10))
```



#### Módulo de po

```python
print("Numero pi: ", float(math.pi))
```



#### Módulo de redondear hacia arriba

```python
print("redondear: ", math.ceil(6.2345257211345143))
```



#### Módulo de redondeo hacia abajo

```python
print("redondear: ", math.floor(6.2345257211345143))
```



#### Módulo Random

Es un módulo aparte, nos permite poner números aleatorios.

```python
import random

print("numero aleatorio entre 15 y 67: ", random.randint(15, 67))
```



[Back to top](#Módulos)