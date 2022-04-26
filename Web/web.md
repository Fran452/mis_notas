# Descargar framework
    $ npm init -y
    $ npm install express --save

# Correr un sitio web

    const express = require("express");
    const app = express();

    app.listen(puerto,funcionDeEjecucion); => pone en linea el codigo en el puerto
    
    app.get(ruta,funciton(req,res,next){   |
        funcion                             > envia respuestas al sitio web, 
    })                                     |    req(contiene propiedades y metodos de la peticion que llego)
                                                res(respuestas que vamos a enviar)

    const path = require("path");

    app.use(path.resolve(__dirname,"./ubicacion")) => uso de archivo estaticos

    app.use(express.static("ubicacion"))  => expone carpeta al usuario


    app.get('/', function(req,res){
        res.sendFile(path.join(__dirname,"./views/home.html")); => inicio de una pagina web 
    });

# vincular css con html

    <!DOCTYPE html>     => version del lenguaje 
        <html lang="en">    => definicion de ht

        <head>              => definicion referente al documento
            <meta charset="UTF-8"  => define el uso de la codificacion del documento (legunaje español (ñ á é í ó ú, etc))            
            <title>Document</title> => se define lo que se mostrara en la pestaña del navegador
            <link rel = "stylesheet" href = "./rutaDelArchivo/style.css"> 
        </head>             => cierre de head           

        <body>              => cuerpo del html 
                
        </body>             => cierre del body

        </html>

# Orden de carpetas
    |_ node_modules
    |_ public
        |_img
            |_ imagenes a utilizar   
        |_css
            |_ styleMain.css
            |_ styleProductosGeneral.css
            |_ stylesProductosEspesifico.css
    |_ src
        |_controllers
            |_ productosControllers.js
            |_ mainControllers.js
            |_ etc 
        |_rotures
            |_ productos.js
            |_ main.js
            |_ etc
        |_views
            |_ partials
                |_index.ejs
            |_ Main.html
            |_ ProductosGeneral.html
            |_ ProductosEspesifico.html
        |_
        |_ app.js
    |_ package-lock.json
    |_ package.json
    |_ README.md

# Express
## paquete pre armado 
- sudo npm install express-generator -g
- express nombreDelProyecto --ejs
- cd nombreDelProyecto
- npm install

# Motores de vista
nos permiten crear una estructura dinamica para las vistas de nuestro proyecto

# Proceso de inicio de sesion
## librerias necesarias:
