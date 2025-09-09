# Convertir un tipo de dato a otro

Habrá ciertos momentos donde se requiera convertir un tipo de dato a otro tipo de dato.

Para convertir un dato a otro se utilizan los siguientes códigos: 

1. str(): convierte el dato a string.
2. float(): convierte el dato a un número float.
3. int(): convierte el dato en un número entero.

```python
texto ="Hola"
                                                                      
numero=str(99)
print(texto + " " + numero)
print()
              
numero=float(99)
print(numero)   
print()         

numero=int(99)
print(numero) 
print()
```



Un ejemplo práctico de esto, es cuando se utiliza un input() y el valor introducido es un número, este número siempre será procesado como string, pero si se quiere utilizar para operarlo no se podrá, debido a que un string no puede operarse con un int.



```python
nombre = input("cual es tu nombre?: ")
print(f"me alegro de conocerte, bienvenido {nombre} ")

edad = input("cuantos años tienes?: ")
print(f"Vaya veo que tienes {edad} ")     

trabajo = input("Hace cuantos años fue tu primer trabajo?: ")
print(f"Entonces empezaste a trabajar a tus {int(edad)-int(trabajo)} años")

```

