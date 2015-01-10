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

<pre><code>
DROP TABLE nombre_tabla;
</code></pre>

Empleado para eliminar tablas, stored procedures e índices.

## ALTER ##
Utilizado para modificar las tablas agregando campos o cambiando la definición de los campos.

### Para agregar una columna ###
<pre><code>
ALTER TABLE tabla_nombre
ADD columna_nombre tipo_de_dato;
</code></pre>

### Para eliminar una columna ###
<pre><code>
ALTER TABLE tabla_nombre
DROP COLUMN columna_nombre;
</code></pre>

### Para cambiar el nombre y el tipo de dato de una columna ###
<pre><code>
ALTER TABLE usuarios
CHANGE nombre_columna nuevo_nombre_columna tipo_de_dato;
</code></pre>

## TRUNCATE ##
Sirve para borrar y recrear una tabla completamente, es el equivalente a un DELETE FROM TABLE pero tiene sus diferencias.

Ejemplo:
<pre><code>
TRUNCATE nombre_tabla:
</code></pre>