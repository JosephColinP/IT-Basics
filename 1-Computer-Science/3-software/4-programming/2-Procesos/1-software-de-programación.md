

# Softwares utilizados para la programación



- [Editores de texto](#Editores de texto)
- [Compiladores](#Compiladores)
- [Intérprete](#Intérprete)
- [Pre-procesador](#Pre-procesador)
- [Esamblador](#Esamblador)
- [Cargador y Enlazador](#Cargador y Enlazador)



## Editores de texto


Son programas que permiten crear  y modificar archivos digitales compestos únicamente por texto sin formato, conocidos comúnmente como archivos de texto o texto plano. El programa lee el archivo e interpreta los bytes leídos según el  código de caracteres que usa el editor.



## Compiladores


Un compilador es un programa que traduce un lenguaje de programación a otro lenguaje de programación, usualmente el lenguaje de programación al cual es traducido es el lenuaje de máquina, el cual le facilita a la computadora leer los códigos. De esta manera un programador puede diseñar un programa en un lenguaje mucho más cercano a cómo piensa un ser humano, para luego compilarlo a un programa más manejable por una computadora.



### Partes del compilador

- **Análisis**: Se trata de la comprobación de la correción del programa fuente, e incluye las fases correspondientes al análisis léxico, análisis sintáctico y análisis semántico.
- **Síntesis**: Generación de la salida expresada en un lenguaje objeto y suee estar formado por una o varias combinaciones de fases de generación de código y de optimización de código.
- **Front-end**: Es la parte que analiza el código fuente, comprueba su validez, genera el árbol de derivación y rellena los valores de la tabla de símbolos. Esta parte suele ser independiente de la plataforma o sistema para el cual se vata a compilar, y está compuesta por las fases comprendidas entre Análisis Léxico y la generación de código intermedio.



### Tipos de compiladores

- **Compiladores cruzados:** generan código para un sistema distinto del que están funcionando.
- **Compiladores optimizadores:** realizan cambios en el código para mejorar su eficiencia, pero mantendiendo la funcionalidad del programa original.
- **Compiladores de una sola pasada:** generan el código máquina a partir de una única lectura del código fuente.
- **Compiladores de varias pasadas:** necesitan leer el código fuente varias veces antes de poder producir el código máquina.
- **Compiladores JIT (Just In Time):** forman parte de un intérprete y compilan partes del código según se necesitan.



## Intérprete


Es un programa informático capaz de analizar y ejecutar otros programas escritos en un lenguaje de alto nivel.

La diferencia entre los intérpretes  y los compiladores, es que los intérpretes traducen un programa desde su descripción en un lenguaje de programación al código de máquina del sistema, los intérpretes solo realizan la traducción a medida que sea necesaria, típicamente, instrucción por instrucción, y normalmente no guardan el resutlado de dicha traducción.



## Pre-procesador


Es un traductor cuyo lenguaje fuente es una forma extendida de algún lenguaje de alto nivel, y cuyo lenguaje objeto es la forma estándar del mismo lenguaje. Realiza la tarea de reunir el programa fuente, que a menudo se divide en módulos almacenados en archivos diferentes.



## Esamblador


Traduce el programa en lenguaje ensamblador, creado por el compilador, a código máquina.



## Cargador y Enlazador

Un cargador es un traductor cuyo lenguaje objeto es el código de la máquina real y cuyo lenguaje fuente es casi idéntico. 

Este consiste usualmente en programas de lenguaje máquina en forma reubicable, junto con tablas de datos que especifican los puntos en donde el código reubicable debe modificarse para convertirse en verdaderamente ejecutable. 

Por otro lado, un enlazador es un traductor con los mismos lenguajes fuente y objeto que el cargador.