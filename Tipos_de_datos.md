                                               Tipos de datos Numéricos
Integer --> Valores enteros

Numeric --> Numeros reales de (hasta) dígitos

Decimal --> Parecido al Numeric

Float   --> Número de coma flotante 

Char    --> Almacena de 1 .. 255 caracteres alfanuméricos

Varchar --> Igual al char, salvo que este, almacena los bytes en el valor campo


                                                    Operadores

1. Aritméticos   
   - (+)   SUMA
   - (-)   RESTA
   - (*)   PRODUCTO
   - (/)   DIVISIÓN
   - (**)  EXPONENTE

2. Relacionales
   - (<)     Menor que
   - (<=)    Menor o igual que
   - (>)     Mayor que
   - (>=)    Mayor o igual que
   - (<> !=) Distinto
   - (!<)    No menor que
   - (!>)    No mayor que
   
3. Lógicos
   - AND 
   - OR
   - NOT
              
4. Concatenación
   - (+)
   
                                             Funciones Agregadas                     
                     
MAX()   -->  Devuelve el valor máximo

MIN()   -->  Devuelve el valor mínimo

SUM()   -->  Extrae el valor de una suma
          
COUNT() -->  Nº de filas que cumplan la condición

AVG()   -->  Promedio de los valores de un campo


                                                 Predicados SQL
                                            
BETWEEN ... AND   Revisa que el valor está dentro de un intervalo

LIKE              Compara una cadena. Admite el uso de comodines (%)

ALL               Señala todos los elementos de una sub_consulta

ANY               Se ejecuta la condición si la comparación es cierta (Para al menos un elemento)

EXISTS            Devuelve TRUE si el resultado de la sub_consulta devuelve resultados

IN                Comprueba un campo si este se encuentra en determinado rango


### Tabla con sus tipos, categorías y definiciones...
<!-- Tabla de datos -->
| TIPO DE DATO  | CATEGORÍA |                             DEFINICIÓN                                                   |             
|---------------|-----------|------------------------------------------------------------------------------------------|
| INTEGER       | Numérico  | Es un número entero y a su vez el más empleado                                           |
| DECIMAL       | Numérico  | Es un núm. preciso. 131070 dígitos (antes de la coma) y 16385 dígitos (desp. de la coma) |               
| REAL          | Numérico  | Es nu número no preciso.                                                                 |
| CHAR          | Texto     | Longitud total y fija limitada                                                           |
| VARCHAR       | Texto     | Longitud variable                                                                        |
| TEXT          | Texto     | Longitud ilimitada variable                                                              |
| DATE          | Fecha     | La fecha del día. Usa 4 BYTES                                                            |
| TIME          | Fecha     | La hora del día. Usa 8 BYTES                                                             |
| TIMESTAMP     | Fecha     | La fecha y hora del día. Es una combinación de ``DATE`` + ``TIME``                       |
| BOOLEAN       | Booleano  | Indica si un valor es ``TRUE`` **OR** ``FALSE``. También puede ser ``NOT NULL``          |
| MONEY         | Dinero    | Número de precisión limitada. Hasta '4' cifras decimales. Se usa con **SUM**             |
| UUID          | OS        | Identificador universal único                                                            |
| JSON          | Fichero   | JavaScript Object Notation                                                               |
| XML           | Fichero   | Extensible Markup Language                                                               |    
| CIDR          | Network   | Direcciones IPV4 e IPV6. No permite bits distintos a '0' a la derecha de la máscara      |
| INET          | Network   | Direcciones IPV4 e IPV6.                                                                 |
<!-- Tabla de datos -->
