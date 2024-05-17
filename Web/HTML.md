<div id = "indice">

# Indice
1. 
|[Definicion](#Que-es)|
|:-------------------------:|

2. 
|[Conformacion](#Conformacion)|
|:-------------------------:|

3. 
|[Etiquetas](#etiquetas)| |
|:-------------------------:|----|
|[Tipos](#etiquetas-tipos)|[Texto](#etiquetas-tipos-texto) <br> [lista](#etiquetas-tipos-lista) |
|[Vinculos](#etiquetas-vinculos)|
|[Semantica](#etiquetas-semantica)|
|[Botones](#etiquetas-botones)|

4. 
|[tabla](#tabla)|
|:-------------------------:|
|[estructura](#tabla-estructura)|
|[propiedades](#tabla-propiedades)|
|[otros](#tabla-otros)|

5. 
|[Atributos](#atributos)|
|:-------------------------:|
|[Partes](#atributos-partes)|


6. 
|[estructura](#estructura)|
|:-------------------------:|
|[Basica](#estructura-Basica)|
|[Compleja](#estructura-Compleja)|

7. 
|[Elementos](#elementos)|
|:-------------------------:|
|[Linea](#elementos-linea)|
|[Bloque](#elementos-bloque)|

8. 
|[Metadato](#Metadato)|
|:-------------------------:|
|[Estructura](#Metadato-estructura)|
|[Tipos](#Metadato-Tipos)|

9. 
|[Google Fonts](#Google-Fonts)|
|:-------------------------:|

10.    
|[EJS](#EJS)|
|:-------------------------:|
|[¿Que es?](#EJS-que)       |
|[Intalacion](#EJS-Intalacion)|
|[Etiquetas](#EJS-Etiquetas)|
|[Parametros](#EJS-Parametros)|

</div>

<div id = "Que-es">

## |[indice](#indice)|
# ¿Que es HTML?
Por sus siglas en ingles HyperText Markup Language es un lenguaje dedicado al maquetado de paginas web.
</div>
<div id = "Conformacion">

## |[indice](#indice)|
# Conformacion
Se forma por etiquetas de apertura `<etiqueta>` y de cierre `</etiqueta>`
</div>
<div id = "etiquetas">

## |[indice](#indice)|
# Etiquetas
Son la base del lenguaje
<div id = "etiquetas-tipos">

## tipos de etiqueta:
<div id = "etiquetas-tipos-texto">

### de texto
|        etiqueta       |                       funcion                      |
|:---------------------:|----------------------------------------------------|
|`<h1> </h1>`           | Titlos
|`<h2> </h2>`           | Subtitulo
|`<h..> </h..>`         | Del 3 al 6 para diferencia titulos de forma escalada
|`<p> </p>`             | Bloques de texto
|`<strong> </strong>`   | Textos en negrita (no se usa)
|`<em> </em>`           | Textos en cursiba (no se usa)
|`<span> </span>`       | Elemento de linea 
|`<div> </div>`         | Elemento de bloque
|`<br>`                 | Salto de linea
|`<b> </b>`             | Texto en negrita (no se usa)
|`<i> </i>`             | Tecto en cursiva (no se usa)
|`<strik> </strik>`     | Texto tachado (no se usa)
|`<small> </small>`     | Chiquita (no se usa)
|`<center> </center>`   | Centra tanto texto como imagenes (no se usa)
</div>
<div id = "etiquetas-tipos-lista">

### lista
|        etiqueta       |        funcion          |
|:---------------------:|-------------------------|
| `<ul> </ul>`          | Lista desordenada       |
| `<ol> </ol>`          | Lista oredenada         |
| `<li> </li>`          | Elemeto de la lista     |



#### atributo
    type = "" => se puede cambiar el typo 
        en ol siendo numerico (1), alfabetico(A) o romanos (I)
        en ul siendo disc, circle, square, none
    star = "" => valor de inicio de la ul
</div> </div>


<div id = "etiquetas-vinculos">

## Vinculos
    <img 
        src = "rutaDeLaImagen" 
        alt = "texto descriptiba"
        title = "titulo de la imagen" 
        width = "ancho de la imange"
        height "alto de la imagen"
    > | para subir imagenes
    <a href = "enlace web" target = "donde se abriar el recurso"> 
        texto 
    </a> => para subir links

    <script src = "archivo.js">  </script> => codigo JS en el head
</div>
<div id = "etiquetas-semantica">

## Semantica
|        etiqueta       |        funcion          |
|:---------------------:|-------------------------|
|`<header> </header>`   |Se utiliza para la cabecera del la pagina
|`<nav> </nav>`         |Barra de navegacion
|`<footer> </footer>`   |Pie de pagina de una pagina
|`<section> </section>` |Seccion de contenido monotematica
|`<articol> </articol>` |Pieza de contenido indepediente
</div>

<div id = "etiquetas-botones">

## Botones
    <button type= "reset">texto</button> => elimina el formulario
    <button type= "<">enviar</button> => envia el formulario
    <button type= "button">algo</button> => se programa en JS
</div> </div>


<div id = "tabla">

## [indice](#indice)
# Tabla
<div id = "tabla-estructura">


## Estructura
    <table>             => creacion de tabla
        <tr>            => fila
            <td> </td>  => columna
        </tr>
    </table>

</div>
<div id = "tabla-propiedades">

## Propiedades
    <table border = 1px> => se le da un borde de x px
</div>
<div id = "tabla-otros">

## otros importantes
    <marquee> </marquee> => crea un texto que se desplaza de derecha a izquierda de la plantalla
</div> </div>


<div id = "atributos">

## |[indice](#indice)|
# Atributos:
caracteristica de la etiqueta a modificar

<div id = "atributos-partes">

## partes del atributo:
    nombre                      |
    =                            > <h1 aling="center"> hola mundo </h1>
    valor del atributo entre "" |         atributo
</div> </div>


<div id = "estructura">

## [indice](#indice)
# Estructura 

<div id = "estructura-Basica">

## Basica
    <!DOCTYPE html>     => version del lenguaje 
    <html lang="en">    => definicion de ht

    <head>              => definicion referente al documento
        <meta charset="UTF-8">  => define el uso de la codificacion del documento (legunaje español (ñ á é í ó ú, etc))
    </head>             => cierre de head           

    <body>              => cuerpo del html 
            
    </body>             => cierre del body

    </html>
</div>
<div id = "estructura-Compleja">

## Compleja
    <!DOCTYPE html>     => version del lenguaje 
    <html lang="en">    => definicion de ht

    <head>              => definicion referente al documento
        <meta charset="UTF-8">       => define el uso de la codificacion del documento (legunaje español (ñ á é í ó ú, etc))
        <link rel = "icon" href = "ubicacion del .ico">   => icono de la web        
        <title>Document</title>       => se define lo que se mostrara en la pestaña del navegador
        <meta name="viewport" content = "widthe=divace-wid th, initial-scale=1"> => hacer escalable la pagina
        <link rel = "stylesheet" href = "./rutaDelArchivo/style.css">   => vincular css con HTML
        <>

    </head>             => cierre de head           

    <body>              => cuerpo del html 
            
    </body>             => cierre del body

    </html>
</div> </div>
<div id = "elementos">

## Elementos
<div id = "elementos-linea">

### de linea 
solo ocupan el espacio del contenido interno
</div>
<div id = "elementos-bloque">

### de bloque
independiente del contenido ocupara el ancho correspondiente
</div> </div>

<div id = "Metadato">

## [indice](#indice)
# Metadato

<div id = "Metadato-estructura">

## Estructura
`<meta name = "" conten = ""> `
</div>
<div id = "Metadato-Tipos">

## Tipos
    <meta name = "keyword" conten = "etiquetas"> 
    <meta name = "description" conten = "descripcion de la pagina"> 
    <meta name = "author" conten = "autor de la pagina "> 
    <meta name = "copyright" conten = "empresa con copyrigth"> 
    <meta name = "robots" conten = "index/noindex">  => es o no indexada
    <meta name="viewport" content = "widthe=divace-wid th, initial-scale=1"> => hace escalable una pagina web
</div> </div>
<div id = "Google-Fonts">

## [indice](#indice)
# Agregar Tipografia Google Fonts
- se entra a la pagina de google fonts:
<a href= "https://fonts.google.com/"> <img src="../img/googleFonts.png" width = 80px></a>
- se copia la tipografia de la pagina el link
ejemplo:
    
    `<link href="https://fonts.googleapis.com/css2?family=Roboto+Serif:wght@100&display=swap" rel="stylesheet">` 
<br>

    `<link rel="preconnect" href="https://fonts.googleapis.com">`
<br>

    `<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>`
    

- luego se aplica el formato en css:

    `h1{
       font-family: 'Roboto Serif', sans-serif;
    }`
</div>
<div id = "EJS">

## [indice](#indice)
# EJS
<div id = "EJS-que">

## ¿Que es?
Es un Template Engine. Esto permite que mis archivos html sean completamente dinamicos asi poder reutilizar la estructura
</div>
<div id = "EJS-Intalacion">

## Intalacion
> primero lo intalamos en nuestro proyecto con : `npm install ejs --save`
> agregar el codigo corresponediente en nuestro app.js: `app.set("view engine","ejs");`
> agregar la ruta donde se encuentran nuestros archivos ejs: ejemplo: `app.set("view","./src/views");`
> y modificar todos los .html a .ejs 
</div>
<div id = "EJS-Etiquetas">

## Etiquetas especiales
| Codigo                  |Funcion|
|:-------------------------:|---|
|`<% codigo %>` |entre este codigo se implementa el codigo JS|
|`<%= codigo %>`|se utiliza para que el contenido sea impreso de forma literal en el html|
|`<%-include(ubicacion) %>`|incluye un codigo guardado anteriormente y reutilizable|
</div>
<div id = "EJS-Parametros">

## Parametros Compartidos
Vamos a poder compartir con la vista cualquier tipo de dato existente en JavaScript
</div> 
</div>
