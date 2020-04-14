 --> REVISAR DIBUJO ANTERIOR

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


### REVISAR LIBRETA
