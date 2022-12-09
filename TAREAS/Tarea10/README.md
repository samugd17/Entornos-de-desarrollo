<div align="justify">

# Clinica Veterinaria:

<div align="center">
  <img src="https://camo.githubusercontent.com/e21930f6d81a091158f817460059fa81e903fb0c4f62faa72ecca8515e437cae/68747470733a2f2f65736375656c616661726d616369612e636f6d2f77702d636f6e74656e742f75706c6f6164732f636c2543332541446e6963612d7665746572696e617269612e6a7067"/>
</div>


Se propone un ejercicio de un diagrama de casos de uso que consiste en el diseño de una aplicación que gestione los tramites a realizar en una clínica veterinaria en base a las siguientes premisas:
- La clínica veterinaria almacena datos de contacto de todos sus clientes como pueden ser: Nombre, Apellidos, DNI, Fecha de nacimiento, Teléfono o Email. Estos datos son introducidos y gestionados por los auxiliares, que ejercen las funciones administrativas.
- Además se almacena información de cada uno de las mascotas de las que es dueño cada cliente. Obviamente, cada cliente puede tener más de una mascota, pero cada mascota solo puede pertenecer a un único cliente. Se permite, además, cambiar el dueño de una mascota por otro.
- Al dar de alta un nuevo animal, se comprobará en el registro del REIAC (Red Española de Identificación de Animales de Compañía) si el animal está correctamente dado de alta. Este proceso unicamente se hará en animales que tengan la obligación de estar identificados.
- Cada vez que un veterinario realiza una consulta sobre un animal, esta queda almacenada incluyendo datos básicos como: Tiempo de consulta, Identificación de la persona que lo ha tratado, Animal tratado, Importe total, Resolución, Recetas… Para calcular el tiempo de la consulta el veterinario tendrá un botón en la aplicación donde pueda pulsar cuando comienza la consulta para calcular el tiempo a modo de cronómetro y otro botón para finalizar.
- En caso de que el animal se quede ingresado en la clínica, el cliente debe ser capaz de acceder al estado en tiempo real del animal. Además podrá comunicarse con una cámara que tendrá el animal colocada, donde podrá ver su situación actual. La gestión de estas cámaras no corresponde al sistema, sino que se utilizará una aplicación ya presente en el veterinario.
- Las recetas y otros documentos relacionados con el servicio se incluirán en un gestor de contenidos que ya está en funcionamiento en la clínica veterinaria.
- Una vez terminado el servicio, el cliente no tiene porque realizar inmediatamente el pago, sino que puede identificarse posteriormente en la aplicación vía web y realizar el pago. Si el cliente tarda más de una semana se efectuará un recargo sobre el precio inicial.
- Además, el cliente debe ser capaz de obtener un histórico de todas las consultas que ha recibido cualquiera de sus mascotas.

<details>

<summary>SOLUCIÓN</summary>

## IDENTIFICACIÓN ELEMENTOS DIAGRAMA:

_**ACTORES**_

- Cliente.
- Veterinario.
- Auxiliar. 
- REIAC (Red Española de Identificación de Animales de Compañía).

_**CASOS DE USO**_

- Introducir datos clientes.
- Gestionar datos clientes. 
- Dar de alta mascota.
- Gestionar datos mascota.
- Comprobar alta. 
- Guardar datos consulta. 
- Cronometrar consulta. 
- Acceder estado del animal. 
- Autenticar usuario. 
- Realizar pago. 
- Acceder histórico consultas.




</details>

</div>
