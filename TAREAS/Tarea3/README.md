# Ejemplos en Git

## Índice

- [Ejercicio 1](#ejercicio-1)
- [Ejercicio 2](#ejercicio-2)
- [Ejercicio 3](#ejercicio-3)
- [Ejercicio 4](#ejercicio-4)
- [Ejercicio 5](#ejercicio-5)
- [Ejercicio 6](#ejercicio-6)
- [Ejercicio 7](#ejercicio-7)
- [Ejercicio 8](#ejercicio-8)
- [Ejercicio 9](#ejercicio-9)

## Paso previo

Como paso previo a la actividad, clonaremos nuestro repositorio *"libro"* y accederemos a el.

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Paso1.Clonaci%C3%B3n.png">

## Ejercicio 1

- Mostrar el historial de cambios del repositorio.
- Crear la carpeta capítulos y crear dentro de ella el fichero capitulo1.txt con el siguiente texto.

```console
Git es un sistema de control de versiones ideado por Linus Torvalds.
```

- Añadir los cambios a la zona de intercambio temporal.
- Hacer un commit de los cambios con el mensaje _Añadido capítulo 1._
- Volver a mostrar el historial de cambios del repositorio.

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio1.png">
<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio1.Parte1.png">
<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio1.Parte2.png">

## Ejercicio 2

- Crear el fichero capitulo2.txt en la carpeta capítulos con el siguiente texto.
 
```console
El flujo de trabajo básico con Git consiste en: 1- Hacer cambios en el repositorio. 2- Añadir los cambios a la zona de intercambio temporal. 3- Hacer un commit de los cambios.
```

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio2.png">

## Ejercicio 3

 - Crear el fichero capitulo3.txt en la carpeta capítulos con el siguiente texto.

```console
Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.
```

 - Añadir los cambios a la zona de intercambio temporal.
 - Hacer un commit de los cambios con el mensaje _Añadido capítulo 3._
 - Mostrar las diferencias entre la primera y la última versión del repositorio.

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio3.png">

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio3.1.png">

## Ejercicio 4

- Crea el fichero índice.txt la siguiente línea:
```console
Indice de los cápitulos, con conceptos avanzados de git
```
- Añadir los cambios a la zona de intercambio temporal.
- Hacer un commit de los cambios con el mensaje _"Indice de los cápitulos, con conceptos avanzados de git_.
- Mostrar quién ha hecho cambios sobre el fichero _indice.txt_.

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio4.png">

## Ejercicio 5

- Crear una nueva rama bibliografía y mostrar las ramas del repositorio.

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio5.png">

## Ejercicio 6

 - Crear el fichero capitulos/capitulo4.txt y añadir el texto siguiente:

```console
  En este capítulo veremos cómo usar GitHub para alojar repositorios en remoto.
```

 - Añadir los cambios a la zona de intercambio temporal.
 - Hacer un commit con el mensaje “Añadido capítulo 4.”
 - Mostrar la historia del repositorio incluyendo todas las ramas.

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio6.png">

## Ejercicio 7

- Cambiar a la rama bibliografía.
 - Crear el fichero bibliografia.txt y añadir la siguiente referencia:
```console
Chacon, S. and Straub, B. Pro Git. Apress.
```
 - Añadir los cambios a la zona de intercambio temporal.
 - Hacer un commit con el mensaje “Añadida primera referencia bibliográfica.”
 - Mostrar la historia del repositorio incluyendo todas las ramas.

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio7.png">

## Ejercicio 8

 - Fusionar la rama bibliografía con la rama main.
 - Mostrar la historia del repositorio incluyendo todas las ramas.
 - Eliminar la rama bibliografía.
 - Mostrar de nuevo la historia del repositorio incluyendo todas las ramas.

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio8.png">

## Ejercicio 9

 - Crear la rama bibliografía.
 - Cambiar a la rama bibliografía.
 - Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias:
```cosole
Scott Chacon and Ben Straub. Pro Git. Apress.
Ryan Hodson. Ry’s Git Tutorial. Smashwords (2014)
```
 - Cambiar a la rama main.
 - Cambiar el fichero bibliografia.txt para que  - contenga las siguientes referencias:
```console
Chacon, S. and Straub, B. Pro Git. Apress.
Loeliger, J. and McCullough, M. Version control with Git. O’Reilly.
```
 - Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Añadida nueva referencia bibliográfica.”
 - Fusionar la rama bibliografía con la rama main.
 - Resolver el conflicto dejando el fichero bibliografia.txt con las referencias:
```console
Chacon, S. and Straub, B. Pro Git. Apress.
Loeliger, J. and McCullough, M. Version control with Git. O’Reilly.
```
Hodson, R. Ry’s Git Tutorial. Smashwords (2014)
 - Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Resuelto conflicto de bibliografía.”
 - Mostrar la historia del repositorio incluyendo todas las ramas.

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea3/IMG/Ejercicio9.png">

<br>

Samuel Eloy González Díaz.1ºDAW.

