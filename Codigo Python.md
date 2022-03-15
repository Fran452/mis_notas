# varios 
| codigo                |explicacion| | | |
|:-------------------:  |---|---|---|---|
| `print("texto")`      |muestra en cosola el texto
| `inputo("texto)`      | muestra por consola el texto y espera resibir un valor
|`id(variable)`         |ubicacion de memoria de la variable
|`int(variable)`        |combierte la variable en int
|`float(variable)`      |combierte la variable en float
|`type(variable)`       |el tipo de la variable
|`#`                    |comentario
|`__name__`             |muestra la ubicacion de donde se utiliza el codigo
|`del variable`         |elimina el objeto

# funciones para listas
| codigo                            |explicacion| | | |
|:-------------------:              |---|---|---|---|
|`len(lista)`                       |cantidad de elementos dentro de la lista
|`lista[valorInicial : valorFinal]` |toma los valores entre el valorInicial y el valorFinal sin incluirlos
|`lista.append(valor)`              |agrega un elemento al final de la lista
|`lista.insert(indice,valor)`       |agrega un elemento en un indice especifico de la lista
|`lista.romeve(valor)`              |remueve el valor de la lista
|`lista.pop()`                      |elimina el ultimo valor de la lista
|`del lista[indice]`                |elimina un elemento de la lista por indice
|`lista.clear()`                    |elimina todos los valores de la lista
|`list(tupla)`                      |convierte la tupla en una lista
|`tuple(lista)`                     |convierte la lista en tupla

# funciones para set
| codigo                |explicacion| | | |
|:-------------------:  |---|---|---|---|
|`len(set)`             |cantidad de elementos
|`valor in set`         |si el valor esta en el set 
|`set.add(valor)`       |agrega valor en el set
|`set.remove(valor)`    | elimina valor del sat 
|`set.discard(valor)`   |elimina valor del set (de no estar no arroja error)
|`set.clear()`          |elimina todos los valores dentro de set
|`del set`              |elimina el set

# funciones para diccionarios
| codigo                                      |explicacion| | | |
|:-------------------:                        |---|---|---|---|
|`len(dicc)`                                  |tamaño de diccionario
|`dicc[key]`                                  |acceder a la definicion de la key
|`dicc.get(key)`                              |acceder a la definicion de la key
|`for key,definicion in dicc.items()`         |recorre un diccionario con las llaves y las definiciones
|`for key,definicion in dicc.key()`           |recorre un diccionario con las llaves
|`for key,definicion in dicc.values()`        |recorre un diccionario con  las definiciones 
|`key in dicc `                               |si la key esta en el diccionario
|`dicc["nueva llave"] = "nueva definicion`    |agrega un nuevo elemento al diccionario
|`dicc.pop(key)`                              |elimina un elemento del diccionario
|`dicc.clear()`                               |elimina todos los valores del diccionario
|`del dicc`                                   |elimina el diccionario

# funcion y estructuras de la clase
## Tipo de clases
La clase es un molde para la creacion ya bien de objetos o de clases "hijas" que heredaran toda la estructura de la base
```
class Persona
    def __init__(self,nombre,apellido):     |
    self.nombre =  nombre                    > contructor de clase
    self.apellido =  apellido               |
    self._nombre1 = nombre                   => variable la cual no se puede modificar

    def nombreDelMetodo(self):                  |
    metodo                                       > creacion de metodos en clase
```
## Clase hijas
Son clases provenientes de otras clase ya exixtente, pueden crearse a partir de una o varias clases
~~~
class Empleado(Persona):                       => herencia de una clase
    def __init__(self,nombre,apellido,sueldo):   |
        super().__init__(nombre,apellido)         > se inicializa la nueva variable y con super las 
        self.sueldo = sueldo                     | variables del "padre"
    
class ClaseHija(ClaseHerdada1, ClaseHeredada2): => herencia de varias clases
    def ____init__(self,): 
        ClaseHerdada1.__init__()       => se inicializa la nueva variable y con el nombre de la 
        ClaseHeredada2.__init__()         herencia las variables del "padre"
~~~
## Clases Abstractas
Es una clase que no admite que se cren objetos a partir de ella. Es meramente de herencia
~~~
from abc import ABC,abstractmethod => importamos las funciones 

class ClaseAbstracta(ABC): => no se puede crear un objeto
    @abstractmethod         |
    def metodoAbstracto():   > metodo obligatorio para las clases hijas
        pass                |
~~~
## Funciones       

**variables de lectura (get)**
```
@property          
    def nombre1(self):              
        return self._nombre1
```        
**variable modificable (set)**
```
@nombre.setter                 
def nombre(self,nombre):        
    self._nombre1 = nombre      
```
**elimina el objeto despues de reproducir el codigo**
```
def __del__(self):              
    codigo                       
```
**cambia la declaracion del objeto de objeto a "codigo"**
```
def __str__(self):              
    codigo                       
```
**Metodos Estaticas**
```
@staticmethod
def metodoEstatico():
    codigo              
```
no puede acceder fuera del contexto

<br>

**Metodos dinamicos de clase**
```         
@classmethod            
def metodoDeClase(cls):   
    codigo              
```
se puede accesder a esta variable fuera del contexto


**crea objeto con la clase**<br>
`persona = Persona("nombre","apellido")`   

**llama al metodo de la clase** <br>
`persona.nombreDelMetodo()`     


**No se puede hacer** <br>
`persona._nombre1`                       

    
        

# Estructuras
## colecciones => 
| Tipo de lista|codear                  |funcion| | |
|:------------:|---|--------------------|---|---|    
|listas         |[]                     |ordenada y modificable
|tuplas         |()                     |ordenada y no se puede modificar
|set            |{}                     |desordenada y modificable (no admite valores duplicados)
|diccionario    |{key : definicion}     |tiene un valor y una definicion asiciada a el|
|clases         |class Clase:<br>pass   | una clase es lal base para la creacion de objeto
|objeto         |objeto = clase()       |es un variable con las propiedades de la clase


## decicion
```
if condicion:
    codigoTrue
elif condicion:
    codigoTrue
else:
    codigoFalse
```
```
codigoTrue if condicion else codigoFalse
```

## ciclo
```
while condicion:
    codigoTrue
else:
    codigoFalse
```
```
for variable in struct:
    codigoTrue
else:
    codigoFalse
```
```
breack => sale del ciclo
continue => saltea codigo seleccionado
range(valor)   => imprime un rango segun el valor colocado
```
## funciones
```
def nombreDeLaFuncion(variable,varible2): -> returnTipoDeVariable:
    codigo
    return => lo que retorna la funcion
        
def nombreDeLaFuncion(*variablesN):  => si no se sabe la cantidad de parametros a tomar
def nombreDeLaFuncion(**terminos):   => si queremos que los elementos sean un diccionario
```

## import
`from Persona import Persona` => para importart solo una clase <br>
`from Persona import *`       => para importar todas las clases del archivo <br>
`from archivo impor objeto as nombre` => importa un objeto y se le hace referencia con el nombre dad

### pruebas en archivos
```
if __name__ == "__main__":
    pruebas             => esto no se va a importar
```
# DEFINICIONES IMPORTANTES  
## clases
    get => trae elementos fijos de clases sin romper encapsulamiento
    set => modifica elementos fijos de clases sin romper encapsulamiento
    read-only => variables que solo tienen get y no ser

## variables
    estaticas = estan atadas al contexto
    dinamicas = pueden modificarse fuera del contexto

## constante
se escribe en mayusculas y se separan las palabras por _ ejemplo: <br>
`MI_CONSTANTE`<br>
las cosntantes **no** se tiene que modificar

# Sobrecarga de operadores
## Que es?
Se le dice a una funcion que actua distinto segun el argumento que se le ingresa como el signo de + que segun que argumentos se les pasa cumple diferentes funciones como la de sumar concatenar etc
## Como funciona
para sobrecargar un atributo en una classe se la tiene que sobrescribir. en la siguiente tabla se visualiza como sobrescribir algunos operadore:

|Operador|        methodo            ||||
|:------:|-------|-----|-----|----------|
| +     | `__add__(self,other)`         |
| -     | `__sub__(self,other)`         |
| *     | `__mul__(self,other)`         |
| /     | `__truediv__(self,other)`     |
| //    | `__floordiv__(self,other)`    |
| %     | `__mod__(self,other)`         |
| **    | `__pow__(self,other)`         |
| <     | `__it__(self,other)`          |
| >     | `__gt__(self,other)`          |
| <=    | `__le__(self,other)`          |
| >=    | `__ge__(self,other)`          |
| ==    | `__eq__(self,other)`          |
| !=    | `__ne__(self,other)`          |
| -=    | `__isub__(self, other)`       |
| +=    | `__iadd__(self, other)`       |
| *=    | `__imul__(self, other)`       |
| /=    | `__idiv__(self, other)`       |
| //=   | `__ifloordiv__(self, other)`  |
| %=    | `__imod__(self, other)`       |
| **=   | `__ipow__(self, other)`       |

# Polimorfismo
## Que es?
Es la ejecucion de varios metodos en tiempo de ejecucion
## algunos metodos

|metodo|accion||||
|:------:|-------|-----|-----|----------|
| `isintance(objeto,clase)`| si el objeto seleccionado pertenece a sierta clase|
||
