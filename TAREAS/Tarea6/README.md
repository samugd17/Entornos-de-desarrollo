<div align="justify">

# Instalación del IDE Netbeans

## Índice
- [Introducción.](#introducción)
- [Prerrequisitos.](#prerrequisitos)
- [Instalación.](#instalación)
- [Instalación a través de wget](#instalación-a-través-de-wget)
  
  
## Introducción
  NetBeans es un IDE popular para desarrollar aplicaciones Java. Esto permite desarrollar aplicaciones a partir de un conjunto de componentes de software modulares llamados módulos. NetBeans está disponible para ejecutarse en sistemas operativos populares como Windows, macOS, Linux.

<div align="center">
  <img src="https://www.linuxadictos.com/wp-content/uploads/apache-netbeans.jpg" width="250px">
</div>

## Prerrequisitos

  Recuerda que para la instalación de __Netbeans__ debes de tener instalado __Java__. Los pasos para realizar su instalación y configuración se encuentra en el siguiente [enlace](tarea-jdk.md).

  Para verificarlo recuerda ejecutar el siguiente enlace:

  ```console
  java --version
  ``` 
  
  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea6/IMG/1.%20JAVA%20VERSION.png">
  
  <br>

## Instalación

  Los paquetes Snap son paquetes de software universales prediseñados que se envían con las bibliotecas y dependencias requeridas por el paquete de software. Son independientes de la distribución y se pueden instalar en cualquier distribución principal de Linux. Los snaps son populares ya que no requieren ninguna dependencia durante la instalación, lo que hace que el proceso de instalación sea fluido y sin errores.
  
  En nuestro caso, antes de poder instalar Netbeans, hemos tenido que instalar los paquetes _snap_ ya que no los teníamos en nuestro sistema.
  Lo hacemos con el siguiente comando:
  
  ```console
  sudo apt install snapd
  ```
  
  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea6/IMG/3.%20NETBEANS%20INSTALLATION%20(WRONG).png">
  
  <br>

  Para instalar la edición Netbeans, ejecute el siguiente comando:

```console
sudo snap install netbeans --classic
```
  
  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea6/IMG/3.%20NETBEANS%20INSTALLATION%20(WRONG).png">
  
  <br>

  La instalación finalizará cuando veas el siguiente mensaje:

  ```console
  netbeans 15 from Apache NetBeans✓ installed
  ```

# Ejecutando Netbeans 15

  Ahora que Netbeans está instalado en su sistema, puede iniciarlo escribiendo netbeans en su terminal o haciendo clic en el icono de Netbeans ( Activities -> Netbeans ).
  
  <img src="https://liukin.es/wp-content/uploads/2021/10/Como-instalar-Netbeans-en-Ubuntu-Linux.png" width="550px">
  
  <br>

# Eliminar Netbeans

__No realices este paso, es para que conozcas como se elimina__.

 Una vez que no necesite Netbeans en su sistema. Use el siguiente comando para eliminar netbeans del sistema Ubuntu usando el comando snap.

```console
sudo snap remove netbeans
```

## Instalación a través de wget

Teniendo en cuenta que has completado la instalación de __java__ en la tarea anterior, puedes realizar la instalación de Netbeans 12.5 a través de __wget__. De esta forma se puede realizar la instalación en ___cualquier distribución de linux___.
  
  En nuestro caso hemos empleado este método ya que con el comando _snap_ no nos aparecía Netbeans.

Los pasos son los siguientes:
- Abre un navegador, navegue hasta la página de descarga de NetBeans IDE y descargue el último script de instalación de NetBeans IDE ([ Apache-NetBeans-12.5-bin-linux-x64.sh](https://netbeans.apache.org/download/nb125/nb125.html) ) para su distribución de Linux instalada.

  Alternativamente, también puede descargar el script de instalación de NetBeans IDE en su sistema a través de la utilidad wget, con el siguiente código:
  ```console
  wget -c  https://archive.apache.org/dist/netbeans/netbeans/12.5/Apache-NetBeans-12.5-bin-linux-x64.sh
  ```
- Una vez completada la descarga, navegue hasta el directorio donde se descargó el instalador de NetBeans IDE y ejecute el siguiente comando para que el script del instalador sea ejecutable y comience a instalarlo.
  Otorgamos permisos de ejecución:
  ```code
  chmod +x Apache-NetBeans-12.5-bin-linux-x64.sh 
  ```
  Ejecutamos el script de instalación
  ```code
  ./Apache-NetBeans-12.5-bin-linux-x64.sh
  ```
  
  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea6/IMG/4.%20INSTALLATION%20NETBEANS.png">
  
  <br>
  
- Después de ejecutar el script de instalación anterior, la “ Página de bienvenida ” del instalador se deben de seguir los pasos para personalizar la instalación (lenguajes soportados, etc).
  
  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea6/IMG/5.%20FINAL%20STEP.png">

</div>
