# Conceptos Fundamentales



- [¿Que es la Programación?](#¿Que es la Programación?)
- [Algoritmos](#Algoritmos)
  - [Representación de algoritmos](#Representación de algoritmos)
- [Lenguajes de programación](#Lenguajes de programación)
- [Programa](#Programa)



## ¿Que es la Programación?

*"La programación es la creación de aplicaciones informáticas, valiéndose de distintas herramientas, para la resolución de un problema".*

Para poder programar o crear una aplicación primeramente se necesita un **problema** a resolver. Se necesita analizar y determinar el objetivo del programa. Una vez hecho lo anterior se necesita un plan de acción que nos diga paso a paso como resolver el problema. Esto es el **algoritmo**. El algoritmo es un conjunto de pasos, instrucciones o acciones que se deben seguir para resolver un problema.

Una vez encontrado el problema y realizado el algoritmo, este último se tiene que traducir a un **lenguaje de programación**, para convertir el algoritmo en un **programa** que será interpretado por una computadora para resolver un problema.

En resumen, para programar se tiene que identificar el problema, posteriormente realizar un algoritmo para su resolución, plasmar este algoritmo en un lenguaje de programación para que este algoritmo se convierta en un programa y pueda ser utilizado por una computadora y así solucionar el problema.



## Algoritmos

*"Un algoritmo es una forma de describir la solución de un problema, explicando paso a paso como se debe proceder para llegar a una respuesta encuadrada a los datos disponibles, en un* tiempo finito".*



### Características

Los algoritmos deben ser precisos, es decir, deben explicar sin ambigüedades que es lo que realizarán. Deberán ser exactos, estos deberán arrojar la misma solución sin importar las veces que sean repetidos.  Por último deberán ser finitos, deben de tener un tiempo finito de ejecución.



### Problemas Algorítmicos

Son aquellos cuya solución puede expresarse mediante un algoritmo. Deben de cumplir las características de un algoritmo, deberán ser precisos, exactos y finitos.  

En caso de no cumplir estas características, entonces no serán considerados problemas algorítmicos, como por ejemplo; escribir todos los números enteros empezando desde el 1. Este problema no es algorítmico porque no es finito.



### Representación de algoritmos

No existe un lenguaje único y universal para escribir algoritmos. Cada lenguaje tiene una sintaxis
determinada, un grupo finito de elementos que ayudan a representar los algoritmos, y una
semántica asociada a la sintaxis, la cual se refiere al concepto que se representa.

Existen dos tipos de representaciones: la gráfica (mediante dibujos) y la no gráfica (mediante
textos). Los métodos usuales para representar algoritmos son:

1. Diagrama de flujo
2. Diagrama de Nassi Schneiderman (comúnmente denominado Diagrama de Chapin)
3. Pseudocódigo
4. Lenguaje natural
5. Fórmulas

Los dos primeros son formas gráficas de representación, mientras que los últimos son no
gráficas.



### PseudoCódigo

La palabra pseudocódigo tiene toda su explicación en el prefijo "pseudo", que significa "falso". Esto quiere decir que no es un código real.

El pseudocódigo es el paso intermedio entre el algoritmo y escribir el programa. Es decir, es la descripción paso a paso de lo que se tiene que hacer el programa antes de realmente escribirlo.

No existe una sintaxis del pseudocógido, este se puede escribir a conveniencia del programador. 



#### Ejemplo con un problema:

Juan tiene un examen de geometría y quiere hacer una calculadora para sacar el área de un triángulo para ahorrarse tiempo.



**Pseudocodigo:**

- Escribir("ingresar la altura del triángulo")
- Escribir("ingresa la base del triángulo"
- Operación = base * altura / 2
- Escribir("El área del triángulo es: ")



**Código:**

```python
  1  
  2 altura = int(input("¿Cuál es la altura del triángulo?\n: "))
  3 base = int(input("¿Cuál es la base del triángulo?\n: "))
  4 operacion = base * altura / 2
  5 print(f"El área del triángulo es: {operacion}")
  6

	#Terminal
    El área del triángulo es: 16.0
 
```









## Lenguajes de programación

Una vez hecho el algoritmo, este se tiene que realizar en un lenguaje de programación. Para así finalmente crear un programa que de con la solución del problema.

*"Lenguaje de programación es un conjunto de símbolos (sintaxis) y reglas (semántica) que permite expresar programas".*

Un lenguaje de programación es básicamente un sistema estructurado de comunicación, conformado por conjuntos de palabras clabes, símbolos y reglas sintáctocas y semánticas que permiten un entendimiento entre programador y la máquina.

Debemos distinguir entre lenguaje de programación y lenguaje informático. Todos los lenguajes de programación son a la vez informáticos, pero no todos los lenguajes informáticos son de programación. Por ejemplo como sucede con el HTML, que es un lenguaje de maquetación web, pero no de programación.

Un lenguaje de programación está compuesto por una serie de instruccones, que tras introducirlas en una máquina, se traducirán en una consecución de operaciones ejecutadas por dicho equipo.



## Programa

*"Un programa es un conjunto de acciones que puede entender y ejecutar una computadora."*

Para llegar a hacer un programa es necesario el diseño previo del algoritmo. Esto es, representar la solución del problema en un lenguaje natural, en el cual se expresan las ideas diariamente.

