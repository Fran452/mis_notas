# descargar framework
    $ npm init -y
    $ npm install express --save

# correr un sitio web

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
