# Procesos e hilos



El concepto de proceso engloba dos conceptos separados y potencialmente independientes: uno relativo a la propiedad de recursos y otros que hace referencia a la ejecución. 



## Unidad que posee recursos

A un proceso se le asigna un espacio de memoria y, de tanto en tanto, se le puede asignar otros recursos como dispositivos de I/O o ficheros.



## Unidad a la que se le asigna el procesador

Un proceso es un flujo de ejecucuión (una taza) a través de uno o más programas.



## Poceso vs hilo

proceso es una entidad relativamente independiente que dispone de su propio espacio de direcciones, su propia información de estado y que utiliza los mecanismos de comunicación entre procesos que le proporciona el sistema operativo para comunicarse con otros procesos.

Hilo es un programa en ejecución que comparte la imagen de la memoria y otras informaciones con otros procesos ligeros o hilos.

Los procesos ligeros son una unidad básica de utilizacion de la CPU consiste en un juego de registros y un espacio de pila. Comparte el código, los datos y lso recursos con sus hebras pares.
   → Una tarea está formada ahora por una o más hebras.
   → Una hebra sólo puede pertenecer a una tarea.



## Características

   → Se comparten recursos
   → La compartición de la memoria permite a las hebras pares comunicarse sin usar. ningún mecanismo de comunicación inter-proceso del S.O.
   → La conmutación de contexto es más rápido gracias al extenso compartir de recursos.
   → No hay protección entre las hebras.
   → Una hebra puede escribir en la pila de otras hebra del mismo proceso.