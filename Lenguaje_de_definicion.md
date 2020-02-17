                                                SENTENCIAS
                                              
**SELECT** nos permite consultar los datos almacenados.

```SQL
SELECT
    <nombre_campo> 
FROM
    <nombre_tabla>
WHERE 
    <condicion>;
```

**FROM** nos indica que los datos serán recuparados de una tabla. Se pueden introducir varias tablas en las subconsultas o consultas combinadas


```SQL
SELECT
    *
FROM
    coches
WHERE 
    marca, modelo;
```

**WHERE** nos permite filtrar el resultado de una clausula `SELECT`

```SQL
    SELECT matricula, 
                marca,
                modelo,
                color,
                numero_kilometros,
                num_plazas 
FROM 
   coches
WHERE 
    matricula = 'M-1525-ZA';
```
