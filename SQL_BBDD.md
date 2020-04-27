                                                CREACIÓN DE UNA BASE DE DATOS (BBDD)
                                        
# DEFINICIÓN
Una base de datos es una colección organizada de información estructurada, o datos, típicamente almacenados electrónicamente en un sistema informático. Una base de datos generalmente está controlada por un sistema de gestión de bases de datos (SGBD).

Un sistema de administración de bases de datos (SGBD) es un paquete de software diseñado para definir, manipular, recuperar y administrar datos en una base de datos. Un SGBD generalmente manipula los datos en sí, el formato de datos, los nombres de campo, la estructura de registros y la estructura de archivos. También define reglas para validar y manipular estos datos.

Un SGBD libera a los usuarios de los programas de una trama para el mantenimiento de datos. Los lenguajes de consulta de cuarta generación, como SQL, se usan junto con el paquete SGBD para interactuar con una base de datos.

Algunos ejemplos de SGBD son los siguientes:

  - MySQL / MariaDB
  - SQL Server
  - Oracle
  - dBASE
  - FoxPro
  - ...
  
***
***
# ÍNDICE <a name="sql-bbdd_index"></a>
1. ⚡ [ANTES DE LA CREACIÓN](#sql_before-create)
2. ⚡ [CREACIÓN BBDD - PROYECTO DE INVESTIGACIÓN](#sql_proyecto-investigacion)
3. ⚡ [CREACIÓN BBDD - NAVES ESPACIALES](#sql_naves-espaciales)
***

## ANTES DE LA CREACIÓN (REPASO) <a name="sql_before-create"></a>
Antes de nada, revisaremos que el proceso de mysql se está ejecutando correctamente...

Para ello escribiremos el siguiente comando

```console
christian@christian-VirtualBox:~$ systemctl status mysql.service
```

![SYSTEMCTL_REPASO](./imagenes/repaso_systemctl.png)
  > Podemos observar que el servicio `MySQL` se está ejecutando correctamente..
  > Systemctl no funciona con el usuario `root`

Lo que haremos ahora, será iniciar el MySQL en modo root (como ya habíamos configurado previamente en SQL_DDL) 😎

Para ello, teclearemos el siguiente comando:

```console
christian@christian-VirtualBox:~$ mysql -u root -p
```
![MySQL_ROOT_USER](./imagenes/repaso_mysql_user_root.png)
  > Como ya hicimos la autenticación de contraseña para el usuario root, procederemos a usar dicho usuario...

👁 [ÍNDICE](#sql-bbdd_index)

Una vez iniciado con el usuario root, en la shell de MySQL, procederemos a crear una BBDD de prueba...

Para ello en MySQL, teclearemos lo siguiente

```sql
CREATE DATABASE REPASO_BBDD;
```
![CREATE_BBDD_REPASO](./imagenes/repaso_create_bbdd.png)
  > 🛡NOTA: En MySQL, no existe ninguna diferencia entre `CREATE SCHEMA` y `CREATE DATABASE`.
  > En otros SGBD (Ej: Oracle) si existe diferencia (Permisos...)

```sql
SHOW DATABASES;
```
![SHOW_DATABASE_REPASO](./imagenes/repaso_show-bbdd.png)

👁 [ÍNDICE](#sql-bbdd_index)

Una vez creada la BBDD anterior, procederemos a eliminarla...

Escribimos 👇

```sql
DROP DATABASE REPASO_BBDD;
```
![DROP_DATABASE_REPASO](./imagenes/repaso_drop_database.png)
  > 🛡PELIGRO: Cuidado con la sentencia `DROP`, una vez ejecutada ya no se puede revertir...
  
Y comprobamos 🤞

```sql
SHOW DATABASES;
```
![SHOW_DATABASE_REPASO2](./imagenes/repaso_show-bbdd_2.png)

👁 [ÍNDICE](#sql-bbdd_index)

## CREACIÓN BBDD - PROYECTO DE INVESTIGACIÓN [MANUAL] <a name="sql_proyecto-investigacion"></a>

Para el ejercicio de 'Proyecto de Investigación', crearemos la BBDD paso a paso, explicando la mayor parte de cosas (en lo posible)

[CÓDIGO de *proyecto de investigación* (GIST)](https://gist.github.com/christiancf9/cdb0675917f45ac279680d89928ffe5f)

### CREACIÓN DE LA BASE DE DATOS - (PROYECTO DE INVESTIGACIÓN)

Lo primero, antes de nada, crearemos la base de datos...

```sql
CREATE DATABASE Proyecto_de_Investigacion;
```
![CREATE DATABASE - PROYECTO DE INVESTIGACION](./imagenes/create_database_proyecto-de-investigacion.png)

Lo siguiente será seleccionar dicha base de datos (Para ello mostraremos las disponibles) 👇

```sql
SHOW DATABASES;
```

```sql
USE Proyecto_de_Investigacion;
```

![MOSTRAR Y SELECCIONAR LA BBDD](./imagenes/show_and_use-databases.png)

### CREACIÓN Y ALTERACIÓN DE TABLAS - (PROYECTO DE INVESTIGACIÓN)

Ahora que hemos creado la BBDD, nos tocará dar paso a la creación de tablas... Para ello, iremos captura por captura, enseñando el proceso de creación de cada una...

#### CREACIÓN TABLA SEDE - (PROYECTO DE INVESTIGACIÓN)

![CREACIÓN DE TABLA_SEDE](./imagenes/create_table-sede.png)

#### CREACIÓN TABLA DEPARTAMENTO - (PROYECTO DE INVESTIGACIÓN)

![CREACIÓN DE TABLA_DEPARTAMENTO](./imagenes/create_table-departamento.png)

#### CREACIÓN TABLA UBICACIÓN - (PROYECTO DE INVESTIGACIÓN)

![CREACIÓN DE TABLA_UBICACIÓN](./imagenes/create_table-ubicación.png)

#### CREACIÓN TABLA GRUPO - (PROYECTO DE INVESTIGACIÓN)

![CREACIÓN DE TABLA_GRUPO](./imagenes/create_table-grupo.png)

#### CREACIÓN TABLA PROFESOR - (PROYECTO DE INVESTIGACIÓN)

![CREACIÓN DE TABLA_PROFESOR](./imagenes/create_table-profesor.png)

#### CREACIÓN TABLA PROYECTO - (PROYECTO DE INVESTIGACIÓN)

![CREACIÓN DE TABLA_PROYECTO](./imagenes/create_table-proyecto.png)

#### ALTERACIÓN TABLA DEPARTAMENTO - (PROYECTO DE INVESTIGACIÓN)

![ALTERACIÓN DE TABLA_PROGRAMA](./imagenes/alter_table-departamento.png)

#### ALTERACIÓN TABLA GRUPO - (PROYECTO DE INVESTIGACIÓN)

![ALTERACIÓN DE TABLA_FINANCIA](./imagenes/alter_table-grupo.png)

#### CREACIÓN TABLA PARTICIPA - (PROYECTO DE INVESTIGACIÓN)

![CREACIÓN DE TABLA_PARTICIPA](./imagenes/create_table-participa.png)

#### CREACIÓN TABLA PROGRAMA - (PROYECTO DE INVESTIGACIÓN)

![CREACIÓN DE TABLA_PROGRAMA](./imagenes/create_table-programa.png)

#### CREACIÓN TABLA FINANCIA - (PROYECTO DE INVESTIGACIÓN)

![CREACIÓN DE TABLA_FINANCIA](./imagenes/create_table-financia.png)

#### ALTERACIÓN TABLA FINANCIA_1 - (PROYECTO DE INVESTIGACIÓN)

![ALTERACIÓN DE TABLA_PROGRAMA](./imagenes/alter_table-financia_1.png)

#### ALTERACIÓN TABLA FINANCIA_2 - (PROYECTO DE INVESTIGACIÓN)

![ALTERACIÓN DE TABLA_FINANCIA](./imagenes/alter_table-financia_2.png)
