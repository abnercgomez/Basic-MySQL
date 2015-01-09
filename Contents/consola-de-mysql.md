# Consola de MySQL #

La consola de MySQL sirve para gestionar la base datos por línea de comandos.

Si usas el entorno de prueba XAMPP, la consola se encuentra en el siguiente directorio:
C:\xampp\mysql\lib

## Conectar con el servidor MySQL ##
<pre><code>
mysql -h localhost -u root -p
</code></pre><br />

<pre><code>
quit
</code></pre>

Cierra la conexión con el servidor

## Comandos básicos ##

<b>SHOW databases;</b><br />
Sirve para listar las bases de datos existentes en el servidor.

<b>USE nombre_base;</b><br />
Sirve para seleccionar una tabla y poder trabajar con sus tablas.

<b>SHOW tables;</b><br />
Sirve para listar las tablas de una base de datos.

<b>DESCRIBE nombre_tabla;</b><br />
<b>SHOW COLUMNS FROM nombre_tabla;</b><br />
Sirve para mostrar información de la tabla, campos que la componen, tipos de datos, etc.