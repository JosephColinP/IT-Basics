# Herencia

Posibilidad de compartir atributos y métodos entre clases. Y que diferentes clases hereden de otras.



### MODULO 1

```python
class Persona:

    #Asignar Atributos
    def getNombre(self):
        return self.nombre

    def getApellidos(self):
        return self.apellidos

    def getEdad(self):
        return self.edad

    def getAltura(self):
        return self.altura

    #Asignar un valor
    def setNombre(self, nombre):
        self.nombre = nombre

    def setApellidos(self, apellidos):
        self.apellidos = apellidos

    def setEdad(self, edad):
        self.edad = edad

    def setAltura(self, altura):
        self.altura = altura
    
    #Método (Función)
    def hablar(self):
        return "Estoy Hablando"

    def dormir(self):
        return "Estoy mimiendo"


#Herencia

class Informatico(Persona):
 #El programador a parte de ser persona conoce lenguajes y tiene experiencia

    #Este es un constructor
    def __init__(self):
        self.lenguajes = "HTML, CSS, JavaScript, PHP"
        self.experiencia = 5

    def getLenguajes(self):
        return self.lenguajes

    def aprender(self, lenguajes):
        self.lenguajes = lenguajes
        return self.lenguajes

    def programar(self):
        return "Estoy programando"

    def reparar(self):
        return "Estoy reparando"

"""
Herencia, se puede hacer una clase llamada técico la cual herede 
todas los métodos y atributos de la clase persona y de la clase informático.
"""
class TecnicoRedes(Informatico):

    def __init__(self):
        super().__init__() #Este comando es para cargar al constructor de la clase informatico si no se carga, cuando se quiera accesder a sus datos desde la herencia Tecnico en redes habrá un error y tendrás que asignarlos manualmente
        self.auditarRedes = "Experto"
        self.experienciaRedes = 15

    def auditoria(self):
        return "estoy auditando una red"

```



### MAIN WORKSTATION

```python
import Practica2


#Crear el Objeto Persona
persona = Practica2.Persona()
persona.setNombre("Victor")
persona.setApellidos("Robles")
persona.setAltura("190cm")
persona.setEdad("30 años")

print(f"la persona es: {persona.getNombre()} {persona.getApellidos()}")
print(persona.hablar())
print("--------------------------------\n")

#Crear objeto informático obteniendo herencia de la clase principal

informatico = Practica2.Informatico()
informatico.setNombre("Carlos")
informatico.setApellidos("Martinez")

print(f"El informático es: {informatico.getNombre()} {informatico.getApellidos()}")
print(f"Lenguajes que sabe: {informatico.getLenguajes()}")
print(f"Su experiencia es: {informatico.experiencia} años")
print("--------------------------------\n")

#Herencia del ténico de redes
tecnico = Practica2.TecnicoRedes()
tecnico.setNombre("Manolo")
print(f"El Técnico es: {tecnico.getNombre()}")
print(f"Lenguajes que sabe: {tecnico.getLenguajes()}")
```

