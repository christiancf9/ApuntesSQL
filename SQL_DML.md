
                                                         SENTENCIAS DML
                                        
# DEFINICIÓN
Usando sentencias **``DML``** formaremos instrucciones con la capacidad de modificar datos en las tablas creadas previamente.

Una agrupación de instrucciones DML, que se ejecutan consecutivamente, se denominan transacciones.

  > Esta opera sobre los objetos en una base de datos, es decir sobre su estructura

Veremos más adelante, ejemplos de su uso...

***
# INDICE <a name="INDICE"></a>
1. ⚡ [DML - INSERT](#dml_insert)
2. ⚡ [DML - UPDATE](#dml_update)
3. ⚡ [DDL - DELETE](#dml_delete)
***
# INSERT <a name="dml_insert"></a>

La consula ``INSERT`` es usada para añadir filas a una tabla


```sql
  INSERT INTO <ejemploTabla> [ (atributo1, atributo2] 
  VALUES (<valor1>, <valor2>)


```

### CREANDO UNA BBDD - [``CREATE DATABASE`` | ``CREATE SCHEMA``]

El ejemplo siguiente demuestra como la consulta ``CREATE`` puede ser usada para crear una base de datos.

```sql
CREATE DATABASE LibreriaDB [IF NOT EXISTS] <nombreBBDD>
                           [CHARACTER SET <nombreCharset>] 
                           [COLLATE <nombreCollate>];
```
