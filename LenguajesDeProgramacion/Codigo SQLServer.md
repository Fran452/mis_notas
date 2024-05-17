<div id = "indice"> <!----- Inicio de indice ------->

# Indice

1. 
| [Tipos de datos](#datos)          |
|:---------------------------------:|
|[Datos numericos](#datos-numericos)|
|[Datos de texto](#datos-texto)     |
|[Datos fecha](#datos-fecha)        |

2. 
| [Constraints](#constraints)   |
|:-----------------------------:|
|[¿Que es?](#constraints-Que-es)|
|[Tipos](#constraints-tipos)    |

3. 
|[Funciones](#funciones)||
|:------------------:|--------------|
|[Crear](#funciones-crear)|
|[Eliminar](#funciones-eliminar)|
|[Editar](#funciones-editar)|[Estructura](#funciones-editar-estructura) <br> [Operadores](#funciones-editar-operadores)|

4. 
|[Funciones de Manipulacion](#funciones-manipulacion)||
|:------------------:|--|
|[Incertar](#funciones-manipulacion-Incertar)|
|[Modificar](#funciones-manipulacion-Modificar)|
|[Eliminar](#funciones-manipulacion-Eliminar)|
|[Seleccionar](#funciones-manipulacion-Seleccionar)|[Filtro](#funciones-manipulacion-Seleccionar-Filtro)<br> [Operadores](#funciones-manipulacion-Seleccionar-Operadores)|
|[Ordenar](#funciones-manipulacion-Ordenar)|
|[Apodar](#funciones-manipulacion-Apodar)|
|[Edicion](#funciones-manipulacion-Edicion)|
|[CASE](#funciones-manipulacion-CASE)|

5. 
|[Union de Tablas](#union-tablas)||
|:------------------:|-|
|[JOIN](#union-tablas-JOIN)|[otros JOIN](#union-tablas-JOIN-otros)
|[DISTINCT](#union-tablas-DISTINCT)|
|[GRUP](#union-tablas-GRUP)|
|[HAVING](#union-tablas-HAVING)|
6. 
|[Funciones de Agregación](#Funciones-agregación)|
|:------------------:| 

</div> <!----- Fin de Indice ------->

<br> 


## [Indice](#indice)

<div id = "datos"> <!----- Inicio de datos ------->

# Datos

<div id = "datos-numericos"> <!----- Inicio de numericos ------->

## Datos numericos 
| datos     |           definicion                  |
|:---------:|---------------------------------------|
|int        |innecesariamente grande para aclarar   |
|tinyint    |de -128 a 128                          |
|smallint   |de -32768 a 32768                      |
|mediumint  |de -8388608 a -8388608                 |
|biging     |innecesariamente grande para aclarar   |
|decimal    |decimales                              |
|float      |numeros con coma                       |

</div> <!----- Fin de numericos ------->
<div id = "datos-texto"> <!----- Inicio de texto ------->

## Datos de texto 
| datos         |           definicion                              | 
|:-------------:|---------------------------------------------------|
|CHAR(num)      |El numero indica la cantidad exacta de caractereres longitud fija tabla ASCII|
|VARCHAR(num)   |El numero indica el valor maximo de caracteres longitud variable tabla ASCII    |
|NCAHR()|El numero indica la cantidad exacta de caractereres longitud Unicode|
|NVARCHAR(num)   |El numero indica el valor maximo de caracteres longitud variable Unicode |
|TEXT           |               No tiene maximo                     |

* Unicode: caracteres extendidos de la tabla ASCII

</div> <!----- Fin de texto ------->
<div id = "datos-fecha"> <!----- Inicio de fecha ------->

## Datos fecha
| datos    |                   definicion                             | 
|:---------:|---------------------------------------------------------|
|date       |Fecha en formato YYY-MM-DD                               |
|time       |Almacena la hora en formato HH:MM:SS                     |
|datetime   |Almacena fecha y hora en anteriores formatos mencionados |

</div> <!----- Fin de fecha ------->
</div> <!----- Fin de datos ------->
 
## [Indice](#indice)
<div id = "constraints"> <!----- Inicio de constraints ------->

# Constraints
<div id = "constraints-Que-es"> <!----- Inicio de Que-es ------->

## ¿Que es?
Limitaciones en tipo de datos de una columna para mantener la integridad de nuestra base de datos. Estas estan diferenciadas de la validacion hecha anteriormente.

</div> <!----- Fin de Que-es ------->
<div id = "constraints-tipos"> </div> <!----- Inicio de tipos ------->

## Tipos
| tipos         |              definicion                               | 
|:-------------:|-------------------------------------------------------|
|NOT NULL       | Esta restriccion no te perimte guardar valores null   |
|UNIQUE         | No se perimte que haya dos filas con el mismo valors  |
|PRIMARY KEY    | Identificador de forma unica a una fila (obligatoria) |
|DEFAULT        | Aplica un valor por defecto                           |
|AUTO_INCREMENT | Generta un numero unico y lo incrementa automaticamente |
|IDENTYTY(valoresInicial,aumento)|Los valores creados ronda del valor incial aumentado segun se inidique|
|CONSTRAIRNT nombre|Se le agrega el nombre para poder identificarlo al momento del error|
|REFERENCE tabla|se utiliza para claves foraneas riferenciando la tabla|
|CHECK (bool)| Agrega una condicion para un capo|

</div> <!----- Fin de tipos ------->
</div> <!----- Fin de constraints ------->

## [Indice](#indice)
<div id = "funciones"> <!----- Inicio de funciones ------->

# Funciones
<div id = "funciones-crear"> <!----- Inicio de crear ------->

## Crear
```SQL
CREATE TABLE nombre_de_la_tabla(
    nombre_de_la_columna_1 TIPO_DE_DATO CONSTRAINTS,
    nombre_de_la_columna_2 TIPO_DE_DATO CONSTRAINTS,
    PRIMARY KET (variable_primaria),
    FOREIGN KEY(variable_foraneas) REFERENCES base_de-datos-variable
)
```
ejemplo: 
```SQL
CREATE TABLE productos(
    id INT NOT NULL AUTO_INCREMENT,
    nombre VARCHAR(100) NOT NULL,
    mail VARCHAR(100) NOT NULL UNIQUE,
    direccion_id INT,
    precio INT,
    PRIMARY KEy (id),
    FOREIGN KEY(direccion_id) REFERENCES direcciones(id),
    CONSTRAINT pro_pre CHECK (precio > 0)
)
```

</div> <!----- Fin de crear ------->
<div id = "funciones-eliminar"> <!----- Inicio de eliminar ------->

## Eliminar
`DROP TABLE IF EXIST nombre_de_la_tabla;`

</div> <!----- Fin de eliminar ------->
<div id = "funciones-editar"> <!----- Inicio de editar ------->

## Editar
<div id = "funciones-editar-estructura"> <!----- Inicio de estructura ------->

### Estructura
```SQL
ALTER TABLE productos(
    ADD id INT NOT NULL AUTO_INCREMENT,
    MODIFY nombre VARCHAR(100) NOT NULL,
    DROP mail
)
```

</div> <!----- Fin de estructura ------->
<div id = "funciones-editar-operadores"> <!----- Inicio de operadores ------->

### Operadores
|Operador   |   Funcion                 | 
|:---------:|---------------------------|
|ADD        | Para agregar una columna  |
|MODIFY     | Para modificar una columna|
|DROP       | Para borrar una columna   |

</div> <!----- Fin de operadores ------->
</div> <!----- Fin de editar ------->
</div> <!----- Fin de funciones ------->

## [Indice](#indice)
<div id = "funciones-manipulacion"> <!----- Inicio de manipulacion ------->

# Manipulacion de datos

<div id = "funciones-manipulacion-Incertar"> <!----- Inicio de Incertar ------->

## Incertar Datos
Con cada uno de los campos
```SQL
INSERT INTO tabla VALUES (valor1,valor2,valor3)
```
si no queremos aclarar cada campo<br>
`INSERT INTO tabla(campo1,campo2,campo3) VALUE (valor1,valor2,valor3)`

</div> <!----- Fin de Incertar ------->
<div id = "funciones-manipulacion-Modificar"> <!----- Inicio de Modificar ------->

## Modificar Datos
```SQL
UPDATE movie 
SET modifiacion  
WHERE criterio
```

</div> <!----- Fin de Modificar------->
<div id = "funciones-manipulacion-Eliminar"> <!----- Inicio de Eliminar ------->

## Eliminar datos
`DELETE FROM MOVIE WHERE bool`

</div> <!----- Fin de Eliminar ------->
<div id = "funciones-manipulacion-Seleccionar"> <!----- Inicio de Seleccionar ------->

## Seleccionar
solicita todos los datos * de una tabla <br>
`SELECT * FROM movies` <br>
si quiero solicitar X campo:<br>
`SELECT campo1,campo2,campo3 FROM movies` <br>
Si se quiere solicitar varias tablas siendo Tabla el nombre de la tabla y tabla1 un apodo para luego usarse <br>
`SELECT tabla1.campo tabla2.campo FROM Tabla1 tabla1, Tabla2 tabla2

<div id = "funciones-manipulacion-Seleccionar-Filtro"> <!----- Inicio de Filtro ------->

### Seleccionar segun filtro
se solicita el filtro agregando WHEARE y la condicion: <br>
`SELECT * FROM movies WHERE rating > 5` <br>
para agregar mas de un filtro se agrega AND o OR.

</div> <!----- Fin de Filtro ------->
<div id = "funciones-manipulacion-Seleccionar-OperadoresLogicos"> <!----- Inicio de Logicos Comparacion------->

### Operadores Logicos
|Operador   |   Funcion                 | 
|:---------:|---------------------------|
| `AND`     | los dos valores true para que se valide|   
| `OR`      | con que un valor sea true se valida|


</div> <!----- Fin de Operadores Logicos------->
<div id = "funciones-manipulacion-Seleccionar-OperadoresComparacion"> <!----- Inicio de Operadores Comparacion------->

### Operadores Comparacion
|Operador   |   Funcion                 | 
|:---------:|---------------------------|
| `=`       | Igual a                   |   
| `>`       | Mayor que                 |
| `>=`      | Mayor o igual que         |
| `<`       | Menor que                 |
| `<=`      | Menor o igual que         |
| `<>`      | Diferente a               |
| `!=`      | Diferente a               |
| `IS NULL` | Es null    |
| `NOT NULL` | No es null                     |
| `BETWEEN valor AND valor` | Entre dos valores
| `IN`      | Lista de valores          |
| `LIKE ("string")`    | Se ajusta a la estring. Puede ser (%string => termina) (string% => inicia) (%string% => contiene)
|`LIMIT int`| no selecciona hasta el limite. va al final de todas las sentencias 
|`OFFSET int`| nos saltea los primeros int resultados al final de todo despues de LIMIT
| `EXISTS` | Existencia de un dato |


</div> <!----- Fin de Operadores Comparacion------->
</div> <!----- Fin de Seleccionar -------> 
<div id = "funciones-manipulacion-Ordenar"> <!----- Inicio de Ordenar ------->

### Ordenar datos seleccionados
Se ordenan los datos agregando ORDER BY campo <br>
`SELECT * FROM movies ORDER BY campo` <br>
si se quiere ordenar de mayor a menor se le agrega al final del campo un DESC<br>
`SELECT * FROM movies ORDER BY campo DESC` <br>
y para agregar una regla de desenpate se hace de la siguente forma: <br>
`SELECT * FROM movies ORDER BY campo DESC, campoDesenpate`

</div> <!----- Fin de Ordenar ------->
<div id = "funciones-manipulacion-Apodar"> <!----- Inicio de Apodar ------->

### Darle un apodo a los campos:
para darle un apodo a los campos seleccionados se le agrega el nombre original mas AS y el apodo dado como en el siguiente ejmplo: <br>
`SELECT nombreOrigina AS apodo FROM movies`

</div> <!----- Fin de Apodar ------->
<div id = "funciones-manipulacion-Edicion"> <!----- Inicio de Edicion ------->

## Funciones de edicion
|Operador   |   Funcion                 | 
|:---------:|---------------------------|
|`CONCAT (columna,columna)`| junta dos columnas en una sola
|`CALESCE(columna,valor)`| nos permite mostrar valor en las filas con columnas NULL
|`NOW()`| nos trae la feha actual
|`DATEDIFF(fecha1, fecha2)`| sirve para comparar dos fechas
|`EXTRACT(dato FROM columna)`| sirve para extraer el valor de la columna dependiendo del dato
|`DATE_FORMAT(columna, "%D/%M/%Y")`| Sirve para definier el formato del dia en el que se le de.
|`REPLACE(columna,variable,variableRemplazante)`| Remplaza la variable con variableRemplazante en la columna seleccionada
|`LENGHT(columna)`| Te da el tamaño de los datos almacenados dentro de la columna
|`COALESCE(variable,variable,variable)`| Te toma el primer valor no null de los x

</div> <!----- Fin de Edicion ------->
<div id = "funciones-manipulacion-CASE"> <!----- Inicio de CASE ------->

## CASE
Se selecciona distintos casos como en la estructura: <br>
```
CASE
    WHEN bool THEN valor
    WHEN bool THEN valor
    ELSE valor
END
```
Ejemplo
```sql
SELECT clie_razon_social AS [Razon Social], clie_telefono AS Telefono, clie_codigo,
CASE WHEN clie_limite_credito < 100 THEN 'Poco'
	 WHEN clie_limite_credito BETWEEN 100 AND 4000 THEN 'Moderado'
	 WHEN clie_limite_credito > 4000 THEN 'Alto'
	 END AS Credito, clie_domicilio 
FROM Cliente
```

</div> <!----- Fin de CASE ------->
</div> <!----- Fin de manipulacion ------->

## [Indice](#indice)
<div id = "union-tablas"> <!----- Inicio de union ------->

# Union de tablas

<div id = "union-tablas-JOIN"> <!----- Inicio de JOIN ------->

## INNER JOIN
```
SELECTO movies.id, campo2,campo3
FROM tabla
INNER JOIN tablaAUnir ON campoTabala = campoTablaB
```

</div> <!----- Fin de JOIN ------->
<div id = "union-tablas-JOIN-otros"> <!----- Inicio de otros ------->

### Otras variables:
|Operador   |   Funcion                 | 
|:---------:|---------------------------|
|`LEFT JOIN` | tabla de la izquierda va a ser aceptado aun no tiendo vinculo
|`RIGHT JOIN`| tabla de la derecha va a ser aceptada aun sin vinculos

</div> <!----- Fin de otros ------->
<div id = "union-tablas-DISTINCT"> <!----- Inicio de DISTINCT ------->

## DISTINCT
Elimina duplicados 100% iguales en sus filas  <br>
`SELECTO DISTINCT movies.id, campo2,campo3 FROM tabla`

</div> <!----- Fin de DISTINCT ------->
<div id = "union-tablas-GRUP"> <!----- Inicio de GRUP ------->

## GROUP BY  
Se crean grupos por diferentes categorias para aplicarle diferentes funciones:<br>
`GROUP BY campoDeAgrupacion`<br> 

</div> <!----- Fin de GRUP ------->
<div id = "union-tablas-HAVING"> <!----- Inicio de HAVING ------->

## HAVING
Agrega condiciones a los datos agrupados <br>
`GRUP BY campoDeAgrupacion HAVING condicionDeGrupacion`<br> 

</div> <!----- Fin de HAVING ------->
</div> <!----- Fin de union ------->


## [Indice](#Indice_)
<div id = "Funciones-agregación"> <!----- Inicio de agregación ------->

# Funciones de agregación
|Operador   |   Funcion                 | 
|:---------:|---------------------------|
|`COUNT(*)`         | Nos suma la cantidad de filas que hay en una tabla segun el campo
|`MAX(campo)`       | Nos devuelve el campo maximo de la tabla segun el campo
|`MIN(campo)`       | Nos devuelve el campo minimo de la tabla segun el campo
|`SUM(campo)`       | Hace la sumatoria de todos la tambla segun el campo
|`AVG(campo)`       | Saca el promedio de todas las filas segun el campo

</div> <!----- Fin de agregación ------->




## [Indice](#indice)
<div id = "Indice"> <!----- Inicio de Indice ------->

# Indices

<div id = "Indice-QueEs"> <!----- Inicio de Que Es ------->

## ¿Que es?
Son estructuras fisicas adicionales. Que van a tener una independencia tanto logica como fisica de la tabla. No es parte de la tabla. 

</div> <!----- Fin de Que Es ------->

<div id = "Indice-Utilizacion"> <!----- Inicio de Utilizacion ------->

## Cuando se utiliza
Al momento de insertar tanto PK o UNIK se insertan automaticamente los indices. Si mi tabla requiere mostrar mas registros no es encesario utilizar indices.

</div> <!----- Fin de Utilizacion ------->
</div> <!----- Fin de Indice ------->

## [Indice](#indice)
<div id = "TiposDeTabla"> <!----- Inicio de TiposDeTabla ------->

# Tipo de tablas
## Parametricas
Son tablas que se ingresan por teclado. Son casos particulares de los parametros del sistema.

## Maestras
Son tablas que se ingresan por teclado. Son datos del modelo (productos, clientes, etc)

## Transaccionales
Estas tablas siempre se crean los registros con un procesos donde interactuan otras tablas transaccionales o parametricas maestras. Siempre se incertan por un proceso

</div> <!----- Fin de TiposDeTabla ------->


## [Indice](#indice)
<div id = "FuncionesDeMotor"> <!----- Inicio de Funciones de motor ------->

# Funciones de motor
<div id = "FuncionesDeMotor-QueEs"> <!----- Inicio de Que es ------->

## ¿Que son?
Son funciones que cada motor tiene y puede variar segun el motor. En el texto usamos SQLServer para estas funciones

</div> <!----- Fin de Que es ------->
<div id = "FuncionesDeMotor-Funciones"> <!----- Inicio de Funciones ------->


## Funciones

|Operador   |   Funcion                 | 
|:---------:|---------------------------|
|`ISNULL(param1,param2)`|Sirve para todo tipo de datos, si param1 no es null recive ese valor de serlo lo cambia por el param2|
|`ROUND(param1,param2)`|Esta funcion redoneda el numero param1 a la cantidad que se le indique en param2|
|`ABS(param)`|Pone param en valor absoluto osea positivo|
|`YEAR(param)`|Toma de param el año, siendo param una fecha el dato resultante es numerico|
|`MONTH(param)`|Toma de param el mes, siendo param una fecha el dato resultante es numerico|
|`DATEDIF(param1,param2,param3)`|Toma tres parametros, param1 es la unidad de medida (YEAR,DAY,MONTH)y tanto param2 como param3 los años y se comparan segun la unidad de medida|
|`DATEDADD(param1,param2,param3)`|Toma tres parametros, param1 es la unidad de medida (YEAR,DAY,MONTH), param2 es la cantidad a sumarsey param3 el año a el cual se le va a sumar|
|`SPACE(param)`|Agrega la cantidad de espacios en blaco que se indiquen en param|
|`UPPER(param)`|Pone el parametro a mayusculas|
|`CHARINDEX(param1,param2)`|Busca el string indicado en param1 en la fila indicada en param2|
|`RTRIM(param)`|Le saca todos los espacios a la derecha del parametro|
|`CONCAT(param1,param2,param3,paramn)`|Concatena todos los aparametros dentro de los parentesis|
|`LEN(param)`|cantidad de caracteres de param|
|`LTRIM(param)`|Saca los espacios a izquierda de param|
|`SUBSTRING(param1,param2,param3)`|param1 es el string total param2 a partir de que columna toma el strign y param3 cuanto toma a partir de param2|
|`CONVERT(param1,param2,param3)`|........................|
|`CAST(param AS variable)`|Convierte param en la variable que se necesite|
|`REPLICATE(param1,param2)`|repite param1 la cantidad de veces que indica param2|

</div> <!----- Fin de Funciones ------->
</div> <!----- Fin de Funciones de motor ------->
