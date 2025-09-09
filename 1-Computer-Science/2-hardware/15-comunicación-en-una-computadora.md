# Comunicación en una computadora

## External Data Bus (EDB)

Are wires that interconnect the parts of the computer, when they send voltage is a 1 and when they or off is 0.

## Registers

Registers let us store data that our CPU works with. For example, our CPU wanted to add two numbers, one number would be stored in a register “A”. Another number would be stored in register “B”. The result of those two numbers would be stored in register “C”.

## Memory control check (MCC)

The MCC is a bridge between the CPU and the RAM. You can think of it, a nerve in your brain connecting to your memories. The CP talks to the MCC, and says, hey, I need the instructions for step number three of this recipe. The MCC finds the instructions for step number three in RAM, grabs the data, and sends it through the EDB.

## Adress Bus

It connects the CPU to the MCC, and sends over the location of the data, but not the data itself. Then the MCC takes the address and looks for the data. And then data is then sent over the EDB.

## Cache

Cache is smaller than RAM, but it let's us store data that we use often, and let's us quickly reference it. cache levels
L1: Smallest and fastest cache.

## Clock

In general, the clock refers to a microchip that regulates the timing and speed of all computer functions

## Clock wire

 Our CPU has an internal clock that keeps its operational in sync. It connects to a special wire called Clock wire. When you send or receive data, it sends a voltage to that clock wire to let the CPU know it can start doing calculations. 

## Clock speed

Have you ever seen a CPU in the store and has something labeled 3.4ghz, this number refers to the Clock speed of the CPU. Which is a maximum number of clock cycles that it can handle in a set in a certain time period. 3.40 gigahertz is 3.4 billion cycles per second.

## Overclocking

There's a way you can exceed the number of clock cycles on your CPU on almost any device. It's referred to as Overclocking and it increases the rate of your CPU clock cycles in order to perform more tasks. This is commonly used to increase the performance in low-end CPUs.

## ¿Como funciona?

Cada accion la procesa el CPU, estas se transmiten por los EDB por medio del código binario, El MCC hace puente entre el CPU y la RAM para sacar la información que necesita la CPU para operar. Pero para esto se necesita un Adress Bus que le dice a la CPU donde están los datos, posteriormente la MCC los recolecta y los manda a travéz del EDB. A veces en vez de ir a la RAM irán al Cache que es una memoria más pequeña pero almacena los datos más frecuentes. Para esto tambien es utiliza un clock wire, que es un cable que envía ceñales al CPU y le dice cuando empezar y terminar de hacer calculos.

## La función de una computadora

1. La fuente de energía alimenta a los componentes.
2. La BIOS analiza el sistema y se asegura que esté todo bien.
3. Le da el mando al disco de almacenamiento que tiene el sistema operativo.
4. El disco inicia el sistema operativo y comienza a trabajar la computadora.
5. Se abre un programa (Todos los componentes siempre están trabajando).
6. El procesador le pide al disco duro que mande todos los datos necesarios.
7. El disco duro se lo manda a la memoria RAM y la memoria RAM al procesador.
8. El procesador ejecuta todas las acciones necesarias.
9. La placa de video transforma todos los datos en imágenes que podamos ver.