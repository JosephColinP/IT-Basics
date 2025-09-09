# Operators



## Operadores de Comparación 

| Operator | Description                                                  | Syntax |
| -------- | ------------------------------------------------------------ | ------ |
| >        | Greater than: True if the left operand is greater than the right | x > y  |
| <        | Less than: True if the left operand is less than the right   | x < y  |
| ==       | Equal to: True if both operands are equal                    | x == y |
| !=       | Not equal to – True if operands are not equal                | x != y |
| >=       | Greater than or equal to True if the left operand is greater than or equal to the right | x >= y |
| <=       | Less than or equal to True if the left operand is less than or equal to the right | x <= y |



### Ejemplos



#### ! (Diferente)

```python
pais = "Rusia"

if pais != "Mexico" or pais != "EspaĆ±a" or pais != "Colombia":
    print (f"{pais} No es un pais de habla hispana")
else:
    print(f"{pais} Es un pais de habla hispana")

```



## Operadores Aritméticos

| Operator | Description                                                  | Syntax |
| -------- | ------------------------------------------------------------ | ------ |
| +        | Addition: adds two operands.                                 | x + y  |
| –        | Subtraction: subtracts two operands.                         | x – y  |
| *        | Multiplication: multiplies two operands.                     | x * y  |
| /        | Division (float): divides the first operand by the second.   | x / y  |
| //       | Division (floor): divides the first operand by the second.   | x // y |
| %        | Modulus: returns the remainder when the first operand is divided by the second. | x % y  |
| **       | Power: Returns first raised to power second.                 | x ** y |



## Operadores Lógicos

| Operator | Description                                        | Syntax  |
| -------- | -------------------------------------------------- | ------- |
| and      | Logical AND: True if both the operands are true    | x and y |
| or       | Logical OR: True if either of the operands is true | x or y  |
| not      | Logical NOT: True if the operand is false          | not x   |



### Ejemplos



#### and (y)

```python
edad_minima = 18
edad_maxima = 65
edad = int(input("introduce tu edad"))

if edad >= 18 and edad <= 65:
    print("esta en edad de trabajar")
else:
    print("no esta en edad de trabajar")
```



#### or (o)

```python
pais = "Rusia"

if pais == "Mexico" or pais == "España" or pais == "Colombia":
    print (f"{pais} es un pais de habla hispana")
else:
    print(f"{pais} no es un pais de habla hispana")
```



#### not (negacion)

```python

pais = "Rusia"

if not pais == "Mexico" or pais == "España" or pais == "Colombia":
    print (f"{pais} no es un pais de habla hispana")
else:
    print(f"{pais} es un pais de habla hispana")
```



## Assigment Operators



| Operator | Description                                                  | Syntax              |
| -------- | ------------------------------------------------------------ | ------------------- |
| =        | Assign value of right side of expression to left side operand | x = y + z           |
| +=       | Add AND: Add right-side operand with left side operand and then assign to left operand | a+=b   a=a+b        |
| -=       | Subtract AND: Subtract right operand from left operand and then assign to left operand | a-=b   a=a-b        |
| *=       | Multiply AND: Multiply right operand with left operand and then assign to left operand | a=a*b               |
| /=       | Divide AND: Divide left operand with right operand and then assign to left operand | a/=b   a=a/b        |
| %=       | Modulus AND: Takes modulus using left and right operands and assign the result to left operand | a%=b   a=a%b        |
| //=      | Divide(floor) AND: Divide left operand with right operand and then assign the value(floor) to left operand | a//=b   a=a//b      |
| **=      | Exponent AND: Calculate exponent(raise power) value using operands and assign value to left operand | a=a**b              |
| &=       | Performs Bitwise AND on operands and assign value to left operand | a&=b   a=a&b        |
| \|=      | Performs Bitwise OR on operands and assign value to left operand | a \|= b a = a \| b  |
| ^=       | Performs Bitwise xOR on operands and assign value to left operand | a^=b   a=a^b        |
| \>>=     | Performs Bitwise right shift on operands and assign value to left operand | a>>=b   a=a>>b      |
| <<=      | Performs Bitwise left shift on operands and assign value to left operand | a <<= b   a= a << b |



## Identify Operators

**is** and **is not** are the [identity operators](https://www.geeksforgeeks.org/python-membership-identity-operators-not-not/) both are used to check if two values are located on the same part of the memory. Two variables that are equal do not imply that they are identical. 

| Operator | Description                            |
| -------- | -------------------------------------- |
| is       | True if the operands are identical     |
| is not   | True if the operands are not identical |

`is` will return `True` if two variables point to the same object, `==` if the objects referred to by the variables are equal.



## Incremento y Decremento

Esto es agregar o disminuir un 1 a un número.



### Incremento

```python
numero = 10
numero = numero + 1
print(numero)
```

### Decremento

```python
numero = 10
numero = numero - 1
print(numero)
```

### Pre-Incremento

```python
numero = 10
numero = 1 + numero
print(numero)
```

### Pre-Decremento

```python
numero = 10
numero = 1 - numero
print(numero)
```

