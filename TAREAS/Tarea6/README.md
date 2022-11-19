<div align="justify">

# Instalación del IDE Netbeans 12

## Índice
- [Introducción.](#introducción)
- [Cómo instalar Java en Ubuntu desde repositorios.](#cómo-instalar-java-en-ubuntu-desde-repositorios)
- [Cómo instalar una versión específica de Java.](#cómo-instalar-una-versión-específica-de-java)
- [Configuración de las variables de entorno](#configuración-de-las-variables-de-entorno)

  NetBeans es un IDE popular para desarrollar aplicaciones Java. Esto permite desarrollar aplicaciones a partir de un conjunto de componentes de software modulares llamados módulos. NetBeans está disponible para ejecutarse en sistemas operativos populares como Windows, macOS, Linux.

<div align="center">
  <img src="https://www.linuxadictos.com/wp-content/uploads/apache-netbeans.jpg" width="250px">
</div>

## Pasos

### Prerrequisitos

  Recuerda que para la instalación de __Netbeans__ debes de tener instalado __Java__. Los pasos para realizar su instalación y configuración se encuentra en el siguiente [enlace](tarea-jdk.md).

  Para verificarlo recuerda ejecutar el siguiente enlace:

  ```console
  java --version
  ``` 
  <div align="center">
  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea6/IMG/1.%20JAVA%20VERSION.png">
  </div> 

## Instalación

  Los paquetes Snap son paquetes de software universales prediseñados que se envían con las bibliotecas y dependencias requeridas por el paquete de software. Son independientes de la distribución y se pueden instalar en cualquier distribución principal de Linux. Los snaps son populares ya que no requieren ninguna dependencia durante la instalación, lo que hace que el proceso de instalación sea fluido y sin errores.

  Para instalar la edición Netbeans, ejecute el siguiente comando:

```console
sudo snap install netbeans --classic
```

  La instalación finalizará cuando veas el sigueinte mensaje:

  ```console
  netbeans 12.5 from Apache NetBeans✓ installed
  ```

# Ejecutando Netbeans 12

  Ahora que Netbeans está instalado en su sistema Ubuntu, puede iniciarlo escribiendo netbeans en su terminal o haciendo clic en el icono de Netbeans ( Activities -> Netbeans ).

<div align="center">
  <img src="https://liukin.es/wp-content/uploads/2021/10/Como-instalar-Netbeans-en-Ubuntu-Linux.png" width="250px">
</div>

  Una vez que se cargue el IDE de Netbeans, se le presentará la página de inicio.

# Eliminar Netbeans

__No realices este paso, es para que conozcas como se elimina__.

 Una vez que no necesite Netbeans en su sistema. Use el siguiente comando para eliminar netbeans del sistema Ubuntu usando el comando snap.

```console
sudo snap remove netbeans
```

## Instalación a través wget (Cualquier distribución Linux)

Teniendo en cuenta que has completado la instalación de __java__ en la tarea anterior, puedes realizar la instalación de Netbeans 12.5 a través de __wget__. De esta forma se puede realizar la instalación en ___cualquier distribución de linux___.

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
- Después de ejecutar el script de instalación anterior, la “ Página de bienvenida ” del instalador se deben de seguir los pasos para personalizar la instalación (lenguajes soportados, etc).
  
  <div align="center">
  <img src="https://github.com/samugd17/Entornos-de-desarrollo/blob/main/TAREAS/Tarea6/IMG/5.%20FINAL%20STEP.png">
  </div>  

</div>
