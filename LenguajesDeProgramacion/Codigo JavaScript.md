# Estructuras
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
switch(valor){
    case "caso1":
        funcion;
    break;

    default:
        funcion;
    }
```
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
# Diferentes funciones segun variables
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
    
## Funcion para Numeros
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`num.toString()`  | pasa el numero a string
|`parseInt(valor)` | pasa de un valor decima a un valor entero

## Funciones para Objetos
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`object.hasOwnPeoperty(propiedad)` | Pregunta si tiene esa propiedad ese objeto
|`object.reduce(function(acumulador,elemento){funcion},acumulador)` | Junta los elementos segun la funcion dada
|`object.map(funcion(valor,indice){Funcion},acumulador)` | Aplica la funcion a cada elemento
|`object.key`|Muestra que contiene la llave
|`object[key]`| devuelve el valor que almacene esa key del objeto de otra forma
|`let object = {...objectA}` | Creo un object con las propiedades de objectA antes declarado

## Funciones de HTML
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`document.write(valor)`    | Muestra el valor en la pantalla
|`prompt(valor)`            | Le pide al ususario un valor 
|`alert(valor)`             | Muestra como alerta el valor

## FS
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`fs.readFileSync("archivo",utg-8)`|lee el archivo indicado en el primer parametro y en el segundo parametro indica el decodificado
|`fs.writeFileSync("archivo",informacionString)`|El archivo es sobreescrito por la informacionString
|`fs.appendFileSync("archivo",informacionString)`|la informacionString se agrega al final del archivo

## path
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`path.join(carpeta1,carpeta2,carpeta3)`| se crea una ruta que indica hacia donde va
|`path.extname(direccion)`|te declara cual es la extencion del archivo
|`path.dirname(direccion)`|te daclara el directorio de un archivo

# Clases
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
# Otros
`nombreDelCiclo:` -> Le pone una etiqueta al ciclo para poder utilizarlo en el caso de break o continue <br>


`continue;` -> No finaliza sino saltea la iteracion <br>
`break;` -> Finaliza el bucle <br>
`process.argv` -> Toma las variables que se pasan por consola despues del node ruta <br>

| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`tipeof valor`    | nos dice el tipo del valor
    
# Modulos
## Variables
`module.exports = nombreDeLaVariable` => __Exportar__ variable del archivo fuente <br>
`module.exports = {variable1, variable2, variable3, ... , variableN}` => Para varias variables <br>
`require("ubicacionDelArchivoFuente")` => __Importar__ variable en un archivo
          
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

# JSON
```
'[{"name":"Argentina","capital":"CABA","reguion":"America"}]'
```
`JSON.parse(datoJSON)` => convierte el dato JSON a objeto literal<br>
`JSON.stringify(datoObjeto)` => convierte el objeto literal en dato JSON<br>

## Como pasar un archivo JSON a javaScript
`fs.readFileSync("rutaDelJson","utf-8")` =>  nos lee y nos guarda el valor<br>

# Objeto Date
## Estructura
let fechaActual = new Date() => crea una variable con el informacion del dividida
## Funciones
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`fechaActual.getDay() `    | Un numero segun el dia de la semana [domingo = 0]
|`fechaActual.getDate()`    | Te da el dia del mes
|`fechaActual.getMoth()`    | Te da el mes en el que te encontras empezado desde 0
|`fechaActual.getFullYear()`| Te retorna el año
|`fechaActual.toUTCString()`| Le da formato al dia 

# Destructuracion
## Para array
```
let array = ["val1", "val2", "val3", ... , "valN"];
let[val1,val2] = array 
```
val1 va ser igual a "val1"
## Para Objetos
```
let object = {nombre : "fran", edad : 19, trabajo : "programador"}
let[nombre,edad] = object
```
cuando declare nombre va almacenar "fran" 

# Express
## Paquetes necesarios y distribucion de carpetas
### paquetes necesarios
#### externos
para una mejor implementaicon de node es necesario descargar estos paquetes de npm:
| descargar                |              requerir          |     Funcion  | | |
|:------------------------:|--------------------------------|---|---|---|
|npm i express             | `require("express")`           | Descarga el paquete basico de express
|npm i method-override     | `require("method-override")`   | Permite subir fotos al servidor
|npm i express-validator   | `require("express-validator")` | Permite validar campos del formulario
|npm i express-session     | `require("express-session")`   | Mantener sesiones aviertas y confg globales
|npm i cookie-parser       | `require('cookie-parser')`     | Sirve para la utilizacion de la coockies en una pagina web
|npm i bcryptjs            | `require('bcryptjs')`          | Se utiliza para incriptar codigo
|npm i ejs --save          |       
#### interno
require(path)
require(fs)
### carpetas utilizadas para una mejor implementacion de express
 mejor definida en el rachivo web.md
> `app.js` en este se implementan todos los arranques de la web
>  __router__ en esta carpeta se guardan todas las direcciones de nuestra web en archivos como `person.js`
> __controller__ en esta carpeta se almacena todas las acciones req res de cada ruta anteriormente mencionada. el nombre de los rachivos es `personController.js`
## Estructura de inicio
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
### Del los archivo routers
```
const controllers{
    rutaA : funcion,
    rutaB : funcion,
    rutaC : funcion,
    rutaD : funcion,
}

module.imports = controllers
```
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
## rutas
### ruta fija
una ruta la cual siempre lleva el mismo nombre y no es modificado
```
router.get('/item',carritoController.agregarItem)
```
### ruta parametrisada
ruta la cual el nombre es modificado ya se por un producto, una seccion etc
```
router.get('/:item',carritoController.agregarItem)
```
### ruta parametrisada obtativa
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

## Middlewares
### que es
es un bloque de código que se va a ejecutar en la "mitad" de un determinado request
### a nivel de la aplicacion
Son los Middlewares que se ejecutan siempre que se hag aun pedido a la app, se declaran del app.js
### a nivel de las rutas
Son los Middlewares que se ejecutan al momento de ingresar a daterminado link. se declaran como en el siguiente ejemplo: <br>
```
router.get("ruta",(req,res,next) => { codigo }, rutaController.action);
```
## Express Validator 
### Primeras comnfigurarciones
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
### Codigo
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`check('nomrbeDelImput').notEmpty()`|obliga que el input no este vacio
|`check('nomrbeDelImput').isEmail()`| obliga que el input sea un mail
|`check('nomrbeDelImput').validacion().withMessage('mensaje de error')`| si la validacion no se cumple salta con este mensaje de error
|`check('nomrbeDelImput').isLength({min : valorMinimo, max: valorMaximo})`| valida si se cumple el rango seleccionado
|`array.isEmpaty()`|nos dice si hay no hay errores de validacion
|`check('nomrbeDelImput').bail()`| corta las siguiente validaciones

## Express session
### Primeras comnfigurarciones
#### app.js
- requerimos elpaquete
- usamos el Middlewares: app.use({secret : "texto"})
### Codigo
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`get.session.parametro`| se almacena de forma global el parametro seleccionado

## Cookies
### Primeras comnfigurarciones
#### app.js
- requerimos el paquete
- lo importamos
- lo configuramos como Middlewares: <br>
`app.use(coockieParser())`

#### controller
- para utilisarse primero se almacena un valor en `res.cookie(nombre,valor,{configuraciones})`
- se llama utilizando la funcion `req.cookie.nombreDelvalor`

## Hashing
### codigo 
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`bcrypt.hashSync("estring",int)`| Se incripta la string seleccionada con la dificultad enumerada en el int 
|`bcrypt.compareSync(contraseña,contraseñaIncriptada)`| indica si la contraseñas concuerda con la contraseñaIncriptada