# Git Fundamentals



## What is git?

Git is software for tracking changes in any set of files, usually used for coordinating work among programmers collaboratively developing source code during software development. Its goals include speed, data integrity, and support for distributed, non-linear workflows (thousands of parallel branches running on different systems).



## Estructura de Git

En git existen tres areas principales en git, las cuales son:

| Working directory                                      | **Staging area**                                             | Local Repository                                             |
| ------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Es una carpeta donde se guardarán todos los proyectos. | Es un area temporal que guardará los cambios que se hagan en el working directory. Cuango se quieran guardar, se guardará de forma oculta en un repositorio llamado Local Rep. Git guardará todos los cambión ahí. | Es un repositorio local, el cual se encuentra oculto, donde se guardarán todos los cambios, a través de este podrás descargar y cargar archivos a la red. |



El workflow será el siguiente:

![download (1)](assets/download (1).png)



Se trabajará en el working directory que no es más que la carpeta que contiene nuestro proyecto. Posteriormente se agregará al staging area. Luego se agregará al repositorio local y finalmente si se requeire al repositorio remoto.



