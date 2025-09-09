# Recursión



La recursión o recursividad es un concepto amplio, con muchas variantes, y difícil de precisar en pocas palabras.

Un objeto recursivo es aquel que aparece en la definición de sí mismo, así como el que se llama a sí mismo. La recursión se pede presentar de dos maneras diferentes:

- **Directa:** El programa o subprograma se llama directamente a sí mismo.
- **Indirecta:** El subprograma llama a otro subprograma, y éste, en algún momento, llama nuevamente al primero.

En toda la definición recursiva de un problema se deben establecer dos pasos; el paso básico y el paso recursivo. El primero, uno o varios, dependiendo de el problema, se utiliza como condición de parada o fin de la recursividad. A éste llegamos uando encontramos la solución del problema o cuando decidimos que ya no vamos a seguir. 

El segundo paso, propicia la recursividad. Se puede presentar uno o varios dependiendo del problema a resolver.

Cuando se analiza la solción recursiva de un problema es importante determinar con precisión cuáles serán los pasos básicos y recursivos. Es importante que cada vuelta del ciclo avancemos al final poco a poco, si esto no sucede, estaremos dentro de un ciclo extraño el cual será un problema que estará mal definido, en este caso la máquina se podría quedar ejecutandose durante un tiempo indefinido y se agotaría la memoria.





