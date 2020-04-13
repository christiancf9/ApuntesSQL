                                                       SENTENCIAS DDL
                                        
Usando sentencias **``DDL``** para crear y manejar tablas

Un esquema es la colección de múltiples objetos de una BBDD, que son conocidos como objetos de un esquema.

Estos objetos tienen un acceso directo al esquema del propietario. Debajo una lista con la enumeración de objetos de un esquema 👇



  * Tabla     --> Para el almacenamiento de datos
  * Vista     --> Para proyectar datos en un formato deseado desde una o más tablas
  * Secuencia --> Para generar valores númericos
  * Índice    --> Para mejorar el rendimiento de las consultas en tablas.
  * Sinónimo  --> Nombre similar/alternativo de un objeto
  
Uno de los primero(s) pasos a la hora de crear una BBDD, es crear las tablas que almacenarán los datos de una organización. Independientemente del tamaño y complejidad de una base de datos, cada una de estas se compone de **tablas**.

  ***
``CREACIÓN`` de una tabla

Sintáxis

```sql
CREATE TABLE [schema.]tabla
          ( { columna tipo_de_dato [expresion por defecto] [restriccion de columna CONSTRAINT] ... 
            | restriccion_tabla} 
         [, { column datatype [DEFAULT expression] [restriccion de columna CONSTRAINT] ... 
            | restriccion_tabla} ]...) 
         [AS subconsulta]
```
  * Es imprescindible tener como privilegio ``CREATE TABLE``.
  * Se ha de especificar:
      * El nombre de la tabla
      * Y para las columnas: Nombre, tipo de dato (datatype) y tamaño.
      
Ejemplo de creación emoji

```sql
CREATE SCHEMA 
```      
 

