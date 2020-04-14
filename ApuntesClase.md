## REVISAR LIBRETA Y GISTHUB

Componentes de SQL (SQL Ansi 92):
  - DDL (Data Definition Language): Su función es la de definir la Base de Datos, tablas, vistas e índices [CREATE, ALTER, DROP, TRUNCATE, COMMENT, RENAME]
  - DML (Data Manipulation Language): Su función es la manipulación de datos. Podemos seleccionar, insertar, eliminar y actualizar datos. [INSERT, UPDATE, DELETE]
  - DCL (Data Control Language): Es el encargado de la seguridad de datos, permisos y accesos  [GRANT, REVOKE]
  - DRL/DQL (Data Retrieval Language / Data Query Language): Es usado para selecionar los datos en una base de datos... [SELECT]
  - TCL (Transact Query Language): Se usa para administrar diferentes transacciones en una BBDD...  [COMMIT, ROLLBACK]


```SQL
[CONSTRAINT] <nome-da-restricción>]
      UNIQUE (<atributos>),
[[NOT]] DERERRABLE
[INITIALLY INMEDIATE | DEFERRABLE]
```


```SQL
CHECK saldo >= (
     SELECT saldo
     FROM empregado
     WHERE departamento='A'
)
```

```SQL
DROP TABLE
     SELECT saldo
     FROM empregado
     WHERE departamento='A'
)
```

TIPOS (DML) --> INSERT, UPDATE y DELETE.

``INSERT``

INSERT INTO nome-da-taboa
[(atributo 1, atributo 2)]
(VALUES (valor1, valor2) | SELECT ...)
  - TIPOS DE DATOS
    --> DATETIME
    --> NCHAR
    --> INTEGER

EJEMPLOS DE VALORES

(1, 'cheese', 9.99)
(2, '')


``UPDATE``

UPDATE world
  SET name = 'España',
  continent = 'Africa',
WHERE name = 'Spain',


``DELETE``

DELETE FROM
  nome-da-taboa
[WHERE predicado]


## REVISAR LIBRETA Y GISTHUB
