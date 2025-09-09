# Getters Y Setters

Getters: Saca los datos
Setters: asigna un valor

```python
#El objeto será un carro.
#Clase
#La clase o el molde será un carro.

class Coche: 
#atributos o propiedades
#carácterísticas

  color = "Negro"
  marca = "Lamborghini"
  modelo = "aventador"
  velocidad = 0
  caballaje = 500
  plazas = 2

# Métodos, son acciones que hace el objeto o el coche (Conocidas anteriormente como funciones)

def acelerar(self):
#para acelerar necesita modificar la velocidad de la clase esto se hará con la palabra "self"
  self.velocidad +=1 #aumentará más 1 cada vez que acelere
    
def frenar(self):
  self.velocidad -=1

def getVelocidad(self):
return self.velocidad

#para hacer un getter se puede asignar un método, en este caso Set color para poder interactuar con los atributos de color sin necesidad de modificarlos.
def setColor(self, color):
  self.color = color

# Este método es para sacar el color de las propiedades
def getColor(self):
return self.color

# fin de la clase

coche = Coche()
coche.setColor("Amarillo") #Aquí se cambiaria el color de negro a amarillo


print(coche) #Aquí solo dirá que tienes un clase objeto porque no haz especificado que quieres ver
print(coche.marca, coche.getColor())
print("velocidad actual: ", coche.getVelocidad())

coche.acelerar()
print("velocidad actual: ", coche.getVelocidad())

coche.frenar()
print("velocidad actual: ", coche.getVelocidad())
#Coche.getVelocidad sería getter porque saca el dato, se llama al método para que ellos interactuen con las propiedades, en vez de interactuar directamente con las propiedades
#coche.acelerar seróa el setter por que asigna un valor
```

