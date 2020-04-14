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
***
CREATE

La consula ``CREATE`` es usada para crear una base de datos u objetos, tales como tablas, vistas, almacenamientos procesados, etc

  
  
**CREANDO UNA BBDD** - [**``CREATE DATABASE``** | **``CREATE SCHEMA``**]


El ejemplo siguiente demuestra como la consulta ``CREATE`` puede ser usada para crear una base de datos.

```sql
CREATE DATABASE LibreriaDB [IF NOT EXISTS] <nombreBBDD>
                           [CHARACTER SET <nombreCharset>] 
                           [COLLATE <nombreCollate>];
```

Otro ejemplo

```sql
CREATE SCHEMA LibreriaDB [IF NOT EXISTS] <nombreBBDD>
                         [CHARACTER SET <nombreCharset>] 
                         [COLLATE <nombreCollate>];
```

NOTA: La diferencia es inexistente en MySQL, pero no en PostgreSQL, donde ``SCHEMA`` añade atributos de permiso. En la práctica se aconseja usar ``SCHEMA``

- `[IF NOT EXISTS]`: Este campo es opcional. Revisa si la BBDD que vayamos a crear exista (o no) en nuestro sistema gestor de base de datos...
- `CHARACTER SET`: Este campo es opcional. Establece un parámetro de conjunto de caracteres que se vaya a utilizar... Ejemplo: UTF-8
- `COLLATE`: Este campo es opcional. Junto a CHARACTER_SET, establece la variante específica global Ejemplo: utf8_unicode_ci


**CREANDO UNA TABLA - [CREATE TABLE]**

La consulta ``CREATE`` también es usada para añadir tablas en una BBDD existentes, tal y como muestra este script 👇

```sql 
CREATE TABLE Libros (
    Nombre VARCHAR (50) NOT NULL,
    Precio CHAR(10)
);
```
**AÑADIENDO ATRIBUTOS**

- Más adelante, veremos que a la hora de declarar atributos, podemos aplicar ciertas RESTRICCIONES (**CONSTRAINT**)

Ejemplo
```sql 
CREATE TABLE Libros (
    Id INT PRIMARY KEY IDENTITY(1,1),
    Nombre VARCHAR (50) NOT NULL,
    Precio CHAR(10)
    
    CONSTRAINT PK_Libros
            PRIMARY KEY (Precio)
);
```
 

