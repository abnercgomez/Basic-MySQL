# Lenguaje de definición de datos #

 Permite definir y describir los objetos de la base de datos, su estructura, relaciones y restricciones. 

## CREATE ##
Utilizado para crear nuevas tablas, stored procedures e índices.

<b>CREATE DATABASE nombre_tabla;</b><br />
Comando que crea una nueva base de datos.

Ejemplo:

<pre><code>
CREATE DATABASE personas;	
</code></pre>

<b>CREATE TABLE nombre_tabla (<br />
    nombre_columna1 descripción,<br />
    nombre_columna2 descripción<br />
);</b><br />
Comando que crea una nueva tabla y su estructura.

Ejemplo:

<pre><code>
CREATE TABLE personas(
id integer(10) NOT NULL AUTO_INCREMENT
nombre varchar(60) NOT NULL,
apellido varchar(60) NOT NULL,
PRIMARY KEY(ID)
);	
</code></pre>

## DROP ##

<b>DROP TABLE nombre_tabla;</b>

Empleado para eliminar tablas, stored procedures e índices.


## ALTER ##
Utilizado para modificar las tablas agregando campos o cambiando la definición de los campos.