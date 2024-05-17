# Formulario
<div id = "indice">

# Indice
1. 
|[estructura](#estructura)|
|:-------------------------:|

2. 
|[Tipos](#Tipos)| 
|:-------------------------:|
|[Enviar ](#Tipos-Enviar)|
|[Oculta](#Tipos-oculta)|
|[Modificar](#Tipos-modificar)|
|[Eliminar](#Tipos-eliminar)|

3. 
|[Etiquetas](#Etiquetas)| 
|:-------------------------:|
|[Type](#type)|

4.     
|[Otras etiquetas](#etiquetas-Poseen)| 
|:-------------------------:|
|[Formulario](#etiquetas-Poseen-Formulario)|
|[Input](#etiquetas-Poseen-Input)|
|[Label](#etiquetas-Poseen-Label)|
|[Lista](#etiquetas-Poseen-Lista)| 
|[Radio Buttons](#etiquetas-Poseen-Radio-Buttons)| 

5. 
|[Estructuras](#estructura)| 
|:-------------------------:|
|[Marcado](#estructura-marcado)|
|[Una Opcion](#estructura-unaOpcion)|
|[Varias Opcione](#estructura-variasOpcione)|
  

</div>
<div id = "estructura">

## |[indice](#indice)|
# Creaci en HTML
    <form  action = "" method = "">
        etiquetas
    </form>
</div>
<div id = "Tipos">

## |[indice](#indice)|
# Tipos de formularios 

<div id = "Tipos-Enviar">

## Enviar los datos por el link
```
<form  method = "GET" action = "/user/buscar">
    etiquetas
</form>
```
</div>
<div id = "Tipos-oculta">

## Enviar los datos de forma oculta
```  
<form  method = "POST" action = "/user/register">
    etiquetas
</form>
```
</div>
<div id = "Tipos-modificar">

## Editar los valores de un objeto ya creado
```
<form  method = "POST"  action = "/user/register?_method=PUT">
    etiquetas
</form>
```
</div>
<div id = "Tipos-eliminar">

## Eliminar objeto
```
<form  method = "POST" action = "/user/register?_method=DELETE">
    <button type = "submit"></button>
</form>
```
</div> </div>
<div id = "Etiquetas">

## |[indice](#indice)|
# Etiquetas importante

|           Tipo                     |          Funcion                 |
|:----------------------------------:|----------------------------------|
|`<input type= "" name = "">`        | Valores del formulario
|`<label> </label>`                  | Agrega texto plano al formulario
|`<textarea></textarea>`             | Campo de texto que se puede modificar
|`<textarea readonly=""></textarea>` | Campo de texto solo de lectura
|`<select> </select>`                | Crea lista de opciones
|`<option> </option>`                | Opciones de la lista select
|`<span> </span>`                    | Muestra un determinado mensaje de error
|`<fieldset></fieldset>`             | Toma parte del formulario
|`<legend></legend>`                 | Pone un texto en le marcado de fieldset

<div id = "type">

## tipos de type
|           Tipo                  |          Funcion                 |
|:-------------------------------:|----------------------------------|
|`type = "text" `                 | Tipea texto
|`type = "password"`              | Contraseña
|`type = "numbre"`                | Numero
|`type = "email"`                 | Obligatorio que sea un mail
|`type = "color"`                 | Eleccion de color
|`type = "date"`                  | Poner un fecha
|`type = "time"`                  | Poneruna hora
|`type = "file"`                  | Explorador de archivos
|`type = "submit"`                | Enviar formulario
|`type = "tel"`                   | Desplega teclado numerico
|`type = "renge" min = "" max ""` | Poner un rango que va desde el min hasta el max
|`type = "radio"`                 | Casilla circular de marcado unico
|`type = "checkbox"`              | Casilla cuadrada de marcado multiple

para mas informacion <a href = "https://developer.mozilla.org/es/docs/Web/HTML/Element/input"> link </a>
</div> </div>
<div id = "etiquetas-Poseen">

## |[indice](#indice)|
# Etiquetas que poseen

<div id = "etiquetas-Poseen-Formulario">

## Formulario
|           Tipo            |          Funcion                 |
|:-------------------------:|----------------------------------|
|`action = "direccion"`     | Define la ruta en donde se va a procesar la informacion
|`method = "metodo"`        | Define como se va a enviar la informacion (GET POST) 
|`required = ""`            | Oblia a completar el capo
</div>
<div id = "etiquetas-Poseen-Input">

## Input
|           Tipo            |          Funcion                 |
|:-------------------------:|----------------------------------|
|`name = "nombre"`          | Identifica al campo
|`id = "nombre"`            | Asocia el input con el label
|`value = "" `              | Se le da un valor de por si
|`placeholder = "texto"`    | Se ingresa un texto de ejemplo
|`required `                | Campo obligatorio
|`multiple `                | Permite seleccionar varios archivos
|`accept = ".jpg, .png"`    | Archivos que acepta la etiqueta type "file"
|`min = ""`                 | Se agrega un valor minimo tanto a range como a date
|`max = ""`                 | Se agrega un valor maximo tanto a range como a date
|`cols = valor`             | Cantidad de columnas segun el valor 
|`rows = valor`             | Cantidad de lineas de texto segun el valor
</div>
<div id = "etiquetas-Poseen-Label">

## Label
|           Tipo            |          Funcion                    |
|:-------------------------:|-------------------------------------|
| `for = "nombre"`          | asocia el campo con su propiedad id |  
</div>
<div id = "etiquetas-Poseen-Lista">

## Lista
|           Tipo            |          Funcion                 |
|:-------------------------:|----------------------------------|
|`value = ""`               | Opcion enviada del `<option>`    | 
|`selected`                 | Opcion pre seleccionada          |      
</div>
<div id = "etiquetas-Poseen-Radio-Buttons"> 

## Radio buttons
|           Tipo            |          Funcion                 |
|:-------------------------:|----------------------------------|
| `checked`                 |       preselecciona el boton     |
</div> </div>
<div id = "estructura">

## |[indice](#indice)|
# Agunas estructura
<div id = "estructura-marcado">

## estructura simpre de formulario de marcado
    <label> <input type = "checkbok"> nombre </label> => estructura de casilla de macardo
</div>
<div id = "estructura-unaOpcion">

## estructura compleja de formulario de marcado de una opcion
    <label><input name = "cassila" type = "radio" value= "opcion A"> opcion A</label>
    <label><input name = "cassila" type = "radio" value= "opcion B"> opcion B</label>    
    <label><input name = "cassila" type = "radio" value= "opcion C"> opcion C</label>  
</div>
<div id = "estructura-variasOpciones">

## estructura compleja de formulario de marcado de varias opciones
    <label><input name = "cassila" type = "checkbox" value= "opcion A"> opcion A</label>  
    <label><input name = "cassila" type = "checkbox" value= "opcion B"> opcion B</label>   
    <label><input name = "cassila" type = "checkbox" value= "opcion C"> opcion C</label>  

</div> </div>