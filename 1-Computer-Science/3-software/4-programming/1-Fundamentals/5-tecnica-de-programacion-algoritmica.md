# Técnicas de programación algorítmica



La elaboración de un algoritmo es totalmente libre, no es necesario seguir ningún modelo o lineamientos. Sin embargo existen ciertos modelos para la programación algorítmica que han sido definidas para el desarollo de un programa.



## Modelo Declarativo

Un modelo de programación declarativa es una forma de escribir código en la cual se especifica lo que se quiere lograr, en lugar de cómo lograrlo. En lugar de especificar los pasos específicos que el programa debe seguir para resolver un problema, se proporciona una descripción abstracta del problema y se deja al compilador o intérprete para resolverlo de la manera más eficiente posible.

Un ejemplo de programación declarativa es la programación funcional. En lugar de usar ciclos y estructuras de control para iterar sobre un conjunto de datos, se utilizan funciones puras y declaraciones de "map", "filter" y "reduce" para describir cómo se quiere transformar un conjunto de datos.



```
print(*range(1,11))
```



En este código, se da a conocer al intérprete el rango de números del 1 al 10, y se utiliza la función print para mostrarlos, dejando al intérprete el trabajo de recorrer el rango y mostrar cada número.



## Modelo Imperativo

El modelo de programación imperativa es una forma de escribir código en la cual se especifican los pasos específicos que el programa debe seguir para resolver un problema. En lugar de proporcionar una descripción abstracta del problema, se proporcionan instrucciones precisas sobre cómo el programa debe manipular datos y cambiar el estado del sistema.

Un ejemplo de programación imperativa es el uso de ciclos y estructuras de control para iterar sobre un conjunto de datos y realizar operaciones específicas en cada iteración.



```
for i in range(1, 11):
    print(i)
```



En este código, se especifica explícitamente cómo se va a recorrer el rango de números del 1 al 10 utilizando un ciclo for, y se especifica cómo se va a imprimir cada número en cada iteración.



## Modelo Orientado a Objetos

La programación orientada a objetos (POO) es un paradigma de programación que se basa en la abstracción de objetos que representan entidades del mundo real y sus relaciones. En POO, un objeto es una instancia de una clase, que es una plantilla para crear objetos con características y comportamientos específicos.

La programación orientada a objetos se caracteriza por tres principios fundamentales: encapsulamiento, herencia y polimorfismo.

- El encapsulamiento se refiere a la ocultación de los detalles de implementación de un objeto detrás de una interfaz pública, de manera que el objeto puede ser utilizado sin conocer su funcionamiento interno.
- La herencia se refiere a la posibilidad de crear una clase a partir de otra clase existente, de manera que la clase nueva hereda las propiedades y métodos de la clase base.
- El polimorfismo se refiere a la capacidad de un objeto de ser tratado como un objeto de una clase base, aun cuando en realidad es un objeto de una clase derivada.

Un ejemplo de programación orientada a objetos en Python podría ser la siguiente clase "Cuenta Bancaria":

```
class CuentaBancaria:
    def __init__(self, titular, saldo):
        self.titular = titular
        self.saldo = saldo

    def depositar(self, monto):
        self.saldo += monto
        print(f"Deposito de {monto} realizado. Nuevo saldo: {self.saldo}")

    def retirar(self, monto):
        if monto > self.saldo:
            print("Saldo insuficiente")
        else:
            self.saldo -= monto
            print(f"Retiro de {monto} realizado. Nuevo saldo: {self.saldo}")

cuenta1 = CuentaBancaria("Juan", 1000)
cuenta2 = CuentaBancaria("Maria", 500)

cuenta1.depositar(100)
cuenta2.retirar(200)

```



En este ejemplo, se define una clase "CuentaBancaria" con dos atributos (titular y saldo) y dos métodos (depositar y retirar) que permiten realizar operaciones en la cuenta. Luego se crean dos objetos de la clase "CuentaBancaria" con titulares y saldos diferentes y se llama a los métodos depositar y retirar de cada uno de ellos.

En este ejemplo se puede ver como se utiliza el encapsulamiento ya que los atributos titular y saldo son privados y solo se pueden modificar mediante los métodos depositar y retirar, también se puede apreciar el polimorfismo ya que a pesar de que cuenta1 y cuenta2 son objetos de la clase "CuentaBancaria" tienen diferentes valores en sus atributos y por lo tanto se comportan de manera diferente al realizar las operaciones depositar y retirar.



## Programación Estructurada

El modelo de programación estructurado es un paradigma de programación que se basa en la organización del código en una serie de bloques estructurados, como funciones y procedimientos, que se ejecutan en orden secuencial. La idea principal es dividir el código en partes pequeñas, fáciles de entender y de testear, para facilitar la lectura y el mantenimiento del código.

Este modelo de programación se caracteriza por ser fácil de entender y seguir, ya que el flujo del código se mantiene en una sola línea, evitando las ramificaciones o llamadas a subrutinas.

Un ejemplo de programación estructurada en Python podría ser el siguiente:

```
def imprimir_numeros():
    for i in range(1,11):
        print(i)

imprimir_numeros()
```



En este ejemplo, se crea una función "imprimir_numeros" que tiene un ciclo for que se encarga de recorrer un rango de numeros del 1 al 10 e imprimirlos, y luego se llama a esa función para ejecutar su contenido. En este ejemplo se puede apreciar la estructuración del código, ya que se separa el proceso de imprimir numeros en una función, facilitando la lectura y el entendimiento del código. Además, al tener esta lógica separada en una función, se puede reutilizar esta lógica en otros lugares del código sin tener que volver a escribir el mismo código.

En resumen, la programación estructurada se enfoca en la organización y estructuración del código, y en la separación de las tareas en bloques de código pequeños y fáciles de entender. Esto ayuda a facilitar la lectura, el mantenimiento y la reutilización del código.



## Otros modelos o paradigmas de la programación



- Programación funcional: Es un paradigma de programación declarativo que se basa en funciones matemáticas y evita el uso de estado y mutabilidad.
- Programación lógica: Es un paradigma de programación declarativo que se basa en la lógica matemática para describir problemas y buscar soluciones.
- Programación concurrente: Es un paradigma de programación que se enfoca en la ejecución simultánea de múltiples tareas y en la sincronización y comunicación entre ellas.
- Programación distribuida: es un paradigma de programación que se enfoca en la ejecución de programas en múltiples sistemas o dispositivos conectados en red, y en la comunicación entre ellos.
- Programación reaccioniva: Es un paradigma de programación que se enfoca en la construcción de sistemas que responden de manera eficiente y escalable a eventos y cambios en el entorno.
- Programación genética: Es un paradigma de programación que se basa en principios de la biología evolutiva para buscar soluciones a problemas complejos de manera automática.

