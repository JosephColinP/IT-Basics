# Control Flow



| Condicionales  | Descripción                                                  |
| -------------- | ------------------------------------------------------------ |
| if             | A block of code is executed, if the condition is ture.       |
| else           | A block of code is executed, if the same condition is false. |
| else if (elif) | A new conidtion is test, if the first condition is false.    |
| switch         | Specify many alternative blocks of code to be executed.      |



## If statement

 ```python
 #True
 color = "rojo"
  
 if color == "rojo":
   print("el color es rojo")
 else:
   print("el color no es rojo")
 
 #False
 color = "Azul"
  
 if color == "rojo":
   print("el color es rojo")
 else:
   print("el color no es rojo")
 
 ```



### if  + input()

```python
color = input("adivina cual es mi color favorito?: ")

if color == "rojo":
  print("Adivinaste")
else:
  print("Ese no es mi color favorito")
```



### if + int(input())

```python
year = int(input("en que año estamos?: "))

#Se mete el codigo int para diferenciar entre un numero y un str

if year >= 2022:
  print("Estamos de 2022 en adelante")
else:
  print("Es un año anterior a 2021")
```



## Ifs Anidados

Se pueden anidar ifs para poder especificar más información en el condicional. 

```python
name = input("Como te llamas?:\n")  
city = input("\nDe que ciudad eres:?\n")
cont = input("\nDe que continente eres?:\n")
age = int(input("\nCual es tu edad?:\n"))
mayoria_edad = 18

if age >= mayoria_edad: 
     print(f"{name} es mayor de edad")  
     if cont != "America":                               
          print(f"{name} no es americano")  
     else:    
         print(f"{name} es americano y de {city}") 
else:
	print (f"{name} no es mayor de edad") 

```

*Note: "Recuerda que al terminar el “if” o el “else” se ponen dos puntos".*



## Elif

Como vemos aquí, else if testea una nueva condición si la primera condición no fue correcta. Para realizar este testeo se necesitan ifs anidados, haciendo así el código más grande. Para evitar esto se utiliza elif.



### Utilizando Ifs anidados

```python
dia = int(input("introduce el número del día de la semana"))

if dia == 1:
    print("es lunes")
else:
    if dia == 2:
        print("es martes")
    else:
         if dia == 3:
            print("es miercoles")

```



### Utilizando elif

```python
#ELIF lo mismo pero sin tanto código

dia = int(input("introduce el número del día de la semana"))

if dia == 1:
    print("es lunes")
elif dia == 2:
    print ("es martes")
elif dia == 3:
    print (" es miercoles")
```



## Bucles

Los bucles son casi lo mismo que los condicionales, la diferencia es que preguntan repititivamente la misma condición.

- [while](#while)
- [do while](#do-while)
- [for](#for)
- [for in](#for-in)
- [for of](#for-of)
- [label](#label)
- [break](#break)
- [continue](#continue)



## while

El bucle while repitirá la misma intrucción si es verdadera hasta que ya no cumpla con la propiedad verdadera.

### Secuencia Condicional

> if condición > verdadera o falsa > ejecutar o no bloque de código.

### Secuencia While

> if condición > verdadera o falsa > ejecutar o no bloque de código > repetir if.



```python
contador = 1
while contador <= 100:
    print(f"estoy en el numero: {contador}")
    contador += 1

```



### Assigment Operator

`+=` is an **assignment** **operator** in Python that adds the right side operand’s value to the left side operand and assigns the result to the left operand.

```python
contador = 1
contador += 1
```

El valor de contador es igual a 1. Entonces al usar += se le agruega el valor de la derecha al contador y se crea un nuevo valor, es decir. 

```py
contador = contador + 1
```



Gracias a este operador se le agregará un 1 en cada loop del bucle. Como definimos "while contador <= 100" el bulce se repetirá hasta llegar a 100





## do while

En el do while, primero se ejecuta el bloque de código y posteriormente se pregunta si la condición se cumple o no.

### Secuencia do while

ejecutar bloque de código > if > condición > verdadera o falsa > volver a ejecutar bloque de código.

### Python do while

En python no existe el do while, pero se puede emular, haciendo que primero realice la acción y posteriormente el loop.

```python
#Syntax

while True:
# statement (s)
If not condition:
break;
```

The test condition is checked first, and if it is true, then the block of statements inside the loop is executed.

```python
#Example

i = 1
while True:
     print(i)
     i = i + 1
     if(i > 5):
     	break; 
```

In this example checks if while is true. So 1 is less than 5 so is true, then proceeds to print (i) and adds a 1. After that while checks again if its true before doing de loop till we reach the number 5, that is not true and stops.



## for

for es similar a el bucle while. Su diferencia es que es un bucle determinado. Los bluces, dependiendo del autor, se pueden clasificar en determinado e indeterminado. 

los bucles while no se le definen cuantas vueltas harán, mientras su condición se cumpla seguirá realizando el bucle. Es por esto que se le clasifica en indeterminado. 

Por el contrario el bucle for es determinado, por lo que se le dice cuantas vueltas dará.



### for in python

El bucle for como tal, no existe en python, sin embargo se utiliza el bucle "for in", que sigue siendo un bucle determinado, es decir, se le asigna primero el número de vueltas que tiene que dar.



## for in

"for in" utiliza arrays en su bucle. A diferencia del bucle "for" donde se especifica la variable, su condición y si aumenta o decrementa. 

En "for in" le especificamos dos variables, la variable "a" que su valor será los datos que se encuentren dentro del "arrary b". 



### "for in" in python

En este caso for in no solo se puede utilizar para arrays si no para tuplas, strings y diccionarios.

```python
# Python program to illustrate
# Iterating over a list
print("List Iteration")
l = ["geeks", "for", "geeks"]
for i in l:
    print(i)
 
# Iterating over a tuple (immutable)
print("\nTuple Iteration")
t = ("geeks", "for", "geeks")
for i in t:
    print(i)
 
# Iterating over a String
print("\nString Iteration")
s = "Geeks"
for i in s:
    print(i)
 
# Iterating over dictionary
print("\nDictionary Iteration")
d = dict()
d['xyz'] = 123
d['abc'] = 345
for i in d:
    print("% s % d" % (i, d[i]))
```



Para hacer que despliege números  como el bucle while se utiliza "range()" que esto es prácticamente un array en el cual se le especifica la cantidad de dígitos que debe contener.



```python
contador = 0

for contador in range (0,5):
    print("voy por el " + str(contador))
```

Esto se traduce como; La variable contador es igual a 0. Luego el for nos dice que la variable contador, será cada uno de los datos o el dato que se encuentre en "range()". El range fue definido del 0 al número 5. Por último imprimirá el número que se encuentra.

Entonces contador igual a 0 se le asigna los valores del range que empieza del 1 entonces imprimirá el 1, posteriormente hará otro loop y se le asigna a la variable contador el nuevo valor de range e imprimirá su nuevo valor que es 2, y así seguirá sucesivamente hasta terminar en el 5. 

Se le indicó al for que diera nadá más 5 vueltas, por lo que al llegar al 5 parará.



## for of

"for of" es lo mismo que "for in" la diferencia está en que en vez de mostrarnos el número de los índices, nos muestra directamente los strings que contiene el array.

Esto no se entenderá en python ya que practicamente "for in" es realmente "for of" en python. a que me refiero.

```python
print("List Iteration")
l = ["geeks", "for", "geeks"]
for i in l:
    print(i)
```

En javascript al ejecutar esto, nos imprimirá los números del 0 al 1, esto porque los arrays empiezan del 0 y este array tiene 3 datos, lo cual nos imprimirá sus indices, es decir geeks = 0, for = 1, geeks = 2.

Pero en python en vez de imprimir los índices, nos imprimirá directamente sus valores.



## break

Nos permite terminar el bucle. Como el ejemplo de do while.

```python
#Example

i = 1
while True:
     print(i)
     i = i + 1
     if(i > 5):
     	break; 
```

En este ejemplo le especificamos que si i es mayor a 5 entonces detendrá el bucle.



## Continue

Al igual que el brake, al especificar cuando parar, este parará, sin embargo a diferencia del break, no terminará el bucle, solo que continuará.

Dando así como resultado, que cuando se le indica donde parar, parará y no mostrará ese número, pero si los siguientes.



```python
# Python program to
# demonstrate continue
# statement

# loop from 1 to 10
for i in range(1, 11):

    # If i is equals to 6,
    # continue to next iteration
    # without printing
	if i == 6:
    	continue
    else:
    	# otherwise print the value
        # of i
        print(i)
```

