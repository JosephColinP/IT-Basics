

### Crear carpetas

```
import os

#Crear carpeta
if not os.path.isdir("./mi_carpeta"):
    os.mkdir("./mi_carpeta")
else:
    print("ya existe el directorio")
```



### Eliminar carpeta

```python
os.rmdir("./mi_carpeta")
```



### copiar carpeta

```python
import os, shutil

#Crear carpeta
if not os.path.isdir("./mi_carpeta"):
    os.mkdir("./mi_carpeta")
else:
    print("ya existe el directorio")

#Copiar carpeta
ruta_original = "./mi_carpeta"
ruta_nueva = "./mi_carpeta_copiada"

shutil.copytree(ruta_original, ruta_nueva)
```



### listar carpeta

```python
import os, shutil

#Crear carpeta
if not os.path.isdir("./mi_carpeta"):
    os.mkdir("./mi_carpeta")
else:
    print("ya existe el directorio")

#listar contenido
print("Contenido: ")
contenido = os.listdir("./mi_carpeta")
print(contenido)
```





