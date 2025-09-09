# Visibilidad de atributo



### MODULO 1

```python
class Coche: 
    color = "Negro"
    marca = "Lamborghini"
    modelo = "aventador"
    velocidad = 0
    caballaje = 500
    plazas = 2

    publico="Hola, soy un atributo publico"
    __privado ="Soy un atributo privado"

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



### MAIN WORKSTATION

```python
from Practica import Coche

carro = Coche("Amarillo", "Renault", "Clio", 150, 200, 4)

print("Coche1")
#por atributo
print(carro.getColor())
print(carro.getMarca())
print("")
#Toda la info
print(carro.getInfo())


#Visibilidad
print(carro.publico)
print(carro.__privado)
```

