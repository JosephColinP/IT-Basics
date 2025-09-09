# FUNDAMENTALS



- [1. Concepto Básico de Computadoras y Comunicación](#1. Concepto Básico de Computadoras y Comunicación)
  - [1.1 Comunicación de una PC](#1.1 Comunicación de una PC)
    - [1.1.1 Código Binario](#1.1.1 Código Binario)
    - [1.1.2 Logic Gates](#1.1.2 Logic Gates)
- [2. Software](#2. Software)
  - [2.1 Concepto General de Software](#2.1 Concepto General de Software)
  - [2.2 System Software](#2.2 System Software)
  - [2.3 Application Software](#2.3 Application Software)
  - [2.4 Tipos de Software Específicos](#2.4 Tipos de Software Específicos)
- [3. Programación](#3. Programación)
  - [3.1 Concepto de Programación](#3.1 Concepto de Programación)
  - [3.2 Lenguajes de Programación](#3.2 Lenguajes de Programación)
  - [3.3 Tipos de Programación](#3.3 Tipos de Programación)



## 1. Concepto Básico de Computadoras y Comunicación



### 1.1 Comunicación de una PC



#### 1.1.1 Código Binario

- **Definición**: El código binario es el lenguaje fundamental que utiliza una computadora. Está compuesto por valores "0" y "1", conocidos como "Bits". Este sistema binario forma la base de todo el procesamiento y transferencia de datos en sistemas de cómputo modernos.
- **Bytes y Character Encoding**: Un byte está compuesto por 8 bits, lo que significa que hay 256 combinaciones posibles en un solo byte. Los sistemas de codificación de caracteres, como ASCII y UTF-8, traducen estas combinaciones binarias en caracteres que los humanos pueden entender. ASCII utiliza una sola codificación de byte, mientras que UTF-8 puede variar de 1 a 4 bytes, permitiendo una representación más rica de caracteres (referencia: [Unicode Consortium](https://www.unicode.org/)).
- **Funcionamiento**: La lógica binaria se utiliza en el corazón de las computadoras. Si hay una señal eléctrica, se representa como 1, y si no hay señal, se representa como 0. Estos valores se manipulan a través de componentes como transistores y Logic Gates para realizar operaciones lógicas.



#### 1.1.2 Logic Gates

- **Definición**: Las compuertas lógicas son componentes fundamentales en electrónica digital. Utilizan la lógica binaria para controlar el flujo de corriente eléctrica. Las puertas más comunes son AND, OR, NOT, NAND, NOR, XOR, y XNOR. Cada una de ellas realiza una operación lógica específica basada en sus entradas y produce una salida correspondiente. (Referencia: M. Morris Mano, "Digital Design").



## 2. Software



### 2.1 Concepto General de Software

- **Definición**: El software es el componente intangible que opera en hardware de computadora. Incluye todo, desde sistemas operativos hasta aplicaciones y datos. Es la manifestación de algoritmos y estructuras de datos que permiten a las computadoras realizar tareas complejas.
- **Tipos de Software**: El software puede ser categorizado en *System Software*, que incluye sistemas operativos y utilidades, y *Application Software*, que son programas específicos diseñados para el usuario final.



### 2.2 System Software

- **Definición**: El software de sistema es esencial para administrar y controlar el hardware de la computadora, facilitando así un entorno en el que el software de aplicación pueda funcionar. Los ejemplos notables incluyen sistemas operativos como Windows, macOS, Linux (referencia: A. Silberschatz, P. B. Galvin, G. Gagne, "Operating System Concepts").



### 2.3 Application Software

- **Definición**: El software de aplicación se desarrolla para permitir a los usuarios realizar tareas específicas. Puede variar desde procesadores de texto hasta navegadores web y juegos. Está diseñado con la interacción del usuario en mente.



### 2.4 Tipos de Software Específicos

- **Comercial**: Software vendido a los consumidores.
- **Open Source**: Software con código fuente accesible y modificable (referencia: E. Raymond, "The Cathedral and the Bazaar").
- **Application software**: Creado para satisfacer necesidades específicas.
- **System software**: Mantener el sistema central en funcionamiento.
- **Firmware**: Software incorporado en un componente de hardware.



## 3. Programación



### 3.1 Concepto de Programación

- **Programación:** La programación es el proceso de diseñar e implementar un conjunto estructurado de instrucciones para que una computadora realice una tarea específica o resuelva un problema determinado.
- **Programa**: Son instrucciones procesadas por la computadora, creadas mediante lenguajes de programación.
- **Ejecutables**: Archivos que consisten en instrucciones traducidas a código máquina.
- **Compilación**: Proceso de traducir el código de alto nivel al lenguaje máquina.



### 3.2 Lenguajes de Programación


Los lenguajes de programación son medios a través de los cuales los programadores expresan instrucciones que las computadoras pueden ejecutar. Estos lenguajes se clasifican en diferentes categorías según su nivel de abstracción y su cercanía al hardware.



#### 3.4.1 Assembly Language (Lenguaje Ensamblador)

- Definición: El lenguaje ensamblador es un tipo de lenguaje de programación de bajo nivel utilizado para programar directamente el hardware.
- Uso: A menudo se usa para tareas críticas en tiempo y en sistemas embebidos donde se necesita un control directo del hardware.
- Relación con otros lenguajes: Es un paso por encima del código máquina, y cada instrucción en ensamblador generalmente se traduce directamente en una instrucción en código máquina.



#### 3.4.2 High-Level Programming Languages (Lenguajes de Programación de Alto Nivel)

- Definición: Los lenguajes de programación de alto nivel son más abstractos y alejados del hardware. Están diseñados para ser más fáciles de leer y escribir.
- Uso: Se utilizan en la mayoría de las aplicaciones de software modernas, desde sistemas operativos hasta aplicaciones web y móviles.
- Relación con otros lenguajes: Los lenguajes de alto nivel se compilan o interpretan en lenguajes de bajo nivel, como el ensamblador o el código máquina, antes de ser ejecutados.
- Ejemplos: Java, Python, C++, etc.



### 3.4.3 Scripting Languages (Lenguajes de Script)

- Definición: Los lenguajes de script son tipos de lenguajes de programación de alto nivel que se utilizan para automatizar tareas o controlar aplicaciones.
- Uso: A menudo se utilizan para tareas rápidas y automatización, o para agregar funcionalidades en aplicaciones web.
- Relación con otros lenguajes: Como lenguajes de alto nivel, también son más abstractos que el ensamblador, pero generalmente se enfocan más en la facilidad de uso y la eficiencia en el desarrollo.
- Ejemplos: JavaScript, Perl, Ruby, etc.



### 3.3 Tipos de Programación



- **Programación Estructurada:** Utiliza una metodología lógica y estructurada para escribir código, facilitando su comprensión y mantenimiento. El código se divide en bloques o funciones, y se evita el uso de la instrucción GOTO, favoreciendo así un flujo de control más predecible y ordenado.



- **Programación Orientada a Objetos (POO):** Utiliza "objetos", que encapsulan datos y comportamientos, promoviendo la reutilización de código y la modularidad. Esto ayuda a que los sistemas sean más escalables y mantenibles (referencia: E. Gamma, R. Helm, R. Johnson, J. Vlissides, "Design Patterns").



- **Programación Orientada a Protocolos (POP):** Este enfoque se centra en la definición de protocolos o interfaces claros para comunicarse entre diferentes partes de un programa o sistema. Los protocolos establecen reglas y expectativas para la interacción, lo que permite que diferentes partes del sistema trabajen juntas de manera más cohesiva y flexible. En grandes proyectos de software y sistemas distribuidos, la POP puede ser crucial para garantizar que todo el sistema funcione de manera uniforme y eficiente.

  La Programación Orientada a Protocolos a menudo se usa en combinación con otros paradigmas de programación para crear una estructura de código robusta y fácil de mantener. Su enfoque en la comunicación y las interfaces claras lo convierte en una opción popular en entornos donde la colaboración y la interoperabilidad son clave.



[Back to top](#FUNDAMENTALS)
