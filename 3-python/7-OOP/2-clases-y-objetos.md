# Clases

La clase se puede definir con el comando “class” a esta clase se le pueden ir agregando atributos. Estos atributos antes los conocíamos como variables.

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

# fin de la clase

coche = Coche()
print(coche) #Aquí solo dirá que tienes un clase objeto porque no haz especificado que quieres ver
print(coche.marca, coche.color)
print("velocidad actual: ", coche.velocidad)

coche.acelerar()
print("velocidad actual: ", coche.velocidad)

coche.frenar()
print("velocidad actual: ", coche.velocidad)
```

