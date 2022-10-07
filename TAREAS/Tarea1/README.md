# Tarea 1: Tienda Ventas
La empresa Puerto Systems ha recibido un nuevo encargo de software.

Se trata de diseñar una aplicación para una tienda especializada en vender productos estéticos.

La tienda desea trabajar con software libre. Además, desea explícitamente que la aplicación sea capaz de cumplir las siguientes tareas:

- Proporcionar facturas de las ventas.
- Llevar la cuenta de lo que vende cada trabajador.
- Controlar el stock de productos en almacén.
- Operar con lector de código de barras y tarjetas de crédito.
- Controlar los precios de los productos y ofrecer la posibilidad de operar con ellos.
- El tiempo de respuesta de la aplicación ha de ser lo menor posible.
- No se podrán procesar dos peticiones a la vez, aunque haya varios equipos funcionando
simultáneamente.

La empresa también quiere almacenar información de sus trabajadores: DNI, nombre,
apellidos, número de la Seguridad Social, fecha de nacimiento, teléfono y localidad.
Asimismo, de los productos interesa almacenar: código, marca, nombre comercial, precio, cantidad.  

- - -

## Análisis de requerimientos del sistema
Comenzaremos nuestro análisis de requisitos del sistema detallando los requisitos funcionales y no funcionales del sistema.   
Los **requisitos funcionales** podemos describirlos como las funciones que tendrá que realizar nuestra aplicación. En este caso son las siguientes:
- Proporcionar facturas de las ventas.
- Llevar la cuenta de lo que vende cada trabajador.
- Controlar el stock de productos en almacén.
- Operar con lector de código de barras y tarjetas de crédito.
- Controlar los precios de los productos y ofrecer la posibilidad de operar con ellos.
- Almacenar información de los trabajadores (DNI, nombre, apellidos, número de la seguridad social, fecha de nacimiento, teléfono y localidad). 
- Almacenar información de los productos (código, marca, nombre comercial, precio y cantidad).

Los **requisitos no funcionales** son la características que debe tener el programa al completos obviando los datos. Para nuestro caso serían las siguientes:
- Reducir el tiempo de respuesta de la aplicación. Intentaremos obtener unos tiempos de respuesta que se adapten a las necesidades del cliente y sean los más rápidos posibles. 
- Impedir el uso de dos peticiones simultáneas, aunque hayan varios equipos funcionando a la misma vez.

Después de esto, planificaremos una serie de reuniones con el cliente con el fin de precisar cada uno de los requerimientos a desarrollar y comprobar las características hardware del equipamiento informático de nuestro cliente.  

## Diseño
Para este proyecto, utilizaremos un **modelo de ciclo de vida ágil**, ya que en este se nos permite adaptar la forma de trabajo a las condiciones del proyecto, consiguiendo flexibilidad e inmediatez en la respuesta para amoldarlo y desarrollarlo teniendo en cuenta las circunstancias específicas del entorno. En concreto, utilizaremos el modelo **Scrum**.  

La metodología Scrum, es un modelo de desarrollo incremental utilizado para llevar a cabo un conjunto de tareas de forma regular, con el objetivo principal de trabajar de manera colaborativa. Consiste en ir realizando entregas regulares y parciales del trabajo final, de manera prioritaria y en función del beneficio que aportan dichas entregas a los receptores del proyecto. Por este motivo, es una metodología especialmente indicada para proyectos complejos, con requisitos cambiantes y en los que la innovación y la flexibilidad son protagonistas.

</br>
<img src="https://www.iebschool.com/blog/wp-content/uploads/2021/04/como-funciona-scrum.png">  
</br>

El diseño de este proyecto lo dividiremos en 4 etapas diferenciadas:
- **1.Planificación: Product Backlog.**
En esta primera fase, en continua comunicación con el cliente, se establecerán las tareas prioritarias y objetivos a lograr. El Product Backlog tiene permitido cambiar y crecer tantas veces como sea necesario en función del aprendizaje adquirido en el desarrollo del producto.  

- **2.Sprint Backlog.**
En la segunda fase, el equipo decide a cuanto trabajo se compromete en vez de serles asignado. Esto hace que el compromiso sea más fiable porque el equipo lo está haciendo basado en su propio análisis y planificación.

- **3.Ejecución: Sprint.**
En esta tercera etapa, que como máximo tendrá una duración de un mes, el equipo de trabajo se focalizará en el desarrollo de tareas para poder conseguir el producto potencialmente entregable. Durante este proceso, habrá reuniones diarias con el equipo donde se irá analizando la marcha de las tareas, posibles inconvenientes que vayamos encontrando y posibles soluciones.

- **4.Revisión: Sprint review.**
Al final del sprint, el equipo se reúne en una sesión informal para ver una demostración o inspeccionar el incremento. El equipo de desarrollo muestra los elementos del backlog que ahora están finalizados a las partes interesadas y a los compañeros de equipo para recibir comentarios. El propietario del producto puede decidir si lanzar o no el producto. En caso de que el cliente no quede satisfecho, se volvería a la fase del Sprint Backlog, para corregir, añadir o suprimir cuantos cambios se quieran realizar.

 En cuanto al sistema gestor de Bases de Datos hemos decido usar MySql ya que es un sistema relacional y además se puede utilizar como software libre, tal y como demanda el cliente. Las entidades y relaciones de la base de datos serán las siguientes:
 
 </br>
  
 </br>

 </br>

 </br>

 </br>
 
 ## Codificación
En este apartado, codificaremos toda la información que hemos visto anteriormente y la llevaremos a código fuente. El Lenguaje de programación que vamos a utilizar es **Python**, ya que se adapta a las necesidades del cliente al ser un software libre y también a nuestras necesidades y conocimientos, al ser un lenguaje de programación más intuitivo y sencillo, orientado a objetos, mediante el cual desarrollaremos un código reutilizable, más fácil de mantener y modular.

Con el entorno de desarrollo Eclipse, al ser un entorno completo, cubriremos las tres partes de la codificación:

- **1.Código Fuente:** Será tarea de los programadores desarrollar este código en el entorno de desarrollo Eclipse utilizando el editor de código. 

- **2.Código Objeto:** Utilizando el plugin "Pydev", el cual, entre las muchas funciones que trae incorporadas, destaca un compilador para python, obtendremos el código binario resultante de compilar el código fuente.

- **3.Código ejecutable:** Este código es el resultado de enlazar los archivos objeto, consta de un único archivo que puede ser ejecutado por el sistema operativo directamente. Este paso también lo realizaremos con la aplicación Eclipse.
 

 
