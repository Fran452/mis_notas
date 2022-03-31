# Formulario

# Creaci en HTML
    <form  action = "" method = "">
        etiquetas
    </form>

## Tipos de formularios 
## Enviar los datos por el link
    <form  method = "GET" action = "/user/buscar">
        etiquetas
    </form>
## Enviar los datos de forma oculta
    <form  method = "POST" action = "/user/register">
        etiquetas
    </form>
## Editar los valores de un objeto ya creado
    <form  method = "POST"  action = "/user/register?_method=PUT">
        etiquetas
    </form>
## Eliminar objeto
    <form  method = "POST" action = "/user/register?_method=DELETE">
        <button type = "submit"></button>
    </form>
## Etiquetas importante

    <input type= "" name = ""> => valores del formulario
    <label> </label> => agrega texto plano al formulario
    <textarea></textarea> => campo de texto que se puede modificar
    <textarea readonly=""></textarea> => campo de texto solo de lectura
    <select> </select> => crea lista de opciones
    <option> </option> => opciones de la lista select
    <span> </span>     => muestra un determinado mensaje de error
    <fieldset></fieldset> => toma parte del formulario
    <legend></legend>   => pone un texto en le marcado de fieldset

### tipos de type

    type = "text"      => tipea texto
    type = "password" => contraseña
    type = "numbre"    => numero
    type = "email"     => obligatorio que sea un mail
    type = "color"     => eleccion de color

    type = "date"      => poner un fecha
    type = "time"      => poneruna hora
    type = "file"      => explorador de archivos
    type = "submit"    => enviar formulario
    type = "tel"       => desplega teclado numerico
    type = "renge" min = "" max "" => poner un rango que va desde el min hasta el max
    type = "radio"  => casilla circular de marcado
    type = "checkbox"   => casilla cuadrada de marcado

para mas informacion <a href = "https://developer.mozilla.org/es/docs/Web/HTML/Element/input"> link </a>

## etiquetas que poseen
### el formulario
    action = "direccion" => define la ruta en donde se va a procesar la informacion
    method = "metodo"   => define como se va a enviar la informacion (GET POST) 
    required = "" => oblia a completar el capo
### input
    name = "nombre" => identifica al campo
    id = "nombre"   => asocia el input con el label
    value = ""      => se le da un valor de por si
    placeholder = "texto" => se ingresa un texto de ejemplo
    required        => campo obligatorio
    multiple        => permite seleccionar varios archivos
    accept = ".jpg, .png" => archivos que acepta la etiqueta type "file"
    min = ""            => se agrega un valor minimo tanto a range como a date
    max = ""            => se agrega un valor maximo tanto a range como a date
    cols = valor        => cantidad de columnas segun el valor 
    rows = valor        => cantidad de lineas de texto segun el valor

### label
    for = "nombre" => asocia el campo con su propiedad id

### lista
    value = "" => opcion enviada del <option>
    selected => opcion pre seleccionada

### radio buttons
    checked  => preselecciona el boton

# Agunas estructura
## estructura simpre de formulario de marcado
    <label> <input type = "checkbok"> nombre </label> => estructura de casilla de macardo
## estructura compleja de formulario de marcado de una opcion
    <label><input name = "cassila" type = "radio" value= "opcion A"> opcion A</label>
    <label><input name = "cassila" type = "radio" value= "opcion B"> opcion B</label>    
    <label><input name = "cassila" type = "radio" value= "opcion C"> opcion C</label>  
## estructura compleja de formulario de marcado de varias opciones
    <label><input name = "cassila" type = "checkbox" value= "opcion A"> opcion A</label>  
    <label><input name = "cassila" type = "checkbox" value= "opcion B"> opcion B</label>   
    <label><input name = "cassila" type = "checkbox" value= "opcion C"> opcion C</label>  