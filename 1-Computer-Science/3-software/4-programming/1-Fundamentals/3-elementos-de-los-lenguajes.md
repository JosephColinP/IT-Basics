# Elementos de los lenguajes de programación



Para poder realizar en programa existen ciertos elementos básicos los cuales se utilizan para construir sobre ellos un programa. Estos son:

   → Datos. 
   → Variables y constantes.
   → Expresiones.
   → Funciones



## Datos

*Los datos es la información que utilizan los lenguajes de programación para realizar diferentes acciones con la información de los mismos.*

Estos datos se dividen en diferentes tipos o categorías lo que permite a los lenguajes de programación realizar acciones con ellos.



## Tipo de datos



### String (Cadena de Texto)

Todo carácter que esté entre comillas se considera así una cadena de texto, así sea un número.

```python
string = "Cadena de texto"
string2 = "19"
string3 = "true"
 
print(string + "\n",string2 + "\n",string3 + "\n")  

#Terminal
Cadena de texto
 19
 true
```

Cabe mencionar que cuando se le pide un input a un usuario con la variable prompt(), cualquier carácter que introdusca el usuario será transformado en string.



### Number / int

El segundo tipo de datos son los números, estos se definen sin comillas.

```python
num = 12
```



### Float

En algunos lenguajes existen los tipos de datos flotantes, estos indican que son un número decimal.

```python
float = 12.5
```



### Booleano

Boleanos solo son 0s o 1s. Pero se traduce como Ture o False.

```python
bool = true
```



### Undefined

Es una variable la cual no está definida.

```javascript
let num;
alert(num); //undefined
```

Este código nos mostrará en pantalla "undefined", debido a que la variable "num" no está definida.



### Null / None

"Undefined" nos dice que la variable fue creada, pero que no tiene ningún dato guardado.

"null" nos menciona que se creó la variable y dentro de esta existe un dato, este dato que está adentro de la variable, no tiene ningún valor.

```javascript
let nul = null;
```





## Variables y Constantes

Las variables son contenedores de datos los cuales se guardan en la memoria y se pueden utilizar.

```python
recipiente = "papel"
```

Las "variables" se les denominan así porque su contenido puede cambiar.

```python
recipiente = "carton"
```

Para utilizar una variable seleccionamos el nombre que se le fue asignado a la variable y lo asignamos a la acción que queremos hacer.

```python
recipiente = "papel"
print(recipiente)
```

El "print" imprimirá la variable "recipiente" en la terminal, que el valor de la variable es "papel".



### Declarar una variable

Para declarar una variable dependerá del lenguaje de programación que se esté utilizando. Pero por lo general a la variable se le asigna un nombre y posteriormente un valor.

```python
recipiente = "papel"
```

```javascript
var recipiente = "papel";
```

En el ejemplo anterior se puede ver la diferencia entre dos lenguajes de programación, el primero, el cual es python, solo basta con el nombre. En cuanto al segundo se le tiene que especificar el prefijo "var" para indicarle que es una variable.



### Constante

Una constante es una variable la cual el dato que tiene adentro no cambia. Normalmente las variables, al definirlas y darles un dato, se pueden volver a definir y darles otro dato diferente, esto hace que la misma variable pueda cambiar.

```python
recipiente = "Este texto no se verá"
recipiente = "papel"

Print("recipiente")

#Terminal
recipiente
```



Esto puede servir de mucho así como ocasionar problemas, para resolver esto se puede utilizar constantes, las cuales son variables las cuales su dato o valor nunca se modifica. Al igual que las variables su declaración dependerá del lenguaje.



```javascript
var variable = "esto es una variable"
const constante = "esto es una constante"
console.log(variable)
console.log(constante)
```





## Expresiones u Operadores

los operadores son usados para crear instrucciones realizando cálculos matemáticos, comparaciones y operaciones lógicas.

### Operadores Aritméticos

| Operadores | Descripción     |
| ---------- | --------------- |
| +          | Sumar           |
| -          | Restar          |
| /          | Dividir         |
| *          | Multiplicar     |
| %          | Residuo o Resto |
| **         | Exponente       |



### Operadores Relacionales

| Operadores | Descripción       |
| ---------- | ----------------- |
| >          | Mayor que         |
| <          | Menor que         |
| >=         | Mayor o igual que |
| <=         | Menor o igual que |
| ==         | Igual             |



### Operadores Lógicos

| Operadores | Descripción |
| ---------- | ----------- |
| and        | Y           |
| or         | O           |
| not        | No          |
| xor        | Exclusivo   |

