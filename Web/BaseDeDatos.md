# CRUD
## que es
 Create, Read, Update y Delete

# HTTP
## metodos
- get: solicita datos
- post: envia/crea datos
- put: remplaza datos
- patch: modifica parcialmente un dato
- delete: borra datos
## lineas de codigo necesarias 
`app.use(express.urlencoded({extended:false}));` <br>
`app.use(express.json())`

# Multer
## implementacion
### JS
- npm i multer
- const multer = require('multer')
- configurar multer
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
- especificar que configuracion se va a usar: `let fileUpload = multer({storage: storage});`
- configurar ruta: se le agrega el upload.single("nombre del formulario") para que la ruta sepa que parte del formulario permite guardar fotos. ejemplo: <br>
`router.post('/register',upload.single("fotoDePerfil"),(req,res)=>{})` para subir una imagne <br>
upload.any("fotoDePerfil")

### HTML
- agregar al formulario la propiedad `enctype="multipart/form-data"`

# Validacion de documentos
## Implementacion
### JS
- npm i express-validator
- const {body} = require('express-validator')
- configuracion de validaciones: <br>
```
const validaciones =[
    body('nombre').notEmpaty(),
    body('mail').notEmpaty(),
    body('contraseña').notEmpaty(),
];
```
- y en el registro de rutas el siguiente codigo <br>
`router.post('/register', validaciones, controlador.registrar);`
- en el controlador: <br>

```
const {validationResult} = require('express-validator');

registrar: (req,res) => {
    let error = validationResult(req)
}
```
en la variable let error se guardan los objetos con  errores

