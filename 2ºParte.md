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
