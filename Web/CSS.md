<div id = "indice"> <!----- Inicio de indice ------->

# Indice

1. 
| [Estructuras](#estructuras) |
|:-------------------------:|

2. 
| [Selectores](#selectores) |
|:-------------------------:|
|[universal](#selectores-universal)|
|[etiqueta](#selectores-etiqueta)|
|[objeto](#selectores-objeto)|
|[clase](#selectores-clase)|
|[descendente](#selectores-descendente)|
|[convinada](#selectores-convinada)|
|[id](#selectores-id)|
      

3. 
| [Estilos](#estilos) |
|:-------------------------:|
|[Tipografia](#estilos-Tipografia)|
|[Fodos](#estilos-Fodos)|
|[Bloques](#estilos-Bloques)|
|[Otros](#estilos-Otros)|

4. 
|[Medida](#medida) |
|:-------------------------:|
|[relativa](#medida-relativa)|
|[absolutas](#medida-absolutas)|

5. 
|[MediaQueries](#MediaQueries) |
|:-------------------------:|
|[estructura](#MediaQueries-estructura)|
|[tipos](#MediaQueries-tipos)|
|[breakpoints](#MediaQueries-breakpoints)|

6. 
|[Flex](#flex) |
|:-------------------------:|
|[estructura](#flex-estructura)|
|[ejes](#flex-ejes)|
|[otros](#flex-otros)|

  
7. 
|[Pseudo Selectores](#pseudoSelectores) |
|:-------------------------:|
|[Definicion](#pseudoSelectores-Definicion)|
|[tipos](#pseudoSelectores-tipos)|
|[propiedades](#pseudoSelectores-propiedades)|
  

8. 
|[Posicionamiento](#posicionamiento) |
|:-------------------------:|
|[Mamejo del posicionamiento](#posicionamiento-Mamejo)|
|[profundidad](#posicionamiento-profundidad)|

9. 
|[Animaciones](#animaciones) |
|:-------------------------:|
|[Estructura](#animaciones-Estructura)|
|[Aplicacion](#animaciones-Aplicacion)|

10. 
|[Normalize](#Normalize ) |
|:-------------------------:|

11. 
|[iconos](#iconos ) |
|:-------------------------:|

<br>
<br>
</div> <!----- Fin de indice ------->

## [indice](#indice)
<div id = "estructuras"> <!----- Inicio de Estructuras ------->

# Estructuras
    selector{
        propiedad:valor;
        propiedad:valor;
        propiedad:valor;
    }

</div> <!----- Fin de Estructura ------->

## [indice](#indice)

<div id = "selectores"> <!----- Inicio de selectores ------->

# Selectores

<div id = "selectores-universal">  <!----- Inicio de universal ------->

## Universal
    *{

    }

</div>  <!----- Fin de universal ------->
<div id = "selectores-etiqueta">  <!----- Inicio de etiqueta ------->

## Etiqueta
    p{

    }

</div>  <!----- Fin de etiqueta ------->
<div id = "selectores-objeto"> <!----- Inicio de objeto ------->

## objeto
    nombreDelObjeto{

    } 

</div> <!----- Fin de objeto ------->
<div id = "selectores-clase"> <!----- Inicio de clase ------->

## clase
    .clase{

    } => css
    <h3 class = "nombre de la clase"> </h3> => html

</div> <!----- Fin de clase ------->
<div id = "selectores-descendente">  <!----- Inicio de descendente ------->

## descendente
    .noticia h2{

    } => css
    <ul id = "noticia">
        <h2> nciwontexto modificadoisoenf </h2>
    </ul>

</div> <!----- Fin de descendente ------->
<div id = "selectores-convinada "> <!----- Inicio de convinada ------->

## convinada
    h2.noticia => css
    <h2 class = "noticia"> texto modificado </h2>

</div> <!----- Fin de convinada ------->
<div id = "selectores-id"> <!----- Inicio de id ------->

## id
    #nombre{

    } => css
    <h3 id = nombre> texto modificado </h3>

</div> <!----- Fin de id ------->
</div> <!----- Fin de selectores ------->

## [indice](#indice)
<div id = "estilos"> <!----- Inicio de estilos ------->

# Estilos
<div id = "estilos-Tipografia">  <!----- Inicio de Tipografia ------->

## Tipografia
| codigo                    |                                  explicacion                              |    
|:-------------------------:|---------------------------------------------------------------------------|
|`color: color`             |se le pone un color a la tipografia
|`font-famili: tipografia`  |se le pone una tipografia al texto
|`font-size: tamaño px`     |se le agrega un tamaño a la tipografia
|`font-style: italica`      |tipografia en cursiba
|`font-weight: bold`        |tipografia en negrita
|`text-aling: left`         |alineacion left(derecha) right(izquierda) center(centrado) justify(jutificado)
|`text-decoration: none`    |agrega un subrallado (underline) o un tachado (line-through)
|`text-transform: none`     |uppercase(todo en mayuscula), lowercase(todo en minusculas)
|`line-height: tamaño`      |distancia entre parrafos

</div> <!----- Fin de Tipografia ------->
<div id = "estilos-Colores"> <!----- Inicio de Colores ------->

## Colores
| codigo                                |                   explicacion         |
|:-------------------------------------:|---------------------------------------|
|`color: nombre`                        |aplicar colores con nombre
|`color: porValorHexa`                  |se menciona los 6 digitos hexadecimal
|`color: rgb(rojo,verde,azul)`          |se menciona por rgb
|`color: rgba(rojo,verde,azul,opacidad)`|se le agrega la opacidad al rgb

</div> <!----- Fin de Colores ------->
<div id = "estilos-Fodos"> <!----- Inicio de Fodos ------->

## Fodos
| codigo                              |                                 explicacion                                 |
|:-----------------------------------:|-----------------------------------------------------------------------------|
|`background-color: color`            |aplica un fonde de un color determinado
|`background-image: url(ubicacion)`   |se agrega una imange de fondo
|`backgroud-repea: repeat`            |se repite indefinidamente  no-repeat(no repite) y el repeat-y/repeat-x(se repite segun un eje)
|`background-position: center botton` |define la posicion de la imagen
|`background-attachment: scroll`      |scroll(baja segun la pagina) fixed (queda fija)
|`background-size: contain `          |tamaño de la imagen contein(que entre la imagen) cover(ocupe toda la pagina )

</div> <!----- Fin de Fodos ------->
<div id = "estilos-Bloques"> <!----- Inicio de Bloques ------->

## Bloques
| codigo                      |                                  explicacion                                            |
|:---------------------------:|-----------------------------------------------------------------------------------------|
|display: inline              |cambiar la dispocicion del elemento, block (comportamiento en bloque) inline-block (comportamiento semi-bloque) inline  (comportamiento en linea) none(oculta el elemento)
| `width: valor px`           |se aplica un ancho a
| `height: valor px`          |se le aplica un alto al bloque
| `padding:  valor px`        |se le aplica un espacion de separacion a los costados
| `padding-top: valor px`     |se le aplica un espacio al costado superior
| `padding-right: valor px`   | se le aplica un espacio al costado lateral derecha
| `padding-bottom: valor px`  |se le aplica un espacio al costado inferior
| `padding-left: valor px`    |se le aplica un espacio al costado lateral izquierdo
| `border-width: valor px`    |se le aplica una anchura al borde
| `border-style: valor`       |el tipo de linea que se le aplica al borde solid (continua), dashed(discontinua) dotted(de puntos) double (doble linea continua)
| `border-color: color`       |le aplica un color a la linea
| `border-radius: valor px`   |redondea el borde 
| `margin: valor px`          |le aplica margenes a la caja
| `margin-top: valor px`      |se le aplica un margenes al costado superior
| `margin-right: valor px`    |se le aplica un margenes al costado lateral derecha
| `margin-bottom: valor px`   |se le aplica un margenes al costado inferior
| `margin-left: valor px `    |se le aplica un margenes al costado lateral izquierdo
| `box-sizing: border-box `   |fina los valores de alto y ancho del width y height
| `overflow: visible`         | Nos indica que hacer con el exedente visual de la pagina: visible (El contenido no es recortado) hidden (El contenido es recortado y no se muestran barras de posición) scroll (
el contenido es recortado y el navegador web usa las barras de desplazamiento) auto (depende del agente de usuario)

</div> <!----- Fin de Bloques ------->
<div id = "estilos-Otros"> <!----- Inicio de Otros ------->

## Otros comandos
| codigo            |                       explicacion                             |
|:-----------------:|---------------------------------------------------------------|
|`opacity: valor`   | se le agrega transparencia
|`content: algo`    | se agrega algo al archivo por ejemplo conten: "hola"
|`transition: propiedad tiempo`| se le agrega una trancicion a algun psudocodigo

</div> <!----- Fin de Otros ------->
</div> <!----- Fin de estilos ------->

## [indice](#indice)
<div id = "medida"> <!----- Inicio de medida ------->

# tipos de medida
<div id = "medida-relativa"> <!----- Inicio de relativa ------->

## medida relativa
son aquellas que se modifican segun el contexto alguns ejemplos son:
    % (porsentaje)
    vw (viewport-width)
    vh (viewport-height)

</div> <!----- Fin de relativa ------->
<div id = "medida-absolutas"> <!----- Inicio de absolutas ------->

## medidas absolutas
son aquella que no se modifican selgun el contexto algunos ejemplos son:
    px (pixel)

</div> <!----- Fin de absolutas ------->
</div> <!----- Fin de medida ------->

## [indice](#indice)
<div id = "MediaQueries"> <!----- Inicio de MediaQueries ------->

# Media queries
### Es una regla de estilo para que nuestra pagina se vea bien en todas las resoluciones, que se define al final del archivo css

<div id = "MediaQueries-estructura"> <!----- Inicio de estructura ------->

## Estructura
    @media(){

    }
    min-width: x px => como minimo (para mobile first)
    max-width x px  => como maximo (para mobile last)
    and (orientation: ) => si se define una orientacion portrait o landscape

</div> <!----- Fin de estructura ------->
<div id = "MediaQueries-tipos"> <!----- Inicio de tipos ------->

## Tipos de forma
mobile first: se empiza por el formato de celular y se va adaptando al modelo de PC (el ma recomendado)
mobile last:  se empieza por el formato de PC a la version de celular 

<img src = "../img/mobile-first.jpg">

</div> <!----- Fin de tipos ------->
<div id = "MediaQueries-breakpoints"> <!----- Inicio de breakpoints ------->

## Breakpoints
Son los puntos recomendados en los cuales hacer un Media queries

<img src = "../img/breakpoints.jpg"  height = 200>

</div> <!----- Fin de breakpoints ------->
</div> <!----- Fin de MediaQueries ------->

## [indice](#indice)
<div id = "flex"> <!----- Inicio de flex ------->

# flex
<div id = "flex-estructura"> <!----- Inicio de estructura ------->

## Estructura basica
    .contenedor{
        displey: flex => hace que los elementos sean flex
        flex-wrap: wrap => matener tamaño de los elementos
    }

</div> <!----- Fin de estructura ------->
<div id = "flex-ejes"> <!----- Inicio de ejes ------->

## Ejes
| codigo                          |explicacion| | | |
|:-------------------------------:|---|---|---|---| 
|`flex-direction: row`            |Eje principal el ancho de izquiera a derecha
|`flex-direction: column `        |Eje principal el largo de arriba a abajo
|`flex-direction: row-reverse`    |Eje principal el ancho de derecha a izquiera
|`flex-direction: column-reverse` |Eje principal el ancho de abajo a arriba

</div> <!----- Fin de ejes ------->
<div id = "flex-manejo-ejes"> <!----- Inicio de manejo ------->

### Manejo de los ejes
#### Main axis (eje X)
| codigo                          |explicacion| | | |
|:-------------------------------:|---|---|---|---| 
|`justify-content: flex-start`    |valor por defecto
|`justify-content: flex-end`      |envia los objetos al final del axis
|`justify-content: center`        |Centra los elementos
|`justify-content: space-between` |Cepara de manera uniforme los objetos
|`justify-content: space-around`  |Cepara de manera uniforme los objetos con separacion al principio y al final

#### Main Cross (eje y)
| codigo                |explicacion| | | |
|:---------------------:|---|---|---|---| 
|`align-items: stretch`   |Se estiran para acabar todo el contenedor
|`align-items: flex-start`|Se alinean al inicio del cross
|`align-items: flex-end ` |Se ubican al final de cross
|`align-items: center`    |Se ubican en el centro
|`align-items: baseline`  |Muestra elementos en la línea base del contenedor (anulana lign-items )
|`align-self: stretch`    |Se estiran para acabar todo el contenedor (anulana lign-items )
|`align-self: flex-start` |Se alinean al inicio del cross (anulana lign-items )
|`align-self: flex-end`   |Se ubican al final de cross (anulana lign-items )
|`align-self: center`     |Se ubican en el centro (anulana lign-items )
|`align-self: baseline`   |Muestra elementos en la línea base del contenedor (anulana lign-items )

</div> <!----- Fin de manejo ------->
<div id = "flex-otros"> <!----- Inicio de otros ------->

## otros
| codigo                                  |explicacion| | | |
|:---------------------------------------:|---|---|---|---| 
|`flew-flow: <flex-direction> <flex-wrap>`|Convina los dos por ejemplo flew-flow: column warp
|`order: valor`                           |Mueve el elemto al valor pos o neg que se le indeque
|`flex-grow: valor`                       |Agranda un elemento segun el valor que se le indique

</div> <!----- Fin de otros ------->
</div> <!----- Fin de flex ------->

## [indice](#indice)
<div id = "grid"> <!----- Inicio de grid ------->

# Grid 
<!------- A COMPLETAR ----->
</div> <!----- Fin de grid ------->

## [indice](#indice)
<div id = "pseudoSelectores"> <!----- Inicio de pseudoSelectores ------->

# Pseudo selectores

<div id = "pseudoSelectores-Definicion">  <!----- Inicio de Definicion ------->

## ¿que es?
es diferenciar un comportamiento al momento de pasar por encima del objeto con un cursor

</div> <!----- Fin de Definicion ------->
<div id = "pseudoSelectores-tipos">  <!----- Inicio de tipos ------->

## Tipos
### Pseudo clases
    .selector:pseudo-clase{
        codigo
    }
### Pseudo codigo
    hs::pseudo-codigo{
        codigo
    }

</div> <!----- Fin de tipos ------->
<div id = "pseudoSelectores-propiedades">  <!----- Inicio de propiedades ------->

### propiedades:
| codigo             |explicacion| | | |
|:------------------:|---|---|---|---| 
|`.a:visited{}`      |Cuando un link fue visitado
|`.a:link{}`         |Se le aplican estilos a los enlaces
|`.a:active{}`       |Se le aplican estilos a los enlaces que estan por ser clickeados
|`.selector:hover{}` |Cuando el usuario pase el curso del mouse
|`.selector:focus{}` |Cuando el cursos se ubique dentro del formulario
|`.selector::before` |Se le agrega algo antes del selector
|`.selector::after`  |Se le agrega algo despues del selector

</div> <!----- Fin de propiedades -------> 
</div> <!----- Fin de pseudoSelectores ------->

## [indice](#indice)
<div id = "posicionamiento">  <!----- Inicio de posicionamiento -------> 

# Posicionamiento
`position: propiedad` <br> algunas de las pociciones son: 
| codigo    |explicacion| | | |
|:---------:|---|---|---|---| 
|static     | Posicionamiento normal
|relative   | Posicionamiento en base a la ubicacion del objeto
|absolute   | El contenedor sera el punto de referencia
|fixed      | No importa si se hace scroll el objeto se matiene

<div id = "posicionamiento-Mamejo">  <!----- Inicio de Mamejo ------->

## Mamejo del posicionamiento
| codigo             |explicacion| | | |
|:------------------:|---|---|---|---|
|`top:tamaño px`      | movimiento hacia abajo
|`right: tamaño px`   | movimiento hacia la izquierda
|`bottom: tamaño px`  | movimiento hacia arriba
|`left: tamaño px`    | movimiento hacia la derecha

</div> <!----- Fin de Mamejo ------->
<div id = "posicionamiento-profundidad">  <!----- Inicio de profundidad ------->

## pocicionamiento en profundidad
| codigo             |explicacion| | | |
|:------------------:|---|---|---|---|
|`z-index: valor`    | se le aplica un valor tanto positivo como negatativo para posicionarlo 

</div> <!----- Fin de profundidad ------->
</div> <!----- Fin de posicionamiento ------->

## [indice](#indice)
<div id = "animaciones">  <!----- Inicio de animaciones ------->

# Animaciones

<div id = "animaciones-Estructura">  <!----- Inicio de Estructura ------->

## Estructura
```
@keyframes nombre{
    0%{ } estado inicial
    100%{ } estado final
}
```

</div> <!----- Fin de Estructura ------->
<div id = "animaciones-Aplicacion">  <!----- Inicio de Aplicacion ------->

## Aplicacion
| codigo             |explicacion| | | |
|:------------------:|---|---|---|---|
|`animation-name: nombre`                   |aplicar la animacion
|`animation-duration: tiempo`               |tiempo en la cual va a durar la animacion
|`animation-iteration-count: iteraciones`   |cantidad de veces que se repetira la animacion, infinite para no tereminarla
|`animation: nombre tiempo iteranciones`    |es una abreviatura de las tres anteriores 
|`animation-direction: valor`               |valor puede ser: alternative (la animacion va y viene)  normal (la animacion va en bucle)

</div> <!----- Fin de Aplicacion ------->
</div> <!----- Fin de animaciones ------->

## [indice](#indice)
<div id = "Normalize"> <!----- Inicio de Normalize ------->

# Normalize
## libreria de estilos para web. descarga: 
<a href = "https://necolas.github.io/normalize.css/"> <img src = "../img/normalize.png"></a>
</div> <!----- Fin de Normalize ------->

## [indice](#indice)
<div id = "iconos">  <!----- Inicio de iconos ------->

# Agregar iconos
1. entrar a la pagina de font awesome 
<br>
<a href = "https://fontawesome.com/"><img src ="../img/fontAwesome.png" width = 50px> </a>

2. copiar etiqueta del kit para el head
`<script src="https://kit.fontawesome.com/6157b502e6.js" crossorigin="anonymous"></script>`

3. copia el codigo del icomo, algo como esto
`<i class="fa-solid fa-soft-serve"></i>`

</div> <!----- Fin de iconos ------->