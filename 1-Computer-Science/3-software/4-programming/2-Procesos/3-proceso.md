# Concepto de proceso



## ¿Qué es un programa?

Es una secuencia de instrucciones escrita.



## Proceso

Un proceso es la instancia de ejecución de un programa.



### Estados de un proceso de ejecución



- **En ejecución:** El proceso ocupa la cpu actualmente, es decir, se está ejecutando.
- **Listo o preparado:** El proceso dispone de todos los recursos para su ejecución. Sólo le falta la CPU
- **bloqueado:** Al proceso le falta algún recurso además de la cpu.



### Otros estados de un proceso

- new (el proceso está siendo creado)
- running ( el proceso se está ejecutando)
- wating (está esperando que se cumpla algun otro evento)
- ready (está pronto para ejecutar esperando a la CPU)
- terminated (el proceso a sido terminado)



### Los procesos pueden dividirse en dos tipos



#### Activos

Son aquellos que compiten con el procesador o están en condicoines de hacerlo.

- Ejecución: Estado en el que se encuentra un proceso cuando tiene el control del procesador

- Preparado: Aquellos procesos que están dispuestos para ser ejecutados, pero no están en ejecución por alguna causa.

- bloqueado: Son los procesos que no pueden ejecutarse de momento por necesitar algún recurso no disponible.

  

#### Inactivos

Son aquellos que no pueden competir por el procesador, pero que pueden volver a hacerlo por medio de ciertas operaciones.

- Suspendido Bloqueado: Es el proceso que fue suspendido en espera de un evento, sin que hayan desaparecido las causas de su bloqueo. 
- Suspendido programado: Es el proceso que han sido suspendido, pero no tiene causa para estar bloqueado.



### Creación de procesos

Crear un proceso implica operaciones como:

- Dar un nombre a un proceso.
- Insertarlo en la lista de procesos conocidos del sistema.
- Determinar la prioridad incial de proceso.
- Crear el bloque de control de proceso.
- Asignar los recursos iniciales al proceso.



## Operaciones de procesos y recursos

Los sistemas operativos poseen una serie de funciones cuyo objetivo es el de la manipulación de procesos.



- **Crear el proceso:** Se produce con la orden de ejecución del programa y suele necesitar varios argumentos, como el nombre y la prioridad del proceso.
- **Jerárquica:** En este, cada proceso que se crea es hijo del proceso creador y hereda el entorno de ejecucción de su padre.
- **No jerarquico:** Cada proceso creado por otro proceso se ejecuta independientemente de su creador con un entorno diferente. Ademas los dos tipos  anteriores pueden realizar las operaciones siguientes:
  - Destruir un proceso: Se trata de la orden de eliminación del proceso con la cual el sistema operativo destuye su PCB
  - Suspender un proceso: Es una operacon de alta prioridad que paraliza un proceso que puede ser renaudado posteriormente.



## Descriptor de procesos y recursos

Un descriptor de procesos y recursos es una estructura de datos asociada a una entidad informática ya sea un recurso o proceso, en la cual se indica y actualiza todas las informaciones relativas a dicha entidad. 










