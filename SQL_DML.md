
                                                         SENTENCIAS DML
                                        
# DEFINICIÓN
Usando sentencias **``DML``** formaremos instrucciones con la capacidad de modificar datos en las tablas creadas previamente.

Una agrupación de instrucciones DML, que se ejecutan consecutivamente, se denominan transacciones.

  > Esta opera sobre los objetos en una base de datos, es decir sobre su estructura

Veremos más adelante, ejemplos de su uso... 👇
  > Para guardar los datos, usaremos la sentencia ``COMMIT``
  > Para cancelar lo que hayamos insertado, usaremos la sentencia ``ROLLBACK``
***
***
# INDICE <a name="INDICE"></a>
1. ⚡ [DML - INSERT](#dml_insert)
2. ⚡ [DML - UPDATE](#dml_update)
3. ⚡ [DDL - DELETE](#dml_delete)
***
## INSERT <a name="dml_insert"></a>

La consula ``INSERT`` es usada para añadir filas a una tabla


```sql
  INSERT INTO <nombre-tabla> [ (<ejemploAtributo1>, <ejemploAtributo2>] 
  VALUES (<valor1>, <valor2>)

```

El orden en que se les asignen los valores en ``VALUES`` tiene que coincidir el orden con el que se han definido las columnas en la creación de una tabla ``INSERT``. Los valores son asignados mediante un posicionamiento relativo 
 

Ejemplos 👇
```sql
INSERT INTO EDADES
VALUES (1,'WILSON');
```

```sql
INSERT INTO PAQUETES (CODPEDIDO,ESTADO)
VALUES (130,1);
```
### INSERCCIÓN DE SENTENCIAS CON MÚLTIPLES FILAS [``INSERT`` + ``SELECT``]
En este caso, para introducir un sub-conjunto de fila(s) de una tabla dentro de otra, se escribe solamente una sentencia ``INSERT`` y una sentencia ``SUBSELECT`` interna (es decir, dentro de ella...) Ejemplo:

```sql
INSERT INTO tabla1 (columna1, columna2, columna3...)
SELECT ([sentencia SELECT]);
```

```sql
INSERT INTO PAQUETES (CODPEDIDO,ESTADO,NOMAPELLIDO)
SELECT CODPEDIDO+75,ESTADO,NOMAPELLIDO FROM PAQUETES WHERE CODPEDIDO IN (0,1,2);
```
  > Referencia a las columnas los valores que han sido recuperados mediante la sentencia ``SELECT``.
  > Añade en la tabla en su totalidad, las filas que se recuperen mediante la sentencia ``SELECT``.


## UPDATE <a name="dml_update"></a>

La consula ``UPDATE`` es usada para actualizar valores, en una o varias columnas (para un subconjunto de tuplas de una tabla).


```sql
  UPDATE <tablaEjemplo>
  SET <atributo1> = <ejemploValor1>, <columna2> = <ejemploValor2>, <columna3> = <ejemploValor3>...
  [WHERE <predicado>];

```
