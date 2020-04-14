
                                                         SENTENCIAS DML
                                        
# DEFINICIÓN
Usando sentencias **``DML``** formaremos instrucciones con la capacidad de modificar datos en las tablas creadas previamente.

Una agrupación de instrucciones DML, que se ejecutan consecutivamente, se denominan transacciones.

  > Esta opera sobre los objetos en una base de datos, es decir sobre su estructura

Veremos más adelante, ejemplos de su uso...
***
***
# INDICE <a name="INDICE"></a>
1. ⚡ [DML - INSERT](#dml_insert)
2. ⚡ [DML - UPDATE](#dml_update)
3. ⚡ [DDL - DELETE](#dml_delete)
***
# INSERT <a name="dml_insert"></a>

La consula ``INSERT`` es usada para añadir filas a una tabla


```sql
  INSERT INTO <nombre-tabla> [ (atributo1, atributo2] 
  VALUES (<valor1>, <valor2>)

```

El orden en que se les asignen los valores en ``VALUES`` tiene que coincidir el orden con el que se han definido las columnas en la creación de una tabla ``INSERT``. Los valores son asignados mediante un posicionamiento relativo 
  > Para guardar los datos, usaremos la sentencia ``COMMIT``
  > Para cancelar lo que hayamos insertado, usaremos la sentencia ``ROLLBACK``

