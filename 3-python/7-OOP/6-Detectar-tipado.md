# Detectar tipado

El método de contructor, es un método especial dentro de una clase y se utiliza para darle un valor a los atributos del objeto al crearlo.



### Módulo 1

```python
class Coche: 
    color = "Negro"
    marca = "Lamborghini"
    modelo = "aventador"
    velocidad = 0
    caballaje = 500
    plazas = 2

#Constuctor

    def __init__(self, color, marca, modelo, velocidad, caballaje, plazas):
        self.color = color
        self.marca = marca
        self.modelo = modelo
        self.velocidad = velocidad
        self.caballaje = caballaje
        self.plazas = plazas

    #Asigna el color
    def setColor(self, color):
        self.color = color

    #Devuelve el color
    def getColor(self):
        return self.color

    #Asigna la marca
    def setMarca(self, marca):
        self.marca = marca

    #Devuelve la marca
    def getMarca(self):
        return self.marca

     #Asigna el modelo
    def setModelo(self, modelo):
        self.modelo = modelo

    #Devuelve el modelo
    def getModelo(self):
        return self.modelo



    def getInfo(self):

        info = "### InformaciĆ³n del coche ###"
        info += "\n color: " + self.getColor()
        info += "\n Marca: " + self.getMarca()
        info += "\n Modelo: " + self.getModelo()

        return info
```



### Main workstation

```python
from Practica import Coche

carro = Coche("Amarillo", "Renault", "Clio", 150, 200, 4)

#Detectar tipado
if type(carro) == Coche:
    print("Es un objeto correcto")
else:
    print("No es un objeto correcto")

```

