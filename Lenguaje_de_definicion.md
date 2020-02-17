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
    SELECT 
          matricula, 
          marca,
          modelo,
          color,
          numero_kilometros,
          num_plazas 
FROM 
   coches
WHERE 
    matricula = '1234CCF';
```

**ORDER BY** permite especificar el orden de los datos a ser devueltos.

```SQL
    SELECT 
          matricula, 
          marca,
          modelo,
          color,
          numero_kilometros,
          num_plazas 
FROM 
   coches
ORDER BY marca ASC, modelo DESC;
```
                                       Consultas combinadas (JOINS)

**JOIN** permite unir dos o más tablas. Existen diferentes tipos:

1. JOIN
   - LEFT  [OUTER] JOIN --> Ignora los valores del lado _derecho_ igual que los valores del lado izq. que no son nulos
   - RIGHT [OUTER] JOIN --> Ignora los valores del lado _izquierdo_ igual que los valores del lado der. que no son nulos
   - INNER JOIN         --> Une todos los valores, tanto del lado _izquierdo_ como _derecho_

