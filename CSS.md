# estructura
    selector{
        propiedad:valor;
        propiedad:valor;
        propiedad:valor;
    }
# selectores
## universal
    *{

    }
## de etiqueta
    p{

    }
    
## de objeto
    nombreDelObjeto{

    } 
    
## de clase
    .clase{

    } => css
    <h3 class = "nombre de la clase"> </h3> => html
    
## descendente
    .noticia h2{

    } => css
    <ul id = "noticia">
        <h2> nciwontexto modificadoisoenf </h2>
    </ul>
    
## convinada
    h2.noticia => css
    <h2 class = "noticia"> texto modificado</h2>
    
## id
    #nombre{

    } => css
    <h3 id = nombre> texto modificado </h3>

# Estilos
## Tipografia
| codigo                    |explicacion| | | |
|:-------------------------:|---|---|---|---| 
|`color: color`             |se le pone un color a la tipografia
|`font-famili: tipografia`  |se le pone una tipografia al texto
|`font-size: tamaño px`     |se le agrega un tamaño a la tipografia
|`font-style: italica`      |tipografia en cursiba
|`font-weight: bold`        |tipografia en negrita
|`text-aling: left`         |alineacion left(derecha) right(izquierda) center(centrado) justify(jutificado)
|`text-decoration: none`    |agrega un subrallado (underline) o un tachado (line-through)
|`text-transform: none`     |uppercase(todo en mayuscula), lowercase(todo en minusculas)
|`line-height: tamaño`      |distancia entre parrafos

## Colores
| codigo                                |explicacion| | | |
|:-------------------------------------:|---|---|---|---| 
|`color: nombre`                        |aplicar colores con nombre
|`color: porValorHexa`                  |se menciona los 6 digitos hexadecimal
|`color: rgb(rojo,verde,azul)`          |se menciona por rgb
|`color: rgba(rojo,verde,azul,opacidad)`|se le agrega la opacidad al rgb
## Fodos
| codigo                              |explicacion| | | |
|:-----------------------------------:|---|---|---|---| 
|`background-color: color`            |aplica un fonde de un color determinado
|`background-image: url(ubicacion)`   |se agrega una imange de fondo
|`backgroud-repea: repeat`            |se repite indefinidamente  no-repeat(no repite) y el repeat-y/repeat-x(se repite segun un eje)
|`background-position: center botton` |define la posicion de la imagen
|`background-attachment: scroll`      |scroll(baja segun la pagina) fixed (queda fija)
|`background-size: contain `          |tamaño de la imagen contein(que entre la imagen) cover(ocupe toda la pagina )


## De Bloques
| codigo                      |explicacion| | | |
|:---------------------------:|---|---|---|---| 
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
## Otros comandos
| codigo            |explicacion| | | |
|:-----------------:|---|---|---|---| 
|`opacity: valor`   | se le agrega transparencia
|`content: algo`    | se agrega algo al archivo por ejemplo conten: "hola"
|`transition: propiedad tiempo`| se le agrega una trancicion a algun psudocodigo

# tipos de medida
## medida relativa
son aquellas que se modifican segun el contexto alguns ejemplos son:
    % (porsentaje)
    vw (viewport-width)
    vh (viewport-height)
## medidas absolutas
son aquella que no se modifican selgun el contexto algunos ejemplos son:
    px (pixel)

# Media queries
### Es una regla de estilo para que nuestra pagina se vea bien en todas las resoluciones, que se define al final del archivo css
## Estructura
    @media(){

    }
    min-width: x px => como minimo (para mobile first)
    max-width x px  => como maximo (para mobile last)
    and (orientation: ) => si se define una orientacion portrait o landscape
## tipos de forma
mobile first: se empiza por el formato de celular y se va adaptando al modelo de PC (el ma recomendado)
mobile last:  se empieza por el formato de PC a la version de celular 

<img src = "./img/mobile-first.jpg">

## Breakpoints
Son los puntos recomendados en los cuales hacer un Media queries

<img src = "./img/breakpoints.jpg"  height = 200>

# flex
## Estructura basica
    .contenedor{
        displey: flex => hace que los elementos sean flex
        flex-wrap: wrap => matener tamaño de los elementos
    }
## Ejes
| codigo                          |explicacion| | | |
|:-------------------------------:|---|---|---|---| 
|`flex-direction: row`            |Eje principal el ancho de izquiera a derecha
|`flex-direction: column `        |Eje principal el largo de arriba a abajo
|`flex-direction: row-reverse`    |Eje principal el ancho de derecha a izquiera
|`flex-direction: column-reverse` |Eje principal el ancho de abajo a arriba
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


## otros
| codigo                                  |explicacion| | | |
|:---------------------------------------:|---|---|---|---| 
|`flew-flow: <flex-direction> <flex-wrap>`|Convina los dos por ejemplo flew-flow: column warp
|`order: valor`                           |Mueve el elemto al valor pos o neg que se le indeque
|`flex-grow: valor`                       |Agranda un elemento segun el valor que se le indique

# Pseudo selectores
## ¿que es?
es diferenciar un comportamiento al momento de pasar por encima del objeto con un cursor
## Tipos
### Pseudo clases
    .selector:pseudo-clase{
        codigo
    }
### Pseudo codigo
    hs::pseudo-codigo{
        codigo
    }
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


# Posicionamiento
`position: propiedad` <br> algunas de las pociciones son: 
| codigo    |explicacion| | | |
|:---------:|---|---|---|---| 
|static     | Posicionamiento normal
|relative   | Posicionamiento en base a la ubicacion del objeto
|absolute   | El contenedor sera el punto de referencia
|fixed      | No importa si se hace scroll el objeto se matiene
## Mamejo del posicionamiento
| codigo             |explicacion| | | |
|:------------------:|---|---|---|---|
|`top:tamaño px`      | movimiento hacia abajo
|`right: tamaño px`   | movimiento hacia la izquierda
|`bottom: tamaño px`  | movimiento hacia arriba
|`left: tamaño px`    | movimiento hacia la derecha

## pocicionamiento en profundidad
| codigo             |explicacion| | | |
|:------------------:|---|---|---|---|
|`z-index: valor`    | se le aplica un valor tanto positivo como negatativo para posicionarlo 

# Animaciones
## Estructura
```
@keyframes nombre{
    0%{ } estado inicial
    100%{ } estado final
}
```
## Aplicacion
| codigo             |explicacion| | | |
|:------------------:|---|---|---|---|
|`animation-name: nombre`                   |aplicar la animacion
|`animation-duration: tiempo`               |tiempo en la cual va a durar la animacion
|`animation-iteration-count: iteraciones`   |cantidad de veces que se repetira la animacion, infinite para no tereminarla
|`animation: nombre tiempo iteranciones`    |es una abreviatura de las tres anteriores 
|`animation-direction: valor`               |valor puede ser: alternative (la animacion va y viene)  normal (la animacion va en bucle)
# Normalize
## libreria de estilos para web. descarga: 
<a href = "https://necolas.github.io/normalize.css/"> <img src = "./img/normalize.png"></a>
# Agregar iconos
1. entrar a la pagina de font awesome 
<br>
<a href = "https://fontawesome.com/"><img src ="./img/fontAwesome.png" width = 50px> </a>

2. copiar etiqueta del kit para el head
`<script src="https://kit.fontawesome.com/6157b502e6.js" crossorigin="anonymous"></script>`

3. copia el codigo del icomo, algo como esto
`<i class="fa-solid fa-soft-serve"></i>`
