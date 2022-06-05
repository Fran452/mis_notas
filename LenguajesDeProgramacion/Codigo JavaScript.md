<div id = "Indice"> <!----- Inicio de Indice ------->

# Indice

1. 
| [Estructuras](#Estructuras) |
|:-------------------------:|
|[Variables](#Estructuras-Variables)|
|[Decicion](#Estructuras-Decicion)|
|[Bucle](#Estructuras-Bucle)|
|[Funcionesz](#Estructuras-Funciones)|

2. 
| [Funciones](#Funciones) |
|:-------------------------:|
| [Array](#Funciones-Array) |
| [String](#Funciones-String) |
| [Numeros](#Funciones-Numeros) |
| [Objetos](#Funciones-Objetos) |
| [HTML](#Funciones-HTML) |
| [FS](#Funciones-FS) |
| [path](#Funciones-path) |

3. 
| [Clases](#Clases) |
|:-------------------------:|
| [Estructura](#Clases-Estructura)|
| [Clases](#Clases)|

4. 
| [Otros](#Otros) |
|:-------------------------:|

5. 
| [Modulos](#Modulos) |
|:-------------------------:|
| [Variables](#Modulos-Variables)|
| [Funciones](#Modulos-Funciones)|

6. 
| [JSON](#JSON) |
|:-------------------------:|
| [Estructura](#JSON-Estructura)|
| [Funciones](#JSON-Funciones)| 
| [Escritura](#JSON-Escritura)| 

7.  
| [Date](#Date) |
|:-------------------------:|
| [Estructura](#Date-Estructura)|
| [Funciones](#Date-Funciones)| 

8. 
| [Destructuracion](#Destructuracion) |
|:-------------------------:|
| [Estructura](#Destructuracion-Array)|
| [Objetos](#Destructuracion-Objetos)| 

9. 
| [Express](#Express) | Extenciones | 
|:-------------------------:|-----|
| [Paquetes](#Express-Paquetes)| sin extencion |
| [Codigo req/res](#Express-Codigo-req/res)| sin extencion | 
| [Codigo app/router](#Express-Codigo-app/router)| sin extencion |
| [Multer](#Express-Multer)| [Configurarciones](#Express-Multer-Configurarciones)|
| [Express Validator](#Express-Validator)| [Configurarciones](#Express-Validator-Configurarciones) <br> [Codigo](#Express-Validator-Codigo)| 
| [Express Session](#Express-Session)| [Configurarciones](#Express-Session-Configurarciones) <br> [Codigo](#Express-Session-Codigo)| 
| [Cookies](#Express-Cookies)| [Configurarciones](#Express-Cookies-Configurarciones)| 
| [Hashing](#Express-Hashing)| [Configurarciones](#Express-Hashing-Configurarciones) <br> [Codigo](#Express-Hashing-Codigo)|
| [Sequelize](#Express-Sequelize) |[Configuracion](#Express-Sequelize-Configuracion)<br>[Modelos](#Express-Sequelize-Modelos)<br>[Select](#Express-Sequelize-Select)<br>[Where](#Express-Sequelize-Where)<br>[Order](#Express-Sequelize-Order)<br>[Limit](#Express-Sequelize-Limit)<br>[Offset](#Express-Sequelize-Offset)<br>[Create](#Express-Sequelize-Create)<br>[Update](#Express-Sequelize-Update)<br>[Destroy](#Express-Sequelize-Destroy)|
| [Fetch](#Express-Fetch)| [¿Que es?](#Express-Fetch-Que) <br> [Configuracion](#Express-Fetch-Configuracion)<br> [Estructura](#Express-Fetch-Estructura)|
    
10. 
| [Promesas](#Promesas) |
|:-------------------------:|
| [¿Que es?](#Promesas-Que)|
| [Then](#Promesas-then)| 
| [Catch](#Promesas-catch)|
| [Promise](#Promesas-Promise)|
| [async](#Promesas-async)|

20. 
|[Material Teorico](#Teorico)|| 
|:--------------------:|-----|
|[Express](#Teorico-express)|[app.js](#Teorico-express-app.js) <br> [routers](#Teorico-express-routers)<br> [controller](#Teorico-express-controller) | 
|[CRUD](#Teorico-CRUD)|[¿Que es?](#Teorico-CRUD-que)| 
|[HTTP](#Teorico-HTTP)|[Metodos](#Teorico-HTTP-Metodos) <br> [codigo](#Teorico-HTTP-codigo)| 
|[Middlewares](#Teorico-Middlewares)|[¿Que es?](#Teorico-Middlewares-Que ) <br> [aplicacion](#Teorico-Middlewares-aplicacion) <br> [rutas](#Teorico-Middlewares-rutas) | 
|[Runtas](#Teorico-Runtas)|[Fija](#Teorico-Runtas-Fija) <br> [parametrisada](#Teorico-Runtas-parametrisada) <br> [obtativa](#Teorico-Runtas-obtativa)| 
|[Carpeta](#Teorico-Carpeta)|| 
|[Error](#Teorico-Error)|[Codigo](#Teorico-Error-Codigo)| 

</div> <!----- Fin de Indice ------->
       
## [Indice](#Indice)
<div id = "Estructuras"> <!----- Inicio de Estructuras ------->

# Estructuras

<div id = "Estructuras-Variables"> <div id = "Estructuras"> <!----- Inicio de Variables ------->

## Variables
| Variable                  |codigo|
|:-------------------------:|---
|string| "texto"
|array |[valor,valor2,varl3,...,valorN]
|object|{clave : valor,clave2 : valor2,... ,claveN: valorN}|
|int| 5
|variables generales| `var nombreCosntate`
|variables constantes| `cosnt nombreConsate`
|variables locales| `let nombreConstate`

</div> <!----- Fin de Variables ------->
<div id = "Estructuras-Decicion"> <!----- Inicio de Decicion ------->

## Decicion
```
if(condicion){
    codigoTrue
}else if(condicion2){
    codigoTrueCondicion3
}else{
    codigoFalse
}
```
```
let variable = bool ? valorTrue : valoFalse
```
```
switch(valor){
    case "caso1":
        funcion;
    break;

    default:
        funcion;
    }
```
</div> <!----- Fin de Decicion ------->
<div id = "Estructuras-Bucle"> <!----- Inicio de Bucle ------->

## Bucle
```
for(let valorInicial ;condicion; modificacionValorInicial){
    codigoBucle
}
```
Repite la cantidad de veces segun la cantidad de objetos del mismo, se toma el indice en clave 
```
for(clave in valor){ 
    funcion;            
}
```
repite la cantidad de veces segun la cantidad de objetos del mismo, se toma el valor en clave y no la pocicion
```
for(clave of valor){ 
    funcion;            
}
```
```
while(condicion){
    codigoTrue
}
```
```
do{
    codigoTrue
}while(condicion)
```


</div> <!----- Fin de Bucle ------->
<div id = "Estructuras-Funciones">  <!----- Inicio de Funciones ------->

## Funciones
### Funcion Comun
```
fuction nombre(variables){  
    codigo
}
```
### Fucion Flecha                         
`let nombre = (variables) => {codigo}`
### Funcion con una cantidad de variables no definidas
```
fuction nombre(...variables){
    codigo
}                                
```
</div> <!----- Fin de Funciones ------->
</div> <!----- Fin de Estructuras ------->

## [Indice](#Indice)
<div id = "Funciones"> <!----- Inicio de Funciones ------->

# Diferentes funciones segun variables

<div id = "Funciones-Array"> <!----- Inicio de Array ------->

## Funciones a tener en cuenta para array:
| Codigo                  |Funcion|
|:-------------------------:|---|
|`array.slice(inicio,fin)`                        | Toma una parte del arreglo sin tomar el del final
|`array.filter(funcion(valor,indice){funcion})`   | Filtra un arreglo
|`array.map(fuction(valor,indice){funcion}) `     | Modifica todos los valores del array segun la funcion
|`arrey.splice(elemento,cantidad)`                | Elimina desde el elemento la cantidad de elementos 
|`array.join(x)`                                  | Devuelve una lista unida por el x
|`array.split(x)`                                 | Devuelve una lista dividida por el x
|`array.push(x)`                                  | Agrega x al arreglo
|`array.mapped()`                                 | Cambia un array a objeto literal
|`array.length`                                   | Tamaño del arreglo
|`array.pop()`                                    | Se elimina el ultimo valor del arreglo
|`array.indexOf(valor)`                           | Nos indica la pocicion del valor en un array
|`array.shift()`                                  | Elimina el primer valor de un array
|`array.includes(valor)`                          | Se indica si el valor esta incluido en el array
|`array.unshift(valor)`                           | Agrega el valor al inicio de la lista
|`array.reduce(function(acumulador,elemento){funcion},acumulador)` | Junta los elementos segun la funcion dada
|`array.forEach(function(elemento){funcion})`     | Cumple la misma funcion que el map sin returnar nada 
|`array.find(function(elemento){funcionBool})`    | Te trae el elemento que cumpla esa condicion
|`let array = [...arraA, ...arrayB]`              | Creo un array con los valores de la arraA y la arraB antes declarado

</div> <!----- Fin de Array ------->
<div id = "Funciones-String"> <!----- Inicio de String ------->

## Funcion para String
| Codigo                  |Funcion|
|:-------------------------:|---|
|`string.toUpperCase()`             | Devuelve el valor con mayusculas
|`Number(string)`                   | Te pasa de una string a un entero 
|`string.length `                   | Tamaño de la string.
|`string.indexOf(valor)`            | Nos indica la pocicion del valor en una  string
|`string.slice(inicio,fin)`         | Toma una parte del string sin tomar el final   
|`string.trim()`                    | Elimina los espacios en blanco del inicio y del final
|`string.split(valor)`              | Convierte la string en array tomando como divisor el valor | ejemplo "hola soy juan".split("j") -> [ 'hola soy ', 'uan' ]
|`string.replace(valor,valor2)`     | Remplaza de la string el primer valor encontrado con valor2
|`string.replaceAll(valor, valor2)` | Remplaza Todos los valor por valor2 
|`hola mi nombre es ${nombre}`      | Forma alternativa para el no uso de "" o '' y eliminar + al usar el `` 

</div> <!----- Fin de String ------->
<div id = "Funciones-Numeros"> <!----- Inicio de Numeros ------->

## Funcion para Numeros
| Codigo                  |Funcion|
|:-------------------------:|---|
|`num.toString()`  | pasa el numero a string
|`parseInt(valor)` | pasa de un valor decima a un valor entero

</div> <!----- Fin de Numeros ------->
<div id = "Funciones-Objetos"> <!----- Inicio de Objetos ------->

## Funciones para Objetos
| Codigo                  |Funcion|
|:-------------------------:|---|
|`object.hasOwnPeoperty(propiedad)` | Pregunta si tiene esa propiedad ese objeto
|`object.reduce(function(acumulador,elemento){funcion},acumulador)` | Junta los elementos segun la funcion dada
|`object.map(funcion(valor,indice){Funcion},acumulador)` | Aplica la funcion a cada elemento
|`object.key`|Muestra que contiene la llave
|`object[key]`| devuelve el valor que almacene esa key del objeto de otra forma
|`let object = {...objectA}` | Creo un object con las propiedades de objectA antes declarado

</div> <!----- Fin de Objetos ------->
<div id = "Funciones-HTML"> <!----- Inicio de HTML ------->

## Funciones de HTML
| Codigo                  |Funcion|
|:-------------------------:|---|
|`document.write(valor)`    | Muestra el valor en la pantalla
|`prompt(valor)`            | Le pide al ususario un valor 
|`alert(valor)`             | Muestra como alerta el valor
|`confirm(valor)`| Envia al js un booleano de una ventana emergente 
|``|

</div> <!----- Fin de HTML ------->
<div id = "Funciones-FS"> <!----- Inicio de FS ------->

## FS
| Codigo                  |Funcion| 
|:-------------------------:|---|
|`fs.readFileSync("archivo",utg-8)`|lee el archivo indicado en el primer parametro y en el segundo parametro indica el decodificado
|`fs.writeFileSync("archivo",informacionString)`|El archivo es sobreescrito por la informacionString
|`fs.appendFileSync("archivo",informacionString)`|la informacionString se agrega al final del archivo

</div> <!----- Fin de FS ------->
<div id = "Funciones-path"> <!----- Inicio de path ------->

## path
| Codigo                  |Funcion|
|:-------------------------:|---|
|`path.join(carpeta1,carpeta2,carpeta3)`| se crea una ruta que indica hacia donde va
|`path.extname(direccion)`|te declara cual es la extencion del archivo
|`path.dirname(direccion)`|te daclara el directorio de un archivo

</div> <!----- Fin de path ------->
</div> <!----- Fin de Funciones ------->

## [Indice](#Indice)
<div id = "Clases"> <!----- Inicio de Clases ------->

# Clases

<div id = "Clases-Estructura"> <!----- Inicio de Estructura ------->

## Estructura
### Declaracion de clase
```
class Clase{
    construnctor(variable1,valriable2){
        this.variable1 = variable1;
        this.variable2 = variable2;
    }
}
```
### Exprecion de clase
#### Anonima
```
const Clase =class{
    construnctor(variable1,valriable2){
        this.variable1 = variable1;
        this.variable2 = variable2;
    }
}
```
#### Nombrada
```
const Clase = class Clase{
    construnctor(variable1,valriable2){
        this.variable1 = variable1;
        this.variable2 = variable2;
    }
}
```
</div> <!----- Fin de Estructura ------->
<div id = "Clases-Herencia"> <!----- Inicio de Herencia ------->

## Herencia
se le agrega el atributo extends y de que clase se hereda
```
class ClasePadre{
    construnctor(variable1,valriable2){
        this.variable1 = variable1;
        this.variable2 = variable2;
    }
}
```
```
class ClaseHija extends ClasePadre{
    construnctor(variable1,valriable2,variableHija){
        super(variable1,variable2);
        this.variableHija = variableHija
    }
}
```

</div> <!----- Fin de Herencia ------->
</div> <!----- Fin de Clases ------->


## [Indice](#Indice)
<div id = "Otros"> <!----- Inicio de Otros ------->

# Otros
`nombreDelCiclo:` -> Le pone una etiqueta al ciclo para poder utilizarlo en el caso de break o continue <br>


`continue;` -> No finaliza sino saltea la iteracion <br>
`break;` -> Finaliza el bucle <br>
`process.argv` -> Toma las variables que se pasan por consola despues del node ruta <br>

| Codigo                  |Funcion| 
|:-------------------------:|---|
|`typeof valor`    | nos dice el tipo del valor


</div> <!----- Fin de Otros ------->
<div id = "Modulos">  <!----- Inicio de Modulos ------->

# Modulos JavaScritp
<div id = "Modulos-Variables">  <!----- Inicio de Variables ------->

## Variables
`module.exports = nombreDeLaVariable` => __Exportar__ variable del archivo fuente <br>
`module.exports = {variable1, variable2, variable3, ... , variableN}` => Para varias variables <br>
`require("ubicacionDelArchivoFuente")` => __Importar__ variable en un archivo

</div> <!----- Fin de Variables ------->
<div id = "Modulos-Funciones"> <!----- Inicio de Funciones ------->

## Funciones 
__exporta__ una lista de funciones
```
module.exports = {         
    funcion1 : funcion1    
    funcion2 : funcion2      
    ...                     
    funcionN : funcionN     
}
```

`let funciones = require("ubicacionDelArchivoFuente")` => __Importar__ las funciones en la variable <br>
`funciones.funcion1()`                                 => convoca a la funcion <br>

</div> <!----- Fin de Funciones ------->
</div> <!----- Fin de Modulos ------->


## [Indice](#Indice)
<div id = "JSON">  <!----- Inicio de JSON ------->

# JSON
<div id = "JSON-Estructura">  <!----- Inicio de Estructura ------->

## Estructura de un archivo .json
```
'[{"name":"Argentina","capital":"CABA","reguion":"America"}]'
```

</div>  <!----- Fin de Estructura ------->
<div id = "JSON-Funciones"> <!----- Inicio de Funciones ------->

## Funciones JSON
| Codigo                  |Funcion|
|:-------------------------:|---|
|`JSON.parse(datoJSON)`|convierte el dato JSON a objeto literal<br>
|`JSON.stringify(datoObjeto)`|convierte el objeto literal en dato JSON<br>

</div> <!----- Fin de Funciones ------->
<div id = "JSON-Escritura"> </div> <!----- Inicio de Escritura ------->

## Como pasar un archivo JSON a javaScript
`fs.readFileSync("rutaDelJson","utf-8")` =>  nos lee y nos guarda el valor<br>

</div> <!----- Fin de Escritura ------->
</div> <!----- Fin de JSON ------->

## [Indice](#Indice)

<div id = "Date"> <!----- Incicio de Date ------->

# Objeto Date
<div id = "Date-Estructura"> <!----- Incicio de Estructura ------->

## Estructura
let fechaActual = new Date() => crea una variable con el informacion del dividida

</div> <!----- Fin de Estructura ------->
<div id = "Date-Funciones"> <!----- Incicio de Funciones ------->

## Funciones
| Codigo                  |Funcion|
|:-------------------------:|---|
|`fechaActual.getDay() `    | Un numero segun el dia de la semana [domingo = 0]
|`fechaActual.getDate()`    | Te da el dia del mes
|`fechaActual.getMoth()`    | Te da el mes en el que te encontras empezado desde 0
|`fechaActual.getFullYear()`| Te retorna el año
|`fechaActual.toUTCString()`| Le da formato al dia 

</div> <!----- Fin de Funciones ------->
</div> <!----- Fin de Date ------->



## [Indice](#Indice)
<div id = "Destructuracion"> <!----- Inicio de Destructuracion ------->

# Destructuracion
<div id = "Destructuracion-array"> <!----- Inicio de array ------->

## Para array
```
let array = ["val1", "val2", "val3", ... , "valN"];
let[val1,val2] = array 
```
val1 va ser igual a "val1"

</div> <!----- Fin de array ------->
<div id = "Destructuracion-Objetos"> <!----- Inicio de Objetos ------->


## Para Objetos
```
let object = {nombre : "fran", edad : 19, trabajo : "programador"}
let[nombre,edad] = object
```
cuando declare nombre va almacenar "fran" 

</div> <!----- Fin de Objetos ------->
</div> <!----- Fin de Destructuracion ------->

## [Indice](#Indice)
<div id = "Express">  <!----- Inicio de Express ------->

# Express
<div id = "Express-Paquetes"> <!----- Inicio de Paquetes ------->

## Paquetes necesarios y distribucion de carpetas
### paquetes necesarios
#### externos
para una mejor implementaicon de node es necesario descargar estos paquetes de npm:
| descargar                |              requerir          |     Funcion  |
|:------------------------:|--------------------------------|--------------|
|npm i express             | `require("express")`           | Descarga el paquete basico de express
|npm i method-override     | `require("method-override")`   | Permite subir fotos al servidor
|npm i express-validator   | `require("express-validator")` | Permite validar campos del formulario
|npm i express-session     | `require("express-session")`   | Mantener sesiones aviertas y confg globales
|npm i cookie-parser       | `require('cookie-parser')`     | Sirve para la utilizacion de la coockies en una pagina web
|npm i bcryptjs            | `require('bcryptjs')`          | Se utiliza para incriptar codigo
|npm i ejs                 | `app.set('view engine', 'ejs')`| Se utiliza para poder usar los archivos ejs en nuestra pagina web
|npm i multer              | `require("multer")`            | Se utiliza para poder subir fotos a nuestra base de datos
|npm i sequelize@5.21      | `require("sequelize")`         | Se utiliza para el manejo de bases de datos 
|npm i mysql2              |                                | Se utiliza para la utilizacion de bases de datos de sql      
|npm i node-fetch          | `require("node-fetch")`        | Nos permite hacer pedidos a una api de terceros desde nuestro back-end
#### interno
`require(path)` <br>
`require(fs)`
### carpetas utilizadas para una mejor implementacion de express
 mejor definida en el rachivo web.md
> `app.js` en este se implementan todos los arranques de la web
>  __router__ en esta carpeta se guardan todas las direcciones de nuestra web en archivos como `person.js`
> __controller__ en esta carpeta se almacena todas las acciones req res de cada ruta anteriormente mencionada. el nombre de los rachivos es `personController.js`
-------------------------- ARREGLAR---------------------

</div> <!----- Fin de Paquetes ------->
<div id = "Express-Codigo-app/router"> <!----- Inicio de app/router ------->

## Codigo app/router
| Codigo                  |Funcion|
|:-------------------------:|---|
|`app.listen(puerto, () => {})`|inicia el servidor en el puerto, con una funcion que retorna una string|
|`app.get('/', (req,res) => {})`| envia una respuesta al link enviado en la primer pocicion ('/')
|`app.use(express.static(publicPath))`|utilizacion del archivo publico como img o css
|`app.set(string1,string2)`|permite definier el motor de plantilla entre otras, con la primer string poniendo "view engine" y en el segundo el Template Engine a usar 
|`app.use(express.urlencoded({extended:false}));`| No se
|`app.use(express.json())`| No se 
|`app.use(methodOverride('_method'))`|
|`router.post('ruta',(req,res) => {})`| recibe la informacion recibida en un cuestionario anteriormente, la info se almacena en `req.body`
|`router.put('ruta',(req,res) => {})`|sirve para modificar datos enviados por un formulario
|`router.delete('ruta',(req,res) => {})`|elimina el objeto enviado por html

</div> <!----- Fin de app/router ------->
<div id = "Express-Codigo-req/res"> <!----- Inicio de app/router ------->

## Codigo req/res
| Codigo                  |Funcion| 
|:-------------------------:|---|
|`req.params.parametroRuta`                     | Nos devuelve el valor parametrizado en la ruta|
|`req.query`                                    | Se almacena el valor de un query que envia el usuario valores al mismo.
|`req.file`                                     | Envia los datos de un documendo subido por multer(informacion en BaseDeDatos)
|`req.body`                                     | Devuelve el kay y valor de los formularios enviados por post
|`req.url`                                      | Devuelve el link en el que se ingreso
|`req.session.valor`                            | Devuelve un objeto con los datos de la session activa en
|`req.cookie.nombreDelvalor`                    | Devuelve el valor de la cookie anterior mente almacenado en el res   
|`res.send(codigo Html)`                        | Envia un codigo html 
|`res.sendFile(ubiacion)`                       | Envia un archivo con una ruta absoluta
|`res.render('nombreDeLaVista',{valorEnviado})` | Sirve para renderizar una vista de ejs y tambien se puede enviar diferentes valores al mismo.
|`res.redirect('link')`                         | Redirige de una pagina a otra
|`res.cookie(nombre,valor,{configuraciones})`   | Se almacena una coookie con el nombre que le asignemos (String) y el valor almacenado, al final se almacena un objeto literal con las configuraciones pj(`maxAge: 60000` guarda la variable por 60 segundos)
|`res.locals.variable`                          | Almacena la variable en locals para poder utilirse en las vistas

</div> <!----- Fin de req/res ------->
<div id = "Express-Multer"> <!----- Inicio de Multer ------->

## Multer
<div id = "Express-Multer-Configurarciones"> <!----- Inicio de configurarciones ------->

### Primeras configurarciones
#### JS
- Requerir el paquete => `const multer = require('multer')`
- Configurar multer => 
```
const storage = multer.diskStorage({
    destination:(req,file,cb) => {
        cb(null, carpetaDondeSeDeseaAlmacenaElArchivo)
        }, => donde se va a guardar el archivo
    filename: (req,file,cb) => {
        cb(null, nombr eQueSeLeDeseaPoner.extencion)
        } => con que nombre se va a guardar el archivo
})
```
- especificar que configuracion se va a usar: <br>
`let fileUpload = multer({storage: storage});`
- configurar ruta: se le agrega el upload.single("nombre del formulario") para que la ruta sepa que parte del formulario permite guardar fotos. ejemplo: <br>
para subir una imagne <br>
`router.post('/register',upload.single("fotoDePerfil"),(req,res)=>{})`<br>
para subir varias => <br> 
`upload.any("fotoDePerfil")`
__------------------ ARREGLAR Y AGREGAR: HTML --------------------------------------__

</div> <!----- Fin de Configurarciones ------->
</div> <!----- Fin de Multer ------->
<div id = "Express-Validator"> <!----- Inicio de Validator ------->

## Express Validator 
<div id = "Express-Validator-Configurarciones"> <!----- Inicio de Configurarciones ------->

### Primeras configurarciones
#### Router
- requerir el paquete => `const {body} = require('express-validator')`
- definir los requisito => <br>
```
const validation = {
    validacion1,
    validacion2,
    validacion3
}
```
- agregar como Middlewares en la rutas => `router.get("link",validation,controller)`
#### Controller
- requerir otra parte del paquete => `const {validationResult} = require('express-validator')`
- llamamos a la funcion en nuestro controller => `let validaciones = validationResult(req)` 
- esto nos devuelve un array de objetos con diferentes parametrso como en el siguiente ejemplo: 
```
errors:[
    {
        value : "",
        msg : ""
        params: "",
        location: ""
    },
    {
        value : "",
        msg : ""
        params: "",
        location: ""
    }
]
```
- tramformamos ese array en un objeto con esta funcion => `validaciones.mapped()`

</div> <!----- Fin de Configurarciones -------> 
<div id = "Express-Validator-Codigo">  <!----- Inicio de Codigo -------> 

### Codigo
| Codigo                  |Funcion|
|:-------------------------:|---|
|`check('nomrbeDelImput').notEmpty()`|obliga que el input no este vacio
|`check('nomrbeDelImput').isEmail()`| obliga que el input sea un mail
|`check('nomrbeDelImput').validacion().withMessage('mensaje de error')`| si la validacion no se cumple salta con este mensaje de error
|`check('nomrbeDelImput').isLength({min : valorMinimo, max: valorMaximo})`| valida si se cumple el rango seleccionado
|`array.isEmpaty()`|nos dice si hay no hay errores de validacion
|`check('nomrbeDelImput').bail()`| corta las siguiente validaciones

</div>  <!----- Fin de Codigo -------> 
</div>  <!----- Fin de Validator -------> 
<div id = "Express-Session">  <!----- Inicio de Session -------> 

## Express Session
<div id = "Express-Session-Configurarciones"> <!----- Inicio de Configurarciones -------> 

### Primeras Configurarciones
#### app.js
- requerimos elpaquete
- usamos el Middlewares: app.use(session({secret : "texto"}))

</div> <!----- Fin de Configurarciones -------> 
<div id = "Express-Session-Codigo"> <!----- Inicio de Codigo -------> 

### Codigo
| Codigo                  |Funcion|
|:-------------------------:|---|
|`get.session.parametro`| se almacena de forma global el parametro seleccionado 

</div> <!----- Fin de Codigo -------> 
</div> <!----- Fin de Session -------> 
<div id = "Express-Cookies"> <!----- Inicio de Cookies -------> 

## Cookies
<div id = "Express-Cookies-Configurarciones"> <!----- Inicio de Configurarciones -------> 


### Primeras configurarciones
#### app.js
- requerimos el paquete
- lo importamos
- lo configuramos como Middlewares: <br>
`app.use(coockieParser())`

#### Controller
- para utilisarse primero se almacena un valor en `res.cookie(nombre,valor,{configuraciones})`
- se llama utilizando la funcion `req.cookie.nombreDelvalor`

</div> <!----- Fin de Configurarciones-------> 
</div> <!----- Fin de Cookies-------> 
<div id = "Express-Hashing"> <!----- Inicio de Hashing-------> 

## Hashing 
<div id = "Express-Hashing-Configurarciones"> <!----- Inicio de Configurarciones-------> 

### Primeras configurarciones
- requerimos el paquete
- lo importamos
__------------------ ARREGLAR Y AGREGAR: primeras --------------------------------------__

</div><!----- Fin de Configurarciones------->  
<div id = "Express-Hashing-Codigo"><!----- Inicio de Codigo-------> 

### Codigo 
| Codigo                  |Funcion|
|:-------------------------:|---|
|`bcrypt.hashSync("estring",int)`| Se incripta la string seleccionada con la dificultad enumerada en el int 
|`bcrypt.compareSync(contraseña,contraseñaIncriptada)`| indica si la contraseñas concuerda con la contraseñaIncriptada

</div>  <!----- Fin de Codigo-------> 
</div> <!----- Fin de Hashing------->  

<div id = "Express-Sequelize"><!----- Inicio de Sequelize-------> 

## Sequelize

<div id = "Express-Sequelize-Configuracion"> <!----- Inicio de Configuracion-------> 

### Configuracion
1. Requerimos el paquete con:  `sudo npm i -g sequelize@5.21 sequelize-cli` 
2. Requerimos la base de dato que vamos a usar: `sudo npm i mysql`
3. Creamos el arichivo `.sequelizerc`. En este se espesifica donde se almacena todo lo relacionado a nuestra base de datos. como por ejemplo:
```
const path=require('path');

module.exports={
    config: path.resolve('./database/config', 'config.js'),
    'models-path': path.resolve('./database/models'),
    'seeders-path': path.resolve('./database/seeders'),
    'migrations-path': path.resolve('./database/migrations'),
}
```

4. Corremos en consola el siguiente comando: `sequelize init` el cual nos crea algunas carpetas.
5. Configuramos config.js, en este configuramos el nombre de la base de datos, tipo, usuario contraseña etc
6. En index.js se realiza la conxion con la base de datos.

</div> <!----- Fin de Configuracion-------> 
<div id = "Express-Sequelize-Modelos"> <!----- Inicio de Modelos-------> 

### Modelos
#### Estructura 
Un modelo es el detalle de una table en especifico. Este se almacena en database/models con el nombre `NombreDeLaTabla.js` . El modelo siguie la siguiente estructura: 
```
module.exports = (sequelize, dataTypes) => {
    const Tabla = sequelize.define("nombreDeLaTabla",
        {
            valor1: {
                propiedades,
                type: dataTypes.TIPO
            },
            valor2: {
                propiedades,
                type: dataTypes.TIPO
            },
            valor3: {
                propiedades,
                type: dataTypes.TIPO
            }
        },
        {
            tableName : "nombreDeLaTabla",
            timestamps: false
        }
    );
    return Tabla:
}
```
#### Tipos
| Codigo Sequelize      |Tipo SQL|
|:-----------------------:|---|
|`dataTypes.INTEGER`          | INTEGER
|`dataTypes.BIGINT`           | BIGIN
|`dataTypes.FLOAT`            | FLOAT
|`dataTypes.DOUBLE`           | DOUBLE
|`dataTypes.DECIMAL`          | DECIMAL
|`dataTypes.DATE`             | DATE
|`dataTypes.STRING`           | VARCHAR(255)
|`dataTypes.STRING(VALOR)`    | VARCHAR(VALOR)

Estos son algunos tipos, para mas informacion: [TIPOS DE DATOS Sequelize](#https://sequelize.org/docs/v6/core-concepts/model-basics/#data-types)
#### Operadores
| Codigo                    |Funcion|
|:-------------------------:|---|
|`autoIncrement: true`      | Auto incremento
|`primaryKey: true`         | Clave Primaria
|`unique: true`             | La clable tiene que ser unica
|`allowNull: true`          | 
|`defaultValue: valor`      | Determina el valor en caso de null en la propiedad valor
|`isEmail: true`            | Tiene que ser un mail
|`isNumeric: true`          | Tiene que ser un numero
|`notEmpty: true`           |no permitir cadenas vacías

</div> <!----- Fin de Modelos------->
<div id = "Express-Sequelize-Pedidos"> <!----- Inicio de Pedidos------->

### Pedidos De Datos

<div id = "Express-Sequelize-Select"> <!----- Inicio de Select------->

#### Select 
| Codigo Sequelize      |       funcion SQL         |
|:---------------------:|---------------------------|
|`Tabla.findAll()`      |SELECT * FROM Tabla        |
|`Tabla.findByPk(id)`    |SELECT * FROM Tabla WHERE Tabla.id = id|
|`Tabla.findOne({where:{columna: condicion}})`|SELECT * FROM Tabla WHERE columna = condicion|

</div><!----- Fin de Select------->
<div id = "Express-Sequelize-Where"> <!----- Inicio de Where-------> 

#### Where
De esta forma filtramos por igualdad dentro de una tabla
```
Tabla.funcionSeleccio(
    {
        where: {columna : valor}
    }
)
```
__Operadores del where__
```
Tabla.funcionSeleccio(
    {
        where: {columna : {
                [db.Sequelize.Op.operador]: valor
        }}
    }
)
```
Para ver todos los operadores entrar al siguiente link: [Operadores](#https://sequelize.org/v5/manual/querying.html) 

</div> <!----- Fin de where------->
<div id = "Express-Sequelize-Order"> <!----- Inicio de Order-------> 

#### Order
```
Tabla.funcionSeleccio(
    {
        order: [
            ['columna','orden']
        ]
    }
)
```
El orden puede ser dos o `ASC` (ascendente) o `DESC` (descendente)

</div>  <!----- Fin de Order------->
<div id = "Express-Sequelize-Limit"> <!----- Inicio de Limit-------> 

#### Limit
```
Tabla.funcionSeleccio(
    {
        limit: valor
    }
)
```

</div> <!----- Fin de Limit------->
<div id = "Express-Sequelize-Offset">  <!----- Inicio de Offset-------> 

#### Offset
```
Tabla.funcionSeleccio(
    {
        offset: valor
    }
)
```

</div> <!------ Fin de Offset ------>
<div id = "Express-Sequelize-Manejo"> <!------ Inicio de Include ------>

#### include
```
Tabla.funcionSeleccio(
    {
        include: [{association : "tablaAAsociar"}]
    }
)
```

</div> <!------ Fin de Include ------>
</div> <!------ Fin de Pedidos ------>
<div id = "Express-Sequelize-Manejo"> <!------ Inicio de Manejo ------>

### Manejo de datos

<div id = "Express-Sequelize-Create"> <!------ Inicio de Create ------>

#### Create
Sirve para crear una fila dentro de una tabla. El metodo que usamos se llama create el cual recibe por parametro un objeto con las propiedades de cada columa
``` 
db.Tabla.create({
    columna : dato,
    columna : dato,
    columna : dato,
    columna : dato,
});
```
__bulkCreate()__ <br>
Este metodo crear mas filas que solo una como en el create. El metodo se llama bulkCreate y en si se recive un array de objetos con las propiedades de las columnas.
``` 
db.Tabla.bulkCreate([{
    columna : dato,
    columna : dato,
    },{
    columna : dato,
    columna : dato,
}]);
```

</div> <!------ Fin de Create ------>
<div id = "Express-Sequelize-Update"> <!------ Inicio de Update ------>

#### Update
Esta funcionalida nos permite actualizar fila de nuestra base de datos.
``` 
db.Tabla.update({
    columnaAActualizar : dato,
    columnaAActualizar : dato
},{
    where:{condicion}
});
```
__upsert()__ <br>
Esta funcion lo que hace es modificar o crear (en el caso que no exista) un campo de una fila
db.Tabla.upsert({
    columnaAActualizar : dato,
    columnaAActualizar : dato,
    columnaUnicaDeDato : dato
});

</div> <!------ Fin de Update------>
<div id = "Express-Sequelize-Destroy"> <!------ Inicio de Destroy------>

#### Destroy
Esta funcion lo que hace es eliminar un registro de la base de datos. para ellos se la pasa un objeto con la condicion para ser eliminado.
```
db.Tabla.destroy({
    where : {propiedad}
}); 
```

</div> <!------ Fin de Destroy ------>
</div> <!------ Fin de Manejo ------>
<div id = "Express-Sequelize-Relaciones"> <!------ Inicio de Relaciones ------>

### Relaciones
<div id = "Express-Sequelize-Relaciones-1aM"> <!------ Inicio de 1aM ------>

##### De 1 a muchos
##### Estructura:
En el archivo de model en cada modelo se utiliza la siguiente funciones para declarar las relaciones: <br>
- __hasMany__ <br>
Se utiliza para la tabla que contiene muchos campos en la otra tabla, por ejemplo en la relacion generos y peliculas. Se utiliza para asociar todos los generos a sus repectivas peliculas 
```
Tabla.associate = (models) => {
    db.Tabla.hasMany(models.tablaAsociada,{
        foreignKey : 'nombreDeLaClaveForania',
        as: 'campoDeLaTablaAsociada'
    })
}
```
- __belongsTo__ <br>
Se utiliza para la tabla que contiene un campo en la otra tabla, por ejemplo en la relacion generos y peliculas. Se utiliza para asociar cada pelicula a su genero
```
Tabla.associate = (models) => {    
    db.Tabla.belongsTo(models.tablaAsociada,{
        foreignKey : 'nombreDeLaClaveForania',
        as: 'campoDeLaTablaAsociada'
    })
}
```
</div> <!----- Fin de 1aM ------->
<div id = "Express-Sequelize-Relaciones-NaN"> <!------ Inicio de NaN ------>

#### De muchos a muchos
##### Estructura:
__belongsToMany__ <br>
Se repiten en ambas relaciones el mismo formato 
```
Tabla.associate = (models) => {    
    db.Tabla.belongsToMany(models.tablaAsociada,{
        as: 'campoDeLaTablaAsociada',
        through : 'tablaDeUnion',
        foreignKey : 'nombreDeLaClaveForaniaPropia',
        otherKey: 'nombreDeLaClaveForaniaTA',
        timestamps : false
        
    })
}
```
__Estructura de la tabla de union__ <br>
Para hacer la union de muchos a muchos antes se necesita un tabla intermedia para unirlos. Esta tabla tendra la siguiente estructura
```
const Tabla = sequelize.define("NombreDeLaTabla", {
    Relaion1: {
         type: Sequelize.INTEGER, 
         references: {model: "TablaRelacion", key: "ColumnRelacion"}},
    Relaion2: {
        type: Sequelize.INTEGER, 
        references: {model: "TablaRelacion", key: "ColumnRelacion"}}
})

module.exports = Tabla;
```
</div> <!----- Fin de NaN ------->
</div> <!------ Fin de Relaciones ------>
</div> <!----- Fin de Sequelize ------->
<div id = "Express-Fetch"> <!----- Inicio de Fetch-------> 

## Fetch
<div id = "Express-Fetch-Que"> <!----- Inicio de Que -------> 

### ¿Que es?

</div> <!----- Fin de Que ------->
<div id = "Express-Fetch-Configuracion"> <!----- Inicio de Configuracion -------> 

### Configuracion
- npm i node-fetch
- requeir el paquete : ` const fetch = require(node-fetch);`

</div> <!----- Fin de Configuracion ------->
<div id = "Express-Fetch-Estructura"> <!----- Inicio de Estructura -------> 

### Estructura 

controllers = {
    fuction : async (req,res){
        fetch("url")
            .then(respuesta de api)
            .then(respuesta del front end)
    }
}


</div> <!----- Fin de Estructura ------->
</div> <!----- Fin de Fetch ------->
</div> <!----- Fin de Express ------->




<div id = "Express-Promesas"> <!----- Inicio de Promesas-------> 

## [Indice](#Indice)
<div id = "Promesas"> <!----- Inicio de Promesas ------->  

# Promesas

<div id = "Promesas-Que"> <!----- Inicio de Que son -------> 

## ¿Que son?
Las promesas son funciones que permiten ejecutar código asincrónico de forma eficiente.

</div> <!----- Fin de Que son -------> 
<div id = "Promesas-then"> <!----- Inicio de then -------> 

## .then() 
Promesa que retorna algo en si
```
funcion(valor)
    .then(fuction(){
        codigo
    })

```

</div> <!----- Fin de then ------->
<div id = "Promesas-catch"> <!----- Inicio de catch -------> 

## .catch()
Codigo que se ejecute al momento de encontrarse con un error
```
funcion(valor)
    .catch(fuction(){
        codigo
    })

```

</div> <!----- Fin de catch -------> 
<div id = "Promesas-Promise"> <!----- Inicio de Promise -------> 

## Promise.all([])
Esto es una array de promesas que una vez que se hayan hecho se ejecutara un then. ejemplo: <br>
`Promise.all([promesa1,promesa2,...,promesaN])`

</div> <!----- Fin de Promise -------> 
<div id = "Promesas-async"> <!----- Inicio de async ------->

## function async
Este es otro metodo para crear funciones asincronicas con una estructura mas limpia que ustilizando el .then(). <br>
Su estructura se basa en la utilizacion del async en la funcion y la utilizacion de await para aclarar que funciones son asincronicas<br>
```
async(parametros){
    const valor = await funcionAsicronica;
    codigo
}
```


</div> <!----- Fin de async -------> 
</div> <!----- Fin de Promesas -------> 
<div id = "Front"> <!----- Inicio de Front end ------->

# Front end

## Window
### ¿Ques es?
Es un objeto literal que tiene funciones para modificar o preguntar propiedades de la venta del navegador
### Codigo
| Codigo                  |Funcion|
|:-------------------------:|---|
|`window.location`|Trae un objeto literal con diferentes datos de la pagina 
|`window.innerHeight`| Te dice cuanto mide de alto la pagina
|`window.innerWidth`|Te dice cuanto mide de ancho la pagina

Para mas informacion <a href = "https://www.w3schools.com/js/js_window.asp"> LINK </a>

## Document
Para mas informacion ingresar al siguiente link <a href = "https://developer.mozilla.org/es/docs/Web/API/Document">LINK </a>
### ¿Ques es?
Es un objeto literal que tiene funciones para modificar o preguntar propiedades del documento html
### Codigo Seleccion
| Codigo                  |Funcion|
|:-------------------------:|---|
|`document.bgColor`| Propiedad con el color de fondo 
|`document.styleSheets`| Propiedad con las hojas de estilos
|`document.querySelector("etiqueta")`| Propiedad que nos permite modificar un selector ejemplo (form , form.class , form#id, .class , #id)
|`document.querySelectorAll("etiqueta")`| Nos retorna un array con todos los selectores que cumpla con la etiqueta
|`document.getElementById("id")`| Almacena la informacion del id seleccionado en el html
|`document.getElementsByClassName("class")`|Almacena la informacion del class seleccionado en el html
|`document.querySelector("etiqueta").innerHTML`| Captura el conetenido del html con el = se lo puede cambiar y con += modificar
|`document.querySelector("etiqueta").innerText`|Trae el texto plano de la etiqueta y de querer modifica sin procesarse la etiquetas html
|`document.querySelector("etiqueta").style.propiedadCss`| Trae el valor de la propiedad seleccionada con la posibilidad de cambiarlo

### Codigo modificacion de clases 
`let query = document.querySelector("etiqueta")`

| Codigo                  |Funcion|
|:-------------------------:|---|
|`query.classList.add("clase")`|agrega una clase a un query
|`query.classList.remove("clase")`| quita una clase a un query
|`query.classList.toggle("clase")`| quita o agrega segun la existienca de la clase
|`query.classList.contains("clase")`| Nos retorna un bool con el valor de existencia de la clase


## Eventos 
### ¿Que son?
Los eventos son cualquier accion que ocurra en un sitio web
### Variable e
La variable e cumple la funcion de espesificar el evento en si. Esta funcion tiene varias acciones segun el evento
### Estructuras

1. Con addEventListener nos permite ejecutar varios eventos simultaneamente
```
window.addEventListener("load", function(){
    
    selector.addEventListener("evento",function(){
        codigo a ejecutar en el evento 
    })
    
})
```

2. Con on + algo. con este evento no nos permite utilizar mas de un evento a la vez
```
window.onload = () => {
codigo
}

```
Los eventos mas usados en este tipo son: 
| Evento                  |Funcion|
|:-------------------------:|---|
|`onclick`| Cuando el usuario hace clic.
|`ondblclick`| Cuando el usuario hace doble clic.
|`onmouseover`| Cuando el mouse se mueve sobre el elemento.
|`onmousemove`|   Cuando se mueve el mouse.
|`onscroll`|  Cuando se hace scroll.
|`onkeydown`| Cuando se aprieta una tecla.
|`onload`| Cuando se carga la página.
|`onsubmit`| Cuando se envía un formulario.

### Mouse
| Evento                  |Funcion|
|:-------------------------:|---|
|`click`| Se ejecuta al momento que se hace click en el query  
|`mouseover`| Se ejecuta cuando se pasa el mause por encima 
|`mouseout`| Se ejecuta cuando el mouse sale del area del query
### Teclado
| Evento                  |Funcion|
|:-------------------------:|---|
|`keydown`| Se utiliza cuando se presiona la tecla
|`keyup`| Se utiliza cuando se suelta la tecla
|`keypress`| Se ejecuta cuando el se finaliza la accion de precion y suelte de la tecla  
|`e.key`| No indica la tecla precionada 

### Formularios
| Evento                  |Funcion|
|:-------------------------:|---|
|focus| Se ejecuta cuando el usuario ingres a un campo del fromulario 
|blur| Se ejecuta cuando el cursor sale del campo del formulario 
|change| Nos detecta camvios en el fromulario
|submit| Se ejecuta cuando se envia un formulario
|query.value| Nos indica que se coloco en el formulario

<!----    FALTA REMARCAR EL CODIGO  -->

## Fetch
### Que es?
Es una funcion asincronica que nos devolvera una api en formato JSON
### Estructura
__Por GET__
```
fetch('linkDeLaApi')
.then(api => {
    return api.json();
})
.then(api => {
    codigo
})
```
__Por POST__
```
let data = {
    objeto enviado por post
}
fetch('linkDeLaApi',{
    'method':'POST';
    'body': JSON.stringify(data)
})
.then(api => {
    return api.json();
})
.then(api => {
    codigo
})
```
        
</div> <!----- Fin de Front end -------> 

## [Indice](#Indice)
<div id = "Teorico"> <!----- Inicio de Teoria-------> 



# Material Teorico

<div id = "Teorico-express">  <!----- Inicio de express -------> 

## Estructura de inicio de express
<div id = "Teorico-express-app.js"> <!----- Inicio de Estructura -------> 

### Del archivo app.js
```
const express = require("express");
const rutaA = require("./router/router.js")
const methodOverride = require('method-override')
const app = express();

app.listen(300) => inicia el servidor
app.use(methodOverride('_method'))
```

</div> <!----- Fin de Estructura -------> 
<div id = "Teorico-express-routers"> <!----- Inicio de routers -------> 

### Del los archivo routers
```
const express = require("express");
const app = express.Routers();
const controller = require("../controllers/controladorControllers.js")
module.imports = router
```

</div> <!----- Fin de routers -------> 
<div id = "Teorico-express-controller"> <!----- Inicio de controller -------> 

### Del los archivo controller
```
const controllers{
    rutaA : funcion,
    rutaB : funcion,
    rutaC : funcion,
    rutaD : funcion,
}

module.imports = controllers
```
</div> <!----- Fin de controller -------> 
</div> <!----- Fin de express -------> 
<div id = "Teorico-CRUD"> <!----- Inicio de CRUD -------> 

## CRUD
<div id = "Teorico-CRUD-que"> <!----- Inicio de que -------> 

### ¿Que es?
 Create, Read, Update y Delete

</div> <!----- Fin de que -------> 
</div> <!----- Fin de CRUD -------> 
<div id = "Teorico-HTTP">  <!----- Inicio de HTTP -------> 

## HTTP
<div id = "Teorico-HTTP-Metodos"> <!----- Inicio de Metodos -------> 

### Metodos
- get: solicita datos
- post: envia/crea datos
- put: remplaza datos
- patch: modifica parcialmente un dato
- delete: borra datos

</div> <!----- Fin de Metodos ------->  
<div id = "Teorico-HTTP-codigo"> <!----- Inicio de codigo -------> 

### Lineas de codigo necesarias 
`app.use(express.urlencoded({extended:false}));` <br>
`app.use(express.json())`

</div> <!----- Fin de codigo -------> 
</div> <!----- Fin de HTTP ------->  
<div id = "Teorico-Middlewares"> <!----- Inicio de Middlewares -------> 

## Middlewares
<div id = "Teorico-Middlewares-Que">  <!----- Inicio de Que -------> 

### ¿Que es?
Es un bloque de código que se va a ejecutar en la "mitad" de un determinado request

</div> <!----- Fin de Que ------->  
<div id = "Teorico-Middlewares-aplicacion"> <!----- Inicio de aplicacion -------> 

### A nivel de la aplicacion
Son los Middlewares que se ejecutan siempre que se hag aun pedido a la app, se declaran del app.js

</div> <!----- Fin de aplicacion ------->  
<div id = "Teorico-Middlewares-rutas"> <!----- Inicio de rutas -------> 

### A nivel de las rutas
Son los Middlewares que se ejecutan al momento de ingresar a daterminado link. se declaran como en el siguiente ejemplo: <br>
```
router.get("ruta",(req,res,next) => { codigo }, rutaController.action);
```

</div> <!----- Fin de rutas ------->  
</div> <!----- Fin de Middlewares -------> 
<div id = "Teorico-Runtas"> <!----- Inicio de rutas -------> 

## Rutas
<div id = "Teorico-Runtas-Fija"> <!----- Inicio de Fija -------> 

### Ruta fija
una ruta la cual siempre lleva el mismo nombre y no es modificado
```
router.get('/item',carritoController.agregarItem)
```

</div>  <!----- Fin de Fija ------->
<div id = "Teorico-Runtas-parametrisada">  <!----- Inicio de parametrisada -------> 

### Ruta parametrisada
ruta la cual el nombre es modificado ya se por un producto, una seccion etc
```
router.get('/:item',carritoController.agregarItem)
```

</div>  <!----- Fin de parametrisada ------->
<div id = "Teorico-Runtas-obtativa"> <!----- Inicio de obtativa -------> 

### Ruta parametrisada obtativa
ruta la cual el nombre es modificado ya se por un producto, una seccion etc y no es obligatoria que este
```
router.get('/:item?',CB)
```

</div>  <!----- Fin de obtativa ------->
</div>  <!----- Fin de Runtas ------->
<div id = "Teorico-Carpeta"> <!----- Inicio de Carpeta -------> 

## Carpeta Rutas
para cada ruta.js
`express.Router()` => te permite crear rutas montables y desmontables en nuestra app<br>
`router.get` => para crear las lineas de codico de cada ruta <br>

para app.js
- primero se importa el modulo
- `app.use("/ruta",imporDeRutas)` => el metodo use llama a nnuestras rutas y las utiliza con la funcion que le pasamos

</div>  <!----- Fin de Carpeta ------->
<div id = "Teorico-Error"> <!----- Inicio de Error -------> 

## Error 404
Este error se genera cuando un recurso no se encuentra dentro del servidor
<div id = "Teorico-Error-Codigo"> <!----- Inicio de Codigo -------> 

### Codigo
```
app.use((req,res,next) =>{
    res.status(404).render('not-found')
})
```

</div>  <!----- Fin de Codigo ------->
</div>  <!----- Fin de Error ------->