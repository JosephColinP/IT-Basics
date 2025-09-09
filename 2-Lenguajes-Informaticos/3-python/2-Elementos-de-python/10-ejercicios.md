# Ejercicios



### 1- Crear variables “pais” y “continente”. Mostrar su valor en pantalla y poner un comentario diciendo el tipo de dato

```python
pais = "mexico"         	#string
continente = "america"      #string

print(pais + " " + continente)

```



### 2- Imprimir un rango de número del 1 al 120 únicamente los números pares.

```python
contador = 1
for contador in range(1,121):
   if contador%2 == 0:
       print(contador) 
```



### 3- Escribir un programa que muestre los cuadrados de los 60 primeros números naturales.

```python
contador =0
while contador <=60:
    cuadrado = contador*contador
    print(cuadrado)
    contador +=1

for contador in range (61):
    cuadrado = contador*contador
    print(cuadrado)
```



### 4- Haz que una persona introduzca dos números y estos números hagan todas las operaciones básicas

```py
numero_1 = int(input("introduce primer numero "))
numero_2 = int(input("introduce segundo numero "))

print("Suma: " + str(numero_1+numero_2))
print("Resta: " + str(numero_1-numero_2))
print("Multiplicación: " + str(numero_1*numero_2))
```



### 5- Haz que una persona introduzca dos numeros y muestra el rango entre esos dos numeros.

```python
numero1 = int(input("primer numero "))
numero2 = int(input("segundo numero "))

if numero1 < numero2:
    for contador in range (numero1, numero2):
        print(contador)
else:
    print("el numero 1 debe ser menor al numero 2")
```



### 6- Muestra todas las tablas de multiplicar

```python
for cabecera in range(1, 11):
    print(f"##### tabla del {cabecera} #####")
    print()

    for numero in range (1,11):
        print(f"{numero} x {cabecera} = {numero*cabecera}")
    
    print("\n")
```



### 7- Muestra si un numero es par o in par dentro de un rango elegido por un usuario. 

```python
numnero1 = int(input("introduce un número "))
numnero2 = int(input("introduce el siguiente número "))

if numnero1 < numnero2:
    for x in range(numnero1, (numnero2 + 1)):
        if x%2 == 0:
            print(f"{x} es par")
        else:
            print(f"{x} es impar")

else:
    print("el numero 1 debe ser menor a 2")
```



### 8- haz que el usuario introduzca dos numeros, uno el porcentaje y el otro el numero que se le sacará el porsentaje y muestralo

```python
numero = int(input("introduce el número: "))
porcentaje = int(input("introduce el porcentaje: "))

operacion = (numero * (porcentaje/100))
print(f"el {porcentaje}% de {numero} es {operacion}")
```

















