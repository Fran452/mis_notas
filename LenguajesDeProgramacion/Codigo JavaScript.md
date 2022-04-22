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

<div id = "Estructuras">

# Estructuras

<div id = "Estructuras-Variables">

## Variables
| Variable                  |codigo| | | |
|:-------------------------:|---|---|---|---| 
|string| "texto"
|array |[valor,valor2,varl3,...,valorN]
|object|{clave : valor,clave2 : valor2,... ,claveN: valorN}|
|int| 5
|variables generales| `var nombreCosntate`
|variables constantes| `cosnt nombreConsate`
|variables locales| `let nombreConstate`
</div>

<div id = "Estructuras-Decicion">

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
</div>


<div id = "Estructuras-Bucle">

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
</div>


<div id = "Estructuras-Funciones">

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
</div>
</div>


<div id = "Funciones">

# Diferentes funciones segun variables

<div id = "Funciones-Array">

## Funciones a tener en cuenta para array:
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
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
</div>

<div id = "Funciones-String">

## Funcion para String
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
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
</div>   


<div id = "Funciones-Numeros">

## Funcion para Numeros
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`num.toString()`  | pasa el numero a string
|`parseInt(valor)` | pasa de un valor decima a un valor entero
</div>


<div id = "Funciones-Objetos">

## Funciones para Objetos
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`object.hasOwnPeoperty(propiedad)` | Pregunta si tiene esa propiedad ese objeto
|`object.reduce(function(acumulador,elemento){funcion},acumulador)` | Junta los elementos segun la funcion dada
|`object.map(funcion(valor,indice){Funcion},acumulador)` | Aplica la funcion a cada elemento
|`object.key`|Muestra que contiene la llave
|`object[key]`| devuelve el valor que almacene esa key del objeto de otra forma
|`let object = {...objectA}` | Creo un object con las propiedades de objectA antes declarado
</div>


<div id = "Funciones-HTML">

## Funciones de HTML
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`document.write(valor)`    | Muestra el valor en la pantalla
|`prompt(valor)`            | Le pide al ususario un valor 
|`alert(valor)`             | Muestra como alerta el valor
</div>


<div id = "Funciones-FS">

## FS
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`fs.readFileSync("archivo",utg-8)`|lee el archivo indicado en el primer parametro y en el segundo parametro indica el decodificado
|`fs.writeFileSync("archivo",informacionString)`|El archivo es sobreescrito por la informacionString
|`fs.appendFileSync("archivo",informacionString)`|la informacionString se agrega al final del archivo
</div>


<div id = "Funciones-path">

## path
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`path.join(carpeta1,carpeta2,carpeta3)`| se crea una ruta que indica hacia donde va
|`path.extname(direccion)`|te declara cual es la extencion del archivo
|`path.dirname(direccion)`|te daclara el directorio de un archivo
</div>
</div>


<div id = "Clases">

# Clases

<div id = "Clases-Estructura">

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
</div>
<div id = "Clases-Herencia">

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
</div>
</div>



<div id = "Otros">

# Otros
`nombreDelCiclo:` -> Le pone una etiqueta al ciclo para poder utilizarlo en el caso de break o continue <br>


`continue;` -> No finaliza sino saltea la iteracion <br>
`break;` -> Finaliza el bucle <br>
`process.argv` -> Toma las variables que se pasan por consola despues del node ruta <br>

| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`tipeof valor`    | nos dice el tipo del valor
</div>


<div id = "Modulos">

# Modulos JavaScritp
<div id = "Modulos-Variables">

## Variables
`module.exports = nombreDeLaVariable` => __Exportar__ variable del archivo fuente <br>
`module.exports = {variable1, variable2, variable3, ... , variableN}` => Para varias variables <br>
`require("ubicacionDelArchivoFuente")` => __Importar__ variable en un archivo
</div>


<div id = "Modulos-Funciones">

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
</div>
</div>



<div id = "JSON">

# JSON
<div id = "JSON-Estructura">

## Estructura de un archivo .json
```
'[{"name":"Argentina","capital":"CABA","reguion":"America"}]'
```
</div>

<div id = "JSON-Funciones">

## Funciones JSON
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`JSON.parse(datoJSON)`|convierte el dato JSON a objeto literal<br>
|`JSON.stringify(datoObjeto)`|convierte el objeto literal en dato JSON<br>
</div>

<div id = "JSON-Escritura">

## Como pasar un archivo JSON a javaScript
`fs.readFileSync("rutaDelJson","utf-8")` =>  nos lee y nos guarda el valor<br>
</div>
</div>

<div id = "Date">

# Objeto Date
<div id = "Date-Estructura">

## Estructura
let fechaActual = new Date() => crea una variable con el informacion del dividida
</div>
<div id = "Date-Funciones">

## Funciones
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`fechaActual.getDay() `    | Un numero segun el dia de la semana [domingo = 0]
|`fechaActual.getDate()`    | Te da el dia del mes
|`fechaActual.getMoth()`    | Te da el mes en el que te encontras empezado desde 0
|`fechaActual.getFullYear()`| Te retorna el año
|`fechaActual.toUTCString()`| Le da formato al dia 
</div>
</div>


<div id = "Destructuracion">

# Destructuracion
<div id = "Destructuracion-array">

## Para array
```
let array = ["val1", "val2", "val3", ... , "valN"];
let[val1,val2] = array 
```
val1 va ser igual a "val1"
</div>
<div id = "Destructuracion-Objetos">

## Para Objetos
```
let object = {nombre : "fran", edad : 19, trabajo : "programador"}
let[nombre,edad] = object
```
cuando declare nombre va almacenar "fran" 
</div></div>


<div id = "Express">

# Express
<div id = "Express-Paquetes">

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
#### interno
`require(path)` <br>
`require(fs)`
### carpetas utilizadas para una mejor implementacion de express
 mejor definida en el rachivo web.md
> `app.js` en este se implementan todos los arranques de la web
>  __router__ en esta carpeta se guardan todas las direcciones de nuestra web en archivos como `person.js`
> __controller__ en esta carpeta se almacena todas las acciones req res de cada ruta anteriormente mencionada. el nombre de los rachivos es `personController.js`
-------------------------- ARREGLAR---------------------
</div>
<div id = "Express-Codigo-app/router">

## Codigo app/router
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
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
</div>
<div id = "Express-Codigo-req/res">

## Codigo req/res
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
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
</div>
<div id = "Express-Multer">

## Multer
<div id = "Express-Multer-Configurarciones">

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

</div>
</div>
<div id = "Express-Validator">

## Express Validator 
<div id = "Express-Validator-Configurarciones">

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
<div id = "Express-Validator-Codigo">

### Codigo
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`check('nomrbeDelImput').notEmpty()`|obliga que el input no este vacio
|`check('nomrbeDelImput').isEmail()`| obliga que el input sea un mail
|`check('nomrbeDelImput').validacion().withMessage('mensaje de error')`| si la validacion no se cumple salta con este mensaje de error
|`check('nomrbeDelImput').isLength({min : valorMinimo, max: valorMaximo})`| valida si se cumple el rango seleccionado
|`array.isEmpaty()`|nos dice si hay no hay errores de validacion
|`check('nomrbeDelImput').bail()`| corta las siguiente validaciones
</div> </div>
<div id = "Express-Session">

## Express Session
<div id = "Express-Session-Configurarciones">

### Primeras Configurarciones
#### app.js
- requerimos elpaquete
- usamos el Middlewares: app.use({secret : "texto"})
</div>
<div id = "Express-Session-Codigo">

### Codigo
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`get.session.parametro`| se almacena de forma global el parametro seleccionado 
</div> </div>
<div id = "Express-Cookies">

## Cookies
<div id = "Express-Cookies-Configurarciones">

### Primeras configurarciones
#### app.js
- requerimos el paquete
- lo importamos
- lo configuramos como Middlewares: <br>
`app.use(coockieParser())`

#### Controller
- para utilisarse primero se almacena un valor en `res.cookie(nombre,valor,{configuraciones})`
- se llama utilizando la funcion `req.cookie.nombreDelvalor`
</div> </div>
<div id = "Express-Hashing">

## Hashing
<div id = "Express-Hashing-Configurarciones">

### Primeras configurarciones
- requerimos el paquete
- lo importamos
__------------------ ARREGLAR Y AGREGAR: primeras Config --------------------------------------__
 </div>
<div id = "Express-Hashing-Codigo">

### Codigo 
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`bcrypt.hashSync("estring",int)`| Se incripta la string seleccionada con la dificultad enumerada en el int 
|`bcrypt.compareSync(contraseña,contraseñaIncriptada)`| indica si la contraseñas concuerda con la contraseñaIncriptada
</div>  </div>  </div>






# Material Teorico
## Estructura de inicio de express
### Del archivo app.js
```
const express = require("express");
const rutaA = require("./router/router.js")
const methodOverride = require('method-override')
const app = express();

app.listen(300) => inicia el servidor
app.use(methodOverride('_method'))
```
### Del los archivo routers
```
const express = require("express");
const app = express.Routers();
const controller = require("../controllers/controladorControllers.js")
module.imports = router
```
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
## CRUD
### ¿Que es?
 Create, Read, Update y Delete

## HTTP
### Metodos
- get: solicita datos
- post: envia/crea datos
- put: remplaza datos
- patch: modifica parcialmente un dato
- delete: borra datos
### Lineas de codigo necesarias 
`app.use(express.urlencoded({extended:false}));` <br>
`app.use(express.json())`

## Middlewares
### ¿Que es?
Es un bloque de código que se va a ejecutar en la "mitad" de un determinado request
### A nivel de la aplicacion
Son los Middlewares que se ejecutan siempre que se hag aun pedido a la app, se declaran del app.js
### A nivel de las rutas
Son los Middlewares que se ejecutan al momento de ingresar a daterminado link. se declaran como en el siguiente ejemplo: <br>
```
router.get("ruta",(req,res,next) => { codigo }, rutaController.action);
```

## Rutas
### Ruta fija
una ruta la cual siempre lleva el mismo nombre y no es modificado
```
router.get('/item',carritoController.agregarItem)
```
### Ruta parametrisada
ruta la cual el nombre es modificado ya se por un producto, una seccion etc
```
router.get('/:item',carritoController.agregarItem)
```
### Ruta parametrisada obtativa
ruta la cual el nombre es modificado ya se por un producto, una seccion etc y no es obligatoria que este
```
router.get('/:item?',CB)
```
## Carpeta Rutas
para cada ruta.js
`express.Router()` => te permite crear rutas montables y desmontables en nuestra app<br>
`router.get` => para crear las lineas de codico de cada ruta <br>

para app.js
- primero se importa el modulo
- `app.use("/ruta",imporDeRutas)` => el metodo use llama a nnuestras rutas y las utiliza con la funcion que le pasamos

## Error 404
Este error se genera cuando un recurso no se encuentra dentro del servidor
### Codigo
```
app.use((req,res,next) =>{
    res.status(404).render('not-found')
})
```