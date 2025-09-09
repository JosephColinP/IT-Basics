# Paquetes

Son conjunto de módulos.  Para crear un paquete se tiene que hacer un carpeta con los módulos y el archivo del paquete, el nombre del archivo del paquete debe de llamarse :

```
__init__.py
```



#### 1er Archivo (Módulo1)

```python
def probando():
    print("esto es una prueba de un módulo de un paquete")
```



#### 2do Archivo (Módulo2)

```python
def nombreCompleto(nombre, apellidos):
    print(f"{nombre}{apellidos}")
```



#### Archivo principal

```python
from Paquete import Modulo
from Paquete import Modulo2

Modulo.probando()
Modulo2.nombreCompleto("Jose", "Torres")
```



#### INSTALAR PAQUETES 

Para instalarlos se puede utilizar la siguiente página: https://pypi.org