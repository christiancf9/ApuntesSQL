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
CREATE

La consula ``CREATE`` es usada para crear una base de datos u objetos, tales como tablas, vistas, almacenamientos procesados, etc

  
  
Creando una base de datos (BBDD)

El ejemplo siguiente demuestra como la consulta ``CREATE`` puede ser usada para crear una base de datos.

```sql
CREATE DATABASE LibreriaDB
```

CREANDO UNA TABLA

La consulta ``CREATE`` también es usada para añadir tablas en una BBDD existentes, tal y como muestra este script 👇

```sql CREATE TABLE Books
(
Id INT PRIMARY KEY IDENTITY(1,1),
Name VARCHAR (50) NOT NULL,
Price INT
` `

 

