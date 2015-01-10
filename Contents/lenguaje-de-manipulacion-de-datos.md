# Lenguaje de manipulación de datos #

Permite el manejo y procesamiento del contenido de la base de datos.

## INSERT ##

INSERT INTO table_name (column1,column2,column3,...)
VALUES (value1,value2,value3,...);

INSERT INTO table_name
VALUES (value1,value2,value3,...);

Utilizado para cargar lotes de datos en la base de datos en una única operación.

Ejemplo especificando el nombre de la columna y su valor:

<pre><code>
INSERT INTO personas(id, nombre, apellidos) values
(null, "Nombre1", "Apellido1"),
(null, "Nombre2", "Apellido2"),
(null, "Nombre3", "Apellido3"),
(null, "Nombre4", "Apellido4");
</code></pre>

Ejemplo especificando solamente el valor de la columna:

<pre><code>
INSERT INTO personas values
(null, "Nombre1", "Apellido1"),
(null, "Nombre2", "Apellido2"),
(null, "Nombre3", "Apellido3"),
(null, "Nombre4", "Apellido4");
</code></pre>

## SELECT ##

Utilizado para consultar registros de la base de datos que satisfagan un criterio determinado.


## UPDATE ##
Utilizado para modificar los valores de los campos y registros especificados.

UPDATE nombre_tabla
SET colunna1=valor1,columna2=valo2,...
WHERE nombre_columna=valor;

Ejemplo:
<pre><code>
UPDATE personas SET nombre="Juan", apellidos="Perez" WHERE id=1;
</code></pre>

## DELETE ##
Utilizado para eliminar registros de una tabla de una base de datos.

Sintaxis<br />
DELETE FROM nombre_tabla
WHERE nombre_columna=valor;

Ejemplo:
<pre><code>
DELETE FROM usuarios WHERE id=1; 
</code></pre>