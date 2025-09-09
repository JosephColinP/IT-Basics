# Constructor

El método de contructor, es un método especial dentro de una clase y se utiliza para darle un valor a los atributos del objeto al crearlo.



### MODULO 1

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



### MAIN WORKSTATION

```python
from Practica import Coche

carro = Coche("Amarillo", "Renault", "Clio", 150, 200, 4)
carro2 = Coche("Verde", "Seat", "Panda", 150, 200, 4)
carro3 = Coche("Azul", "Citroen", "Xara", 150, 200, 4)

print("Coche1")
#por atributo
print(carro.getColor())
print(carro.getMarca())
print("")
#Toda la info
print(carro.getInfo())

print("")
print("Coche2")
#por atributo
print(carro2.getColor())
print(carro2.getMarca())
print("")
#Toda la info
print(carro2.getInfo())

print("")
print("Coche3")
#por atributo
print(carro3.getColor())
print(carro3.getMarca())
print("")
#Toda la info
print(carro3.getInfo())
```





