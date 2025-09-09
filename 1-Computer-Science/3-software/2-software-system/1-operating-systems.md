#  Operating systems



- [Operating system](#Operating system)
- [Componentes de un sistema operativo](#Componentes de un sistema operativo)
  - [Kernel](#Kernel)
  - [Processes Management](#Processes Management)
  - [Memory Management](#Memory Management)
  - [Disk access and File Management](#Disk access and File Management)
  - [I/O Management](#I/O Management)
  - [Network Management](#Network Management)
  - [Security Management](#Security Management)
  - [User Interface](#User Interface)
  - [Command Interpreter System](#Command Interpreter System)

- [Clasificación de los Sistemas Operativos](#Clasificación de los Sistemas Operativos)





## Operating system

An operating system (OS) is an interface between a computer user and computer hardware. an OS is a system software that manages computer hardware, software resources, and provides common services for computer programs.



Un sistema operativo es un software sobre el cual trabajan otros softwares que permiten administrar los recursos de la computadora y controlar su funcionamiento. Un sistema operativo realiza cinco funciones básicas:
   → Suministro de interfaz al usuario.
   → Administración de recursos.
   → Administración de archivos.
   → Adminsitración de tareas.
   → Servicio de soporte.



### Definiciones

*"An Operating System is the low-level software that supports a computer's basic functions, such as scheduling tasks and controlling peripherals".*



We can refine this definition as follows:

*"An operating system is a program that acts as an interface between the user and the computer hardware and controls the execution of all kinds of programs".*



## Componentes de un sistema operativo

An operating system is a large and complex system that can only be created by partitioning into small parts. These pieces should be a well-defined part of the system, carefully defining inputs, outputs, and functions.

Although Windows, Mac, UNIX, Linux, and other OS do not have the same structure, most operating systems share similar OS system components, such as file, memory, process, I/O device management.



### Kernel

The kernel is a computer program (software) at the core of a computer's operating system and has complete control over everything in the system.

It is the portion of the operating system code that is always resident in memory, and facilitates interactions between hardware and software components.

It manly do three things

- Handles the rest of the start-up process
- Handles the input/output request from other programs.
- Manages memory and hardware peripherals (keyboards, monitors, printers, speakers, etc.)



### Processes Management

The process management component is a procedure for managing many processes running simultaneously on the operating system. Every running software application program has one or more processes associated with them.

Process management keeps processes running efficiently. It also uses memory allocated to them and shutting them down when needed.



#### Functions of process management

   → Process creation and deletion.
   → Suspension and resumption.
   → Synchronization process
   → Communication process



### Memory Management

Among other things, a multiprogramming operating system kernel must be responsible for managing all system memory which is currently in use by programs. This ensures that a program does not interfere with memory already in use by another program. Since programs time share, each program must have independent access to memory.



#### Virtual Memory

Is a combination of hard drive space and RAM that acts like memory that our processes can use. When we execute a process, we take the data of the program in chunks we call pages. We store these pages in virtual memory. If we want to read and execute these pages, they have to be sent to physical memory or RAM.



### Disk access and File Management

Access to data stored on disks is a central feature of all operating systems. Computers store data on disks using files, which are structured in specific ways in order to allow for faster access, higher reliability, and to make better use of the drive's available space. 

The specific way in which files are stored on a disk is called a file system, and enables files to have names and attributes. It also allows them to be stored in a hierarchy of directories or folders arranged in a directory tree.



#### Function of file management  

The operating system has the following important activities in connection with file management:  

   → File and directory creation and deletion. 
   → For manipulating files and directories. 
   → Mapping files onto secondary storage. 
   → Backup files on stable storage media.



### I/O Management


Los input/output devices son todos los perifericos. El kernel carga los drivers que se necesitan ser usados para reconocer los periféricos, también manjea la intercomunicación entre los perifericos. Por esto también se encarga de ver cual es la manera más eficiente de transferencia e intenta que durante estos procesos no haya errores.



### Network Management

Network management is the process of administering and managing computer networks. It includes performance management, provisioning of networks, fault analysis, and maintaining the quality of service.



### Security Management

Security refers to a mechanism for controlling the access of programs, processes, or users to the computer resources. 

The operating system must be capable of distinguishing between requests which should be allowed to be processed, and others which should not be processed.

Some of the security measurement are:

- Distinguish between "privileged" and "non-privileged"
- Have a form of requester identity, such as username or password
- Other methods of authentication, such as magnetic cards or biometric data

In addition to the allow or disallow model of security, a system with a high level of security also offers auditing options. These would allow tracking of requests for access to resources (such as, "who has been reading this file?").



### User Interface

Every computer that is to be operated by an individual requires a user interface. The user interface is usually referred to as a shell and is essential if human interaction is to be supported.

The two most common forms of a user interface have historically been the **command-line interface**, where computer commands are typed out line-by-line, and the **graphical user interface**, where a visual environment is present.



### Command Interpreter System

One of the most important components of an operating system is its command interpreter. The command interpreter is the primary interface between the user and the rest of the system.

One of the most important components of an operating system is its command interpreter. The command interpreter is the primary interface between the user and the rest of the system.





## Clasificación de los Sistemas Operativos



### Por su Estructura

- **Monolitica:** Constituidos fundamentalmente por un solo programa compuesto de un conjunto de rutinas entrelazadas de tal forma que cada una puede llamar a cualquier otra.
- **Jerárquica/estratos:** Se compone por subpartes y está organizado en niveles.



### Según la Administración de Tareas

- **Monotareas:** Este tipo de sistemas operativos son capaces de manejar un programa o realizar una sola tarea a la vez.
- **Multitarea:** Permiten ejecutar varios procesos a la vez, desde uno o varias computadoras, es decir que los pueden utilizar varios usuarios al mismo tiempo.



### Según la Administración de Usuarios

- **Mono-usuarios:** Sólo pueden responder a un usuario por vez. Existe un único usuario que puede realizar cualquier tipo de operación.
- **Multi-usuarios:** Son capaces de dar servicio a más de un usuario a la vez.



### Según sus CPUs

- **MonoProceso:** Un sistema operativo monoproceso es aquél que es capaz de manejar solamente un procesador de la computadora, de manera que si la computadora tuviese más de uno le sería inútil. 
- **Multiproceso:** Las computadoras que tienen mas de un CPU son llamadas multiproceso. Un sistema operativo multiproceso coordina las operaciones de las computadoras multiprocesadoras







