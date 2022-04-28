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
|[](#)|
|:------------------:|
|[](#)|
|[](#)|

</div>
 

<div id = "datos">

# Tipos de datos

<div id = "datos-numericos">

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


<div id = "funciones-manipulacion">

# Manipulacion de datos
## Incertar Datos
Con cada uno de los campos
```
INSERT INTO tabla VALUES (valor1,valor2,valor3)
```
si no queremos aclarar cada campo<br>
`INSERT INTO tabla(campo1,campo2,campo3) VALUE (valor1,valor2,valor3)`
## Modificar Datos
```
UPDATE movie 
SET modifiacion  
WHERE criterio
```
## Eliminar datos
`DELETE FROM MOVIE WHERE bool`

## Seleccionar
solicita todos los datos * de una tabla <br>
`SELECT * FROM movies` <br>
si quiero solicitar X campo:<br>
`SELECT campo1,campo2,campo3 FROM movies` <br>

### Seleccionar segun filtro
se solicita el filtro agregando WHEARE y la condicion: <br>
`SELECT * FROM movies WHERE rating > 5` <br>
para agregar mas de un filtro se agrega AND o OR.

#### Operadores
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
| `NOT NULL` | Es null                     |
| `BETWEEN valor AND valor` | Entre dos valores
| `IN`      | Lista de valores          |
| `LIKE`    | Se ajusta a (%a => termina) (a% => inicia) (%a% => contiene)
|`LIMIT int`| no selecciona hasta el limite. va al final de todas las sentencias 
|`OFFSET int`| nos saltea los primeros int resultados al final de todo despues de LIMIT 
### Ordenar datos seleccionados
Se ordenan los datos agregando ORDER BY campo <br>
`SELECT * FROM movies < campo` <br>
si se quiere ordenar de mayor a menor se le agrega al final del campo un DESC<br>
`SELECT * FROM movies ORDER BY campo DESC` <br>
y para agregar una regla de desenpate se hace de la siguente forma: <br>
`SELECT * FROM movies ORDER BY campo DESC, campoDesenpate`

### Darle un apodo a los campos:
para darle un apodo a los campos seleccionados se le agrega el nombre original mas AS y el apodo dado como en el siguiente ejmplo: <br>
`SELECT nombreOrigina AS apodo FROM movies`

## Funciones de edicion
|Operador   |   Funcion                 | 
|:---------:|---------------------------|
|`CONCAT (columna,columna)`| junta dos columnas en una sola
|`CALESCE(columna,valor)`| nos permite mostrar valor en las filas con columnas NULL
|`NOW()`| nos trae la feha actual
|`DATEDIFF(fecha1, fecha2)`| sirve para comparar dos fechas
|``| 

</div>