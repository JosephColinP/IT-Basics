# Chipsets


El chipset es el conjunto de chips que se encargan de controlar determinadas funciones del ordenador como la forma en que interacciona el microprocesador con la memoria o el caché, o el control de los puertos, PCI, AGP, USB.

## A Brief History of Chipsets

Back in the days of computer yore, PC motherboards consisted of lots of discrete integrated circuits. This generally required a separate chip or chips to control each system component: mouse, keyboard, graphics, sounds, and so on.

As you can imagine, having all those various chips scattered about was pretty inefficient.

In order to address this problem, computer engineers needed to devise a better system, and began integrating these disparate chips into fewer chips.

With the advent of the [PCI bus](https://en.wikipedia.org/wiki/Conventional_PCI), a new design emerged: bridges. Instead of a bunch of chips, motherboards came with a *northbridge* and a *southbridge*, which consisted of just two chips with very specific duties and purposes.

## Types of chipsets

### Northbirde

Es el encargado de gestionar la RAM, los puertos gráficos (AGP) y el acceso al resto de componentes del chipset, así como la comunicación entre estos y el procesador.

### South Bridge

Controla lo relacionado con los puertos o conectores donde podemos conectar nuestros periféricos, es decir se encarga de la E/S de datos.

## Total Integration

Hasta el momento que fue escrito esto, existen pequeños cambios a la integración de un sistema de un solo chip. Diferentes componentes como controladores gráficos o de almacenamiento ya están integrados directamente al CPU. Dejando así las tareas que quedan al southbridge. Eso hace que el northbridge ya no sea utilizado y se utilice un solo chipset. 

## Otras Funcionalidades

El chipset también determina que partes son compatibles, es decir, determina el tipo de conexión que acepta la placa madre. También determina los puerto, esto quiere decir que determinará que tipo de perifpericos se van a conectar y que conexión se utilizará.

Por último tambíen determinará la capacidad de la computadora para realizar Overclocking.



