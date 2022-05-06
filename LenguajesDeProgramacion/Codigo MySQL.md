<div id = "indice">

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
</div>


<br> 


## [Indice](#Indice)
<div id = "datos">null
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
</div>
<div id = "datos-texto">

## Datos de texto 
| datos         |           definicion                              | 
|:------ ------:|---------------------------------------------------|
|char(num)      |El numero indica la cantidad exacta de caractereres|
|varchar(num)   |El numero indica el valor maximo de caracteres     |
|text           |               No tiene maximo                     |
</div>
<div id = "datos-fecha">

## Datos fecha
| datos    |                   definicion                             | 
|:---------:|---------------------------------------------------------|
|date       |Fecha en formato YYY-MM-DD                               |
|time       |Almacena la hora en formato HH:MM:SS                     |
|datetime   |Almacena fecha y hora en anteriores formatos mencionados |
</div> </div>

## [Indice](#Indice)
<div id = "constraints">

# Constraints
<div id = "constraints-Que-es">

## ¿Que es?
Limitaciones en tipo de datos de una columna para mantener la integridad de nuestra base de datos. Estas estan diferenciadas de la validacion hecha anteriormente.
</div>
<div id = "constraints-tipos">

## Tipos
| tipos         |              definicion                               | 
|:-------------:|-------------------------------------------------------|
|NOT NULL       | Esta restriccion no te perimte guardar valores null   |
|UNIQUE         | No se perimte que haya dos filas con el mismo valors  |
|PRIMARY KEY    | Identificador de forma unica a una fila (obligatoria) |
|DEFAULT        | Aplica un valor por defecto                           |
|AUTO_INCREMENT | Generta un numero unico y lo incrementa automaticamente |
</div> </div>

## [Indice](#Indice)
<div id = "funciones">

# Funciones
<div id = "funciones-crear">

## Crear
```
CREATE TABLE nombre_de_la_tabla(
    nombre_de_la_columna_1 TIPO_DE_DATO CONSTRAINTS,
    nombre_de_la_columna_2 TIPO_DE_DATO CONSTRAINTS,
    PRIMARY KET (variable_primaria),
    FOREIGN KEY(variable_foraneas) REFERENCES base_de-datos-variable(id)
)
```
ejemplo: 
```
CREATE TABLE productos(
    id INT NOT NULL AUTO_INCREMENT,
    nombre VARCHAR(100) NOT NULL,
    mail VARCHAR(100) NOT NULL UNIQUE,
    direccion_id INT,
    PRIMARY KEy (id),
    FOREIGN KEY(direccion_id) REFERENCES direcciones(id)
)
```
</div>
<div id = "funciones-eliminar">

## Eliminar
`DROP TABLE IF EXIST nombre_de_la_tabla;`
</div>
<div id = "funciones-editar">

## Editar
<div id = "funciones-editar-estructura">

### Estructura
```
ALTER TABLE productos(
    ADD id INT NOT NULL AUTO_INCREMENT,
    MODIFY nombre VARCHAR(100) NOT NULL,
    DROP mail
)
```
</div>
<div id = "funciones-editar-operadores">

### Operadores
|Operador   |   Funcion                 | 
|:---------:|---------------------------|
|ADD        | Para agregar una columna  |
|MODIFY     | Para modificar una columna|
|DROP       | Para borrar una columna   |
</div> </div> </div>

## [Indice](#Indice)
<div id = "funciones-manipulacion">

# Manipulacion de datos

<div id = "funciones-manipulacion-Incertar">

## Incertar Datos
Con cada uno de los campos
```
INSERT INTO tabla VALUES (valor1,valor2,valor3)
```
si no queremos aclarar cada campo<br>
`INSERT INTO tabla(campo1,campo2,campo3) VALUE (valor1,valor2,valor3)`
</div>
<div id = "funciones-manipulacion-Modificar">

## Modificar Datos
```
UPDATE movie 
SET modifiacion  
WHERE criterio
```
</div>
<div id = "funciones-manipulacion-Eliminar">

## Eliminar datos
`DELETE FROM MOVIE WHERE bool`
</div>
<div id = "funciones-manipulacion-Seleccionar">

## Seleccionar
solicita todos los datos * de una tabla <br>
`SELECT * FROM movies` <br>
si quiero solicitar X campo:<br>
`SELECT campo1,campo2,campo3 FROM movies` <br>


<div id = "funciones-manipulacion-Seleccionar-Filtro">

### Seleccionar segun filtro
se solicita el filtro agregando WHEARE y la condicion: <br>
`SELECT * FROM movies WHERE rating > 5` <br>
para agregar mas de un filtro se agrega AND o OR.
</div>
<div id = "funciones-manipulacion-Seleccionar-Operadores">

### Operadores
|Operador   |   Funcion                 | 
|:---------:|---------------------------|
| `=`       | Igual a                   |   
| `>`       | Mayor que                 |
| `>=`      | Mayor o igual que         |
| `<`       | Menor que                 |
| `<=`      | Menor o igual que         |
| `<>`      | Diferente a               |
| `!=`      | Diferente a               |
| `IS NULL` | Es null    
| `NOT NULL` | No es null                     |
| `BETWEEN valor AND valor` | Entre dos valores
| `IN`      | Lista de valores          |
| `LIKE ("string")`    | Se ajusta a la estring. Puede ser (%string => termina) (string% => inicia) (%string% => contiene)
|`LIMIT int`| no selecciona hasta el limite. va al final de todas las sentencias 
|`OFFSET int`| nos saltea los primeros int resultados al final de todo despues de LIMIT 
</div>
<div id = "funciones-manipulacion-Ordenar">

### Ordenar datos seleccionados
Se ordenan los datos agregando ORDER BY campo <br>
`SELECT * FROM movies ORDER BY campo` <br>
si se quiere ordenar de mayor a menor se le agrega al final del campo un DESC<br>
`SELECT * FROM movies ORDER BY campo DESC` <br>
y para agregar una regla de desenpate se hace de la siguente forma: <br>
`SELECT * FROM movies ORDER BY campo DESC, campoDesenpate`

<div id = "funciones-manipulacion-Apodar">

### Darle un apodo a los campos:
para darle un apodo a los campos seleccionados se le agrega el nombre original mas AS y el apodo dado como en el siguiente ejmplo: <br>
`SELECT nombreOrigina AS apodo FROM movies`
</div>

<div id = "funciones-manipulacion-Edicion">

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
</div>
<div id = "funciones-manipulacion-CASE">

## CASE
Se selecciona distintos casos como en la estructura: <br>
```
CASE
    WHEN bool THEN valor
    WHEN bool THEN valor
    ELSE valor
END
```
</div> </div>

## [Indice](#Indice)
<div id = "union-tablas">

# Union de tablas

<div id = "union-tablas-JOIN">

## INNER JOIN
```
SELECTO movies.id, campo2,campo3
FROM tabla
INNSER JOIN tablaAUnir ON campoTabala = campoTablaB
```
</div>
<div id = "union-tablas-JOIN-otros">

### Otras variables:
|Operador   |   Funcion                 | 
|:---------:|---------------------------|
|`LEFT JOIN` | tabla de la izquierda va a ser aceptado aun no tiendo vinculo
|`RIGHT JOIN`| tabla de la derecha va a ser aceptada aun sin vinculos
</div>
<div id = "union-tablas-DISTINCT">

## DISTINCT
Elimina duplicados 100% iguales en sus filas  <br>
`SELECTO DISTINCT movies.id, campo2,campo3 FROM tabla`
</div>
<div id = "union-tablas-GRUP">

## GRUP BY  
Se crean grupos por diferentes categorias para aplicarle diferentes funciones:<br>
`GROUP BY campoDeAgrupacion`<br> 
</div>
<div id = "union-tablas-HAVING">

## HAVING
Agrega condiciones a los datos agrupados <br>
`GRUP BY campoDeAgrupacion HAVING condicionDeGrupacion`<br> 
</div> </div>


## [Indice](#Indice)
<div id = "Funciones-agregación">

# Funciones de agregación
|Operador   |   Funcion                 | 
|:---------:|---------------------------|
|`COUNT(*)`         | Nos suma la cantidad de filas que hay en una tabla segun el campo
|`MAX(campo)`       | Nos devuelve el campo maximo de la tabla segun el campo
|`MIN(campo)`       | Nos devuelve el campo minimo de la tabla segun el campo
|`SUM(campo)`       | Hace la sumatoria de todos la tambla segun el campo
|`AVG(campo)`       | Saca el promedio de todas las filas segun el campo
</div>