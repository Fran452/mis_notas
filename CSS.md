display:        


# estructura
    selector{
        propiedad:valor
    }

# selectores
## de etiqueta
    p{}
    
## de objeto
    nombreDelObjeto{} 
    
## de clase
    .clase{} => css
    <h3 class = "nombre de la clase"> </h3> => html
    
## descendente
    .noticia h2{} => css
    <ul id = "noticia">
        <h2> nciwontexto modificadoisoenf </h2>
    </ul>
    
## convinada
    h2.noticia => css
    <h2 class = "noticia"> texto modificado</h2>
    
## id
    #nombre{} => css
    <h3 id = nombre> texto modificado </h3>

# Estilos
## Tipografia
    - color: rojo                 => se le pone un color a la tipografia
    - font-famili: tipografia     => se le pone una tipografia al texto
    - font-size: tamaño px        => se le agrega un tamaño a la tipografia
    - font-style: italica         => tipografia en cursiba
    - font-weight: bold           => tipografia en negrita
    - text-aling : left           => alineacion left(derecha) right(izquierda) center(centrado) justify(jutificado)
    - text-decoration : none      => agrega un subrallado con underline o un tachado con line-through
    - text-transforme: none       => uppercase(todo en mayuscula), lowercase(todo en minusculas)
    - line-height: tamaño         => distancia entre parrafos

## Colores
    - color: nombre                           => aplicar colores con nombre 
    - color: porValorHexa                     => se menciona los 6 digitos hexadecimal
    - color: rgb(rojo,verde,azul)             => se menciona por rgb
    - color: rgba(rojo,verde,azul,opacidad)   => se le agrega la opacidad al rgb

## Fodos
    - background-color: color               => aplica un fonde de un color determinado
    - background-image: url(ubicacion)      => se agrega una imange de fondo
    - backgroud-repea: repeat               => se repite indefinidamente  no-repeat(no repite) y el repeat-y/repeat-x(se repite segun un eje)
    - background-position: center botton    => define la posicion de la imagen
    - background-attachment: scroll         => scroll(baja segun la pagina) fixed (queda fija)
    - background-size: contain              => tamaño de la imagen contein(que entre la imagen) cover(ocupe toda la pagina )
## Otros comandos
    - opacity: valor               => se le agrega transparencia
    - display: inline              => cambiar la dispocicion del elemento, block (comportamiento en bloque) inline-block (comportamiento semi-bloque) inline  (comportamiento en linea) none(oculta el elemento)
