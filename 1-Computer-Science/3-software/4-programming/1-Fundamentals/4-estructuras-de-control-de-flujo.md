# Estructuras de control

Llamaremos estructuras de control a las organizaciones que controlan la ejecución de las acciones en un algoritmo. Las estructuras de control son las que establecen el orden de ejecución de las acciones. Permiten especificar la coordinación yregulacióndelalgoritmo, porque dirigen la dirección que debe seguir el flujo de información en el mismo.



## Condiconales

Los condicionales permiten ejecutar un bloque de código o un context execution, que es el código que va dentro de las llaves. 

```javascript
//Bloqe de código
{
    alert("hola");
    document.write("pedro");
}
```



Las condiccionales nos permiten ejecutar estos bloques de código únicamente si una condición se cumple.

```javascript
if (true){
        alert("Se ejecuta")
}

if (false){
        alert("No se ejecuta")
}
```



Si la condición no se cumple y es falsa, simplemente se saltará el bloque de código y continuará con el siguiente.

| Condicionales | Descripción                                                  |
| ------------- | ------------------------------------------------------------ |
| if            | A block of code is executed, if the condition is ture.       |
| else          | A block of code is executed, if the same condition is false. |
| else if       | A new conidtion is test, if the first condition is false.    |
| switch        | Specify many alternative blocks of code to be executed.      |



```javascript
var jugador = prompt("Como te llamas?");
var manquimetro = prompt("Cuantos kills haces por partida?");

if (manquimetro > 10){
        alert("Eres un crack")
}else if (manquimetro <= 10 && manquimetro >= 4){
        alert("Eres manco, pero te queremos")
}else{
        alert("uninstall")
}
```



_"Note: "if" solo se puede poner uno en la condicional, "else if" se pueden poner varios en caso de que el "if" no cumpla el criterio y  else solo se puede utilizar uno".



## Bucles e Iteraciones

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

 ```javascript
//bucle con if

let numero = 0;
let num = 0;
if (numero < 5){
        numero++;
        numero++;
        numero++;
        numero++;
        numero++;
        document.write(numero + "<br>")
}

//bluce con while
while (num < 5){
        num++;
        document.write(num + "<br>")
}
 ```



## do while

En el do while, primero se ejecuta el bloque de código y posteriormente se pregunta si la condición se cumple o no.

### Secuencia do while

ejecutar bloque de código > if > condición > verdadera o falsa > volver a ejecutar bloque de código.

```javascript
let i = 0;

do {
        i++;
        document.write(i + "<br>")
}       

while ( i < 6)
```



## for

for es similar a el bucle while. Su diferencia es que es un bucle determinado. Los bluces, dependiendo del autor, se pueden clasificar en determinado e indeterminado. 

los bucles while no se le definen cuantas vueltas harán, mientras su condición se cumpla seguirá realizando el bucle. Es por esto que se le clasifica en indeterminado. 

Por el contrario el bucle for es determinado, por lo que se le dice cuantas vueltas dará.

```javascript
// Pasos del bucle for
// Delcaración e Inicialización - "for"
// Condición - "(let i = 0; i < 6;)"
// Aumento o decremento - "(i++)"

for (let i = 0; i < 6; i++){
        document.write(i + "<br>")
} 
```



## for in

"for in" utiliza arrays en su bucle. A diferencia del bucle "for" donde se especifica la variable, su condición y si aumenta o decrementa. 

En "for in" le especificamos dos variables, la variable "a" que su valor será los datos que se encuentren dentro del "arrary b". 

```javascript
let animales = ["gato", "perro", "dinosaurio"];

//Variable "a" Animal
//Variable "b" Animales
for (animal in animales){
        document.write(animal + "<br>")
}
```

En este ejemplo, el bucle "for in"  nos mostrará el indice de cada elemento, es decir gato = 0, perro = 1, y dinosaurio = 2.

Entonces se usa el array animales, el cual tiene datos adentro. Posteriormente se hace el bucle "for in" indicando que la variable "animal" será cada uno de los datos que se encuentran en el array "animales". 

La primera vuelta que de el bucle "for in", arrojará el dato "gato" porque tiene el indice 0, la segunda vuelta que de será "perro" con indice uno y por ultimo, la última vuelta será "dinosaurio" con indice 2.

Para mostrar los nombres y no los indices se tendra que utilizar los corchetes.

```javascript
let animales = ["gato", "perro", "dinosaurio"];

for (animal in animales){
        document.write(animales[animal] + "<br>") //Se utilizan los corchetes con la variable "animal" dentro de estos.
}
```

De esta forma le estamos diciendo que entre al array animales y que nos muestre la variable animal, entonces en su primera vuelta nos mostrará la variable animal con el dato gato, dará su segunda vuelta y cambiará a perro y así sucesivamente.

## for of

"for of" es lo mismo que "for in" la diferencia está en que en vez de mostrarnos el número de los índices, nos muestra directamente los strings que contiene el array.

```javascript
for (animal of animales){
        document.write(animal + "<br>")
}
```



## break

Nos permite terminar el bucle.

```javascript
let i = 0;

while (i < 1000){
        i++;
        document.write(i);
        if(i == 10){
                break;
        }
} 
```

Si no existiera el condicional if con el break, el código contaria hasta mil.



## Continue

Al igual que el brake, al especificar cuando parar, este parará, sin embargo a diferencia del break, no terminará el bucle, solo que continuará.

Dando así como resultado, que cuando se le indica donde parar, parará y no mostrará ese número, pero si los siguientes.

```javascript
for (let i = 0; i < 20; i++){
        if ( i == 12){
                continue;
        }
        document.write(i + "<br>")
}
```

Así en este bucle cuando llegue al 12 lo va a saltar y va a continuar con el bucle.

