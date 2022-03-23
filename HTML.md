Que es HTML
    lenguan

Como se forma
    se forma por etiquetas <> </>

# Etiquetas
Son la base del lenguaje

## tipos de etiqueta:
### de texto
    <h1> </h1>    => titlos
    <h2> </h2>     => subtitulo
    <h..> </h..>   => del 3 al 6 para diferencia titulos de forma escalada
    <p> </p>       => bloques de texto
    <strong> </strong> => textos en negrita
    <em> </em>         => textos en cursiba
    <span> </span> => elemento de linea
    <div> </div>   => elemento de bloque
    <br>           => salto de linea
    <b> </b>       => texto en negrita
    <i> </i>       => tecto en cursiva
    <strik> </strik> => texto tachado 
    <small> </small> => chiquita
    <center> </center> => centra tanto texto como imagenes

### lista
    <ul> </ul> => lista oredenada
    <ol> </ol> => lista desordenada
    <li> </li> => elemeto de la lista
#### atributo
    type = "" => se puede cambiar el typo 
        en ul siendo numerico (1), alfabetico(A) o romanos (I)
        en ol siendo disc, circle, square, none
    star = "" => valor de inicio de la ul
        
## de vinculos
    <img 
        src = "rutaDeLaImagen" 
        alt = "texto descriptiba"
        title = "titulo de la imagen" 
        width = "ancho de la imange"
        height "alto de la imagen"
    > => para subir imagenes
    <a href = "enlace web" target = "donde se abriar el recurso"> 
        texto 
    </a> => para subir links
        
## semantica
    <header> </header>      => se utiliza para la cabecera del la pagina
    <nav> </nav>            => barra de navegacion
    <footer> </footer>      => pie de pagina de una pagina
    <section> </section>    => seccion de contenido monotematica
    <articol> </articol>    => pieza de contenido indepediente
## Botones
    <button type= "reset">texto</button> => elimina el formulario
    <button type= "submit">enviar</button> => envia el formulario
    <button type= "button">algo</button> => se programa en JS
# Tabla
## Estructura
    <table>             => creacion de tabla
        <tr>            => fila
            <td> </td>  => columna
        </tr>
    </table>
## propiedades
    <table border = 1px> => se le da un borde de x px
## otros importantes
    <marquee> </marquee> => crea un texto que se desplaza de derecha a izquierda de la plantalla
# Atributos:
caracteristica de la etiqueta a modificar
    
## partes del atributo:
    nombre                      |
    =                            > <h1 aling="center"> hola mundo</h1>
    valor del atributo entre "" |         atributo

# Estructura 
## Basica
    <!DOCTYPE html>     => version del lenguaje 
    <html lang="en">    => definicion de ht

    <head>              => definicion referente al documento
        <meta charset="UTF-8">  => define el uso de la codificacion del documento (legunaje español (ñ á é í ó ú, etc))
    </head>             => cierre de head           

    <body>              => cuerpo del html 
            
    </body>             => cierre del body

    </html>

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

## Elementos
### de linea 
solo ocupan el espacio del contenido interno
### de bloque
independiente del contenido ocupara el ancho correspondiente

# Metadato
## Estructura
    <meta name = "" conten = ""> 
## Tipos
    <meta name = "keyword" conten = "etiquetas"> 
    <meta name = "description" conten = "descripcion de la pagina"> 
    <meta name = "author" conten = "autor de la pagina "> 
    <meta name = "copyright" conten = "empresa con copyrigth"> 
    <meta name = "robots" conten = "index/noindex">  => es o no indexada
    <meta name="viewport" content = "widthe=divace-wid th, initial-scale=1"> => hace escalable una pagina web

# Agregar Tipografia Google Fonts
- se entra a la pagina de google fonts:
<a href= "https://fonts.google.com/"> <img src="./img/googleFonts.png" width = 80px></a>
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


# EJS
## ¿Que es?
Es un Template Engine. Esto permite que mis archivos html sean completamente dinamicos asi poder reutilizar la estructura
## Intalacion
> primero lo intalamos en nuestro proyecto con : `npm install ejs --save`
> agregar el codigo corresponediente en nuestro app.js: `app.set("view engine","ejs);`
> y mnodificar todos los .html a .ejs 

## Etiquetas especiales
| Codigo                  |Funcion| | | |
|:-------------------------:|---|---|---|---|
|`<% codigo %>` |entre este codigo se implementa el codigo JS|
|`<%= codigo %>`|se utiliza para que el contenido sea impreso de forma literal en el html|
## Parametros Compartidos
Vamos a poder compartir con la vista cualquier tipo de dato existente en JavaScript
### Codigo
