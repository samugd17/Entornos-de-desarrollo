<div align="justify"> 

# Instalación de JDK en Devian

## Índice
- [Introducción.](#introducción)
- [Cómo instalar Java en Ubuntu desde repositorios.](#cómo-instalar-java-en-ubuntu-desde-repositorios)
- [Cómo instalar una versión específica de Java.](#cómo-instalar-una-versión-específica-de-java)
- [Configuración de las variables de entorno](#configuración-de-las-variables-de-entorno)

## Introducción

Java sin dudas es un lenguaje de programación que es utilizado para diversos propósitos y es un complemento casi esencial para la ejecución y funcionamiento de diversas herramientas, la instalación de java es prácticamente una tarea esencial después de haber realizado la instalación de este.

Es por ello que en esta ocasión compartiré con ustedes un sencillo tutorial de como instalar Java en nuestro sistema con el JDK el cual es un entorno de desarrollo y el entorno de ejecución JRE.

## ¿Cómo instalar Java en Ubuntu desde repositorios?

Lo primero debemos de actualizar el sistema con:

```
  sudo apt-get update
```
e instalamos Java con este comando:

```
  sudo apt-get install default-jdk
```

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea5/IMG/1.png">


para comprobar que tenemos instalado Java en nuestro sistema solo debemos de ejecutar:
```console
  java --version
```

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea5/IMG/1.1.png">

</br>

## ¿Cómo instalar una versión específica de Java?

Para instalar Ubuntu Java Open JDK ("la que utilizaremos en 1º").
 - OpenJDK:
   - 11
   ```
   sudo apt install openjdk-11-jdk
   ```
    - 17
   ```
   sudo apt install openjdk-17-jdk
   ```
 _**En mi caso, he instalado la  versión 17 por fallos de compatibilidad con otras versiones como la 8 o la 13**_.
 
 <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea5/IMG/2.png">

Al igual que antes, comprobamos la versión que tenemos activa con:

```console
  java --version
```
<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea5/IMG/2.1.png">



## Configuración de las variables de entorno

 El siguiente paso consiste en establecer las variables de entorno. Es necesario porque cuando se usa Java, Linux necesita saber dónde está ubicado el programa para ejecutarlo y qué versión de Java usar de forma predeterminada. Para modificar esto, usaremos el editor de texto nano. Primero, abra el archivo en Nano.

### Listar la versiones de OpenJDK instaladas

 Ejecuta el siguiente comando para verificar que se han descargado las diferentes versiones de OpenJDK.

```console
 ls /usr/lib/jvm
```

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea5/IMG/3.png">

### Actualización de las variables de entorno

 Edita y modifica el fichero profile, con los comandos:

```console
sudo update-alternatives --config java
```

 y selecciona la version _11_.

en

```console
/etc/profile.d/java.sh
```
<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea5/IMG/6.png">

</br>
</br>

_**Dentro del editor escribimos "hola soy un script" para hacer la prueba y luego guardamos el archivo**_.

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea5/IMG/5.png">

Haga que el script sea ejecutable con chmod:

```console
sudo chmod +x /etc/profile.d/java.sh
```

Finalmente, cargue las variables de entorno usando el comando de source

```console
source /etc/profile.d/java.sh
```

<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea5/IMG/7.png">

<div align="right"> 
Samuel Eloy González Díaz.1ºDAW
</div>

</div>
