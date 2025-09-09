# Buses

El bus es un medio de transmisión compartido que interconecta dos o más dispositivos en un sistema.  

## Constitución

Esta constituido por un conjunto de lineas que son conductores eléctricos que están compartidos por todos los dispositivos.  

## Bus del sistema

Conecta el procesador “CPU” con la memoria principal, de manera que gestiona la transferencia de datos y las instrucciones entre los dos componentes.  

## Modo de Operación

##### Elementos implicados en una transferencia

   → **Bus Master:** Inicia y dirige las transferencias.
   → **Bus Slave:** Obedece y accede a las peticiones del bus master.

##### Tipos básicos de transferencia

  → **Escritura:** Master envía el dato a Slave
  → **Lectura:** Slave envía el dato a Master    

##### Ciclos del Bus

   → **Direccionamiento** del slave
   → Especificacion del **tipo de operación** (Lectura o Escritura)
   → **Transferencia** del dato
   → **Finalización** del ciclo del bus

##### Control de transferencia

   → **Sincronización:** Determina el inicio y el final de cada transferencia
   → **Arbitraje:** control el acceso al bus en caso de varios masters.



## Parametros de caracterización

   → **Capacidad de conexión:** Número de cables
   → **Longitud de bus:** Distancia que puede separar dos dispositvos conectados
   → **Ancho de bus:** Número de lineas. 
   → **Ancho de datos:** número total de líneas para datos
   → **Ancho de banda:** caudal máximo de información que puede transmitirse
   → **Protocolo de transferencia o de sincronización:** Método para sincronizar Master y Slave
   → **Protocolo de arbitraje:** método para la resolución de conflictos de acceso por varios masters.



## Clasificación de las líneas del bus

### Según su función

​          Según su función
   → **Líneas de datos (bus de datos):** Transmiten datos.
   → **Líneas de direcciones (bus de direcciones):** Designa la fuente o el destino de un dato.
   → **Lineas de control:** Gobiernan el acceso y el uso de las lineas de datos y las lienas de direcciones.
​         • **Lineas de operación:** Determinan el tipo de operación que debe realizar el slave.
​         • **Lineas de sincronización:** determinan el comienzo y el final de cada transferencia.
​         • **Líneas de arbitraje:** Determinan cual de los elementos conectados puede usar el bus.

### Según su uso

→**Líneas dedicadas:** tienen asignada una única función
→**Líneas multiplexadas:** Realizan distintas funciones a lo largo del tiempo.



## Protocolos de transferencia

### Función

sincronizar los elementos implicados en una transferencia (Master y Slave)
Determinar el comienzo y el final de cada transferencia

### Tipos de transferencia

   → Lectura
   → Escritura
   → Lectura de bloque
   → Esctiruda de bloque
   → Lectura - modificacion - escritura
   → Lectura despues de escritura

### Tipos de protocolo

   → Asincrono
   → Sincrono: Las transefencias están gobernadas por una única señal de reloj compartida con todos los dispositivos. Cada transferencia se realiza en un número fijo de periodos de reloj. Los flancos del reloj determinan el comienzo de un nuevo ciclo del bus y el final del ciclo anterior.
   → Semisincrono
   → Ciclo partido