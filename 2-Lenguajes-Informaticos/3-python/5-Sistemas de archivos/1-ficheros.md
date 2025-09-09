# Ficheros



## Crear, Abrir y Escribir

```python
from io import open

#Crear archivo, Para abrirlo tendrás que poner toda la dirección de donde se encuentra
archivo = open("fichero_texto.txt", "a+")
```



### Abrir un archivo path absoluto

```python
from io import open
import pathlib

ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo = open(ruta, "a+")
```



### Escribir y close

```python
from io import open
import pathlib

ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo = open(ruta, "a+")

archivo.write("******* Texto Prueba *******")

archivo.close
```



### Leer contenido

```python
from io import open
import pathlib

ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo = open(ruta, "a+")

archivo.write("******* Texto Prueba *******")

archivo.close

#LEER CONTENIDO
ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo_lectura = open(ruta, "r")

contenido = archivo_lectura.read()
print(contenido)

```



### Para leerlo en forma de lista

```python
from io import open
import pathlib

ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo = open(ruta, "a+")

archivo.write("#### SOY UN TEXTO PRUEBA ####\n")
archivo.close

#LEER CONTENIDO
ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo_lectura = open(ruta, "r")

lista = archivo_lectura.readlines()
archivo_lectura.close()

for frase in lista:
    print("- "+frase)
```



### Para Copiar

```python
from io import open
import pathlib
import shutil

ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo = open(ruta, "a+")

archivo.write("#### SOY UN TEXTO PRUEBA ####\n")
archivo.close

#LEER CONTENIDO
ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo_lectura = open(ruta, "r")

lista = archivo_lectura.readlines()
archivo_lectura.close()

for frase in lista:
    print("- "+frase)

#copiar
ruta_original = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
ruta_nueva = str(pathlib.Path().absolute()) + "/fichero_copiado.txt"
shutil.copyfile(ruta_original, ruta_nueva)
```



### Renombrar o mover

```python
from io import open 
import pathlib 
import shutil  

ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt" archivo = open(ruta, "a+")  

archivo.write("#### SOY UN TEXTO PRUEBA ####\n") 
archivo.close 

#LEER CONTENIDO 

ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt" archivo_lectura = open(ruta, "r")  
lista = archivo_lectura.readlines() 
archivo_lectura.close()  
for frase in lista:     
    print("- "+frase)  

#Mover
ruta_original = str(pathlib.Path().absolute()) + "/fichero_texto.txt" ruta_nueva = str(pathlib.Path().absolute()) + "/fichero_Nuevo.txt" shutil.move(ruta_original, ruta_nueva)
```



### Eliminar

```python
from io import open
import pathlib
import shutil

ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo = open(ruta, "a+")

archivo.write("#### SOY UN TEXTO PRUEBA ####\n")
archivo.close

#LEER CONTENIDO
ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo_lectura = open(ruta, "r")

lista = archivo_lectura.readlines()
archivo_lectura.close()

for frase in lista:
    print("- "+frase)

#Eliminar
import os
ruta_nueva = str(pathlib.Path().absolute()) + "/fichero_copiado.txt"
os.remove(ruta_nueva)
```



### Comprobar si existe un archivo

```python
from io import open
import pathlib
import shutil

ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo = open(ruta, "a+")

archivo.write("#### SOY UN TEXTO PRUEBA ####\n")
archivo.close

#LEER CONTENIDO
ruta = str(pathlib.Path().absolute()) + "/fichero_texto.txt"
archivo_lectura = open(ruta, "r")

lista = archivo_lectura.readlines()
archivo_lectura.close()

for frase in lista:
    print("- "+frase)

#Comprobar si existe un archivo
import os.path
if os.path.isfile(os.path.abspath("./") + "/fichero_texto.txt"):
    print("El archivo existe")
else:
    print("el arcivho no existe")
```

