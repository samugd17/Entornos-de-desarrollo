<div align="justify">

# Instalación de MAVEN en Ubuntu

## Índice
- [Introducción.](#introducción)
- [Instalación.](#instalación)
- [Establecer variables de entorno](#establecer-variables-de-entorno)

## Introducción

 Apache Maven es una herramienta de gestión y comprensión de proyectos de código abierto que se utiliza principalmente para proyectos Java. Maven usa un modelo de objetos de proyecto (POM), que es esencialmente un archivo XML que contiene información del proyecto, detalles de configuración, dependencias del proyecto y más.
 <br>
 
 <div align="center">
 <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/52/Apache_Maven_logo.svg/1200px-Apache_Maven_logo.svg.png" width="300px">
 </div>

## Instalación

### Instalar Apache Maven con apt

 Instalar Maven en Ubuntu usando apt es un proceso simple y directo.

 Actualice el índice del paquete e instale Maven ingresando los siguientes comandos:

```
 sudo apt update
```
 
<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea9/IMG/1.%20ACTUALIZANDO%20%C3%8DNDICE%20DE%20PAQUETES.png">
 
 Seguidamente, aplicamos el siguiente comando para instalar el IDE.
 
```
 sudo apt install maven
```
 
 
 Al ejecutarlo, nos aparece un error _**«could not get lock /var/lib/dpkg/lock»**_. Este fallo suele aparecer cuando otro proceso que haga uso de apt este en ejecución ya sea en un segundo plano o cuando se tiene abierto el centro de software de Ubuntu, Synaptic y demás. Esto se debe a que Ubuntu, de forma predeterminada, habilita las actualizaciones en segundo plano para la actualización de seguridad. Cuando Ubuntu termina de iniciarse, automáticamente ejecuta el comando apt-get update comando. Si hay actualizaciones de seguridad disponibles, las instalará en segundo plano. Así que si ejecutan el comando sudo apt upgrade al mismo tiempo, se muestra el error anterior.
 
 Para solucionar esto, a través de la terminal, modificaremos el fichero donde se permite a Ubuntu actualizarse automáticamente siguiendo estos sencillos pasos:
 
 **1.** Ingresamos el siguiente comando:

 ```
sudo nano /etc/apt/apt.conf.d/20auto-upgrades
 ```
 
 **2.** Este nos abrirá el editor nano donde habrá que reemplazar el contenido original por este:
 
 ```
APT::Periodic::Update-Package-Lists "1";
 
APT::Periodic::Download-Upgradeable-Packages "0";
 
APT::Periodic::AutocleanInterval "0";
 
APT::Periodic::Unattended-Upgrade "0";
 ```
 
 Quedando tal y como aparece en la imagen
 
 
  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea9/IMG/2.%20SOLUCION.png">
 
Acto seguido, guardaremos el archivo con Ctrl + O y saldremos con Ctrl + X. Posteriormente reiniciamos nuestro equipo.
 
 Ahora si, ya podemos ejecutar con normalidad el comando de instalación que antes fallaba y seguir adelante con los  pasos.

  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea9/IMG/3.%20MAVEN%20INSTALL.png">

 Para verificar la instalación, ejecute mvn -version:
```
 mvn -version
```

 La salida debería verse de forma similar:

 <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea9/IMG/4.%20MAVEN%20VERSION.png">

 Eso es todo. Maven ahora está instalado en su sistema y puede comenzar a usarlo.

### Instalar una versión concreta de Apache Maven

 En el momento de escribir este artículo, la última versión disponible de Apache Maven es la 3.8.6.

 Descargue Apache Maven en el directorio /tmp:

```
wget https://www.apache.org/dist/maven/maven-3/3.8.6/binaries/apache-maven-3.8.6-bin.tar.gz -P /tmp
```

 Una vez que se complete la descarga, extraiga el archivo en el directorio /opt
```
sudo tar xf /tmp/apache-maven-*.tar.gz -C /opt
```
 
 Para tener más control sobre las versiones y actualizaciones de Maven, que a crear un maven enlace simbólico que apunte al directorio de instalación de Maven:

```
sudo ln -s /opt/apache-maven-3.8.6 /opt/maven
```
 
<img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea9/IMG/5.%20DESCARGA%20ESPEC%C3%8DFICA%20MAVEN.png">
 
 Cuando se lanza una nueva versión, puede actualizar su instalación de Maven desempaquetando la última versión y cambiando el enlace simbólico para señalarla.


## Establecer variables de entorno
 
 A continuación, necesitaremos establecer las variables de entorno. Para hacer esto, abra su editor de texto y cree un nuevo archivo llamado maven.sh en el directorio /etc/profile.d/
```
sudo nano /etc/profile.d/maven.sh
```
Pega el siguiente código:

```
 export M2_HOME=/opt/maven
 export MAVEN_HOME=/opt/maven
 export PATH=${M2_HOME}/bin:${PATH}
```
 
  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea9/IMG/6.%20NANO.png">
 <br>
  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea9/IMG/6.1.%20NANO.png">
 <br>

 Guarde y cierre el archivo. Este script se utilizará al iniciar el shell.

 Haga que el script sea ejecutable con chmod:

```
 sudo chmod +x /etc/profile.d/maven.sh
```
 Finalmente, cargue las variables de entorno usando el comando de source
```
 source /etc/profile.d/maven.sh
```
 
  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea9/IMG/7.%20SCRIPT.png">

### Verificar la instalación

Para verificar que Maven está instalado, use el mvn -version que imprimirá la versión de Maven:

```
mvn -version
```

Debería ver algo similar a lo siguiente:

 <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea9/IMG/8.%20MAVEN%20VERSION%20FINAL.png">

Eso es todo. La última versión de Maven ahora está instalada en su sistema Ubuntu.

Conclusión
Le mostramos cómo instalar Apache Maven en Ubuntu. Ahora debería visitar la página de documentación oficial de Apache Maven y aprender cómo empezar con Maven.
 
 <div align="right">
 Samuel Eloy González Díaz.1ºDAW
 </div>

</div>
