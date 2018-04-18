Clase Conexion PHP
=================

Clase para conectar base de datos mySQL con php.
Se compone del fichero de la clase Conn y del fichero de configuración de usuarios.

CONFIGURACION
--------------------
Debe crear un usuario e indicar en name server en el archivo de configuracion.
Se incluye en el constructor de la clase. 

METODOS
--------
+ getConnect() 
	retorna la conexion a la base de datos
+ getDB()
	retorna la base de datos
+ query()
	realiza una consulta dada en la variable sql a la base datos 

+ getAll([return])
	retorna todos los registros de la tabla seleccionada
	parametro return: string opcional -> indica campos a retornar

+ getById(id, [return])
	retorna una consulta realizada con el indice de la tabla (id es campo clave numerico)
	parametro id : entero obligatorio -> el identificador de la fila
	parametro return: string opcional -> indica campos a retornar

+ getBy(campos, [return])
	retorna una consulta que tiene como filtros los argumentos pasados
	paremetro campos es un array donde la clave es la columna donde buscar y el valor es el valor a 
buscar
	parametro return: string opcional -> indica campos a retornar 
	
