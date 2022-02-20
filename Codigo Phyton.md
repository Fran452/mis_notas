# varios 
    - print("texto") => muestra en cosola el texto
    - inputo("texto) => muestra por consola el texto y espera resibir un valor
    - id(variable)   => ubicacion de memoria de la variable
    - int(variable)  => combierte la variable en int
    - float(variable) => combierte la variable en float
    - type(variable)  => el tipo de la variable
    - # => comentario
    - __name__ => muestra la ubicacion de donde se utiliza el codigo
    del variable => elimina el objeto

# funciones para listas
    len(lista) => cantidad de elementos dentro de la lista
    lista[valorInicial : valorFinal] => toma los valores entre el valorInicial y el valorFinal sin incluirlos
    lista.append(valor) => agrega un elemento al final de la lista
    lista.insert(indice,valor) => agrega un elemento en un indice especifico de la lista
    lista.romeve(valor) => remueve el valor de la lista
    lista.pop() => elimina el ultimo valor de la lista
    del lista[indice] => elimina un elemento de la lista por indice
    lista.clear() => elimina todos los valores de la lista
    list(tupla)   => convierte la tupla en una lista
    tuple(lista)  => convierte la lista en tupla

# funciones para set
    len(set) => cantidad de elementos
    valor in set => si el valor esta en el set 
    set.add(valor) => agrega valor en el set
    set.remove(valor) => elimina valor del sat 
    set.discard(valor) => elimina valor del set (de no estar no arroja error)
    set.clear() => elimina todos los valores dentro de set
    del set => elimina el set

# funciones para diccionarios
    len(dicc) => tamaño de diccionario
    dicc[key] => acceder a la definicion de la key
    dicc.get(key) => acceder a la definicion de la key
    for key,definicion in dicc.items()  => recorre un diccionario con las llaves y las definiciones
    for key,definicion in dicc.key()    => recorre un diccionario con las llaves
    for key,definicion in dicc.values() => recorre un diccionario con  las definiciones 
    key in dicc => si la key esta en el diccionario
    dicc["nueva llave"] = "nueva definicion => agrega un nuevo elemento al diccionario
    dicc.pop(key) => elimina un elemento del diccionario
    dicc.clear() => elimina todos los valores del diccionario
    del dicc => elimina el diccionario

# funcion y estructuras de la clase
## Tipo de clases
        class Persona
            def __init__(self,nombre,apellido):         |
                self.nombre =  nombre                   > contructor de clase
                self.apellido =  apellido               |
                self._nombre1 = nombre                   => variable la cual no se puede modificar

            def nombreDelMetodo(self):                      |
                metodo                                       > creacion de metodos en clase

## Clase hijas
        class Empleado(Persona):                       => herencia de una clase
            def __init__(self,nombre,apellido,sueldo): |
            super().__init__(nombre,apellido)           > se inicializa la nueva variable y con super las variables del "padre"
            self.sueldo = sueldo                       |
    
        class ClaseHija(ClaseHerdada1, ClaseHeredada2): => herencia de varias clases
            def ____init__(self,): 
                ClaseHerdada1.__init__()       => se inicializa la nueva variable y con el nombre de la herencia las variables del "padre"
                ClaseHeredada2.__init__() 

## Clases Abstractas
        from abc import ABC,abstractmethod => importamos las funciones 

        class ClaseAbstracta(ABC): => no se puede crear un objeto
            @abstractmethod         |
            def metodoAbstracto():   > metodo obligatorio para las clases hijas
                pass                |

## Funciones          
            @property                      |
            def nombre1(self):              > variables de lectura (get)
                return self._nombre1       |
            
            @nombre.setter                  |
            def nombre(self,nombre):         > variable modificable (set)
                self._nombre1 = nombre      |

            def __del__(self):              |
                codigo                       > elimina el objeto despues de reproducir el codigo

            def __str__(self):              |
                codigo                       > cambia la declaracion del objeto de objeto a "codigo"

            @staticmethod
            def metodoEstatico():   => no puede acceder a las variables dinamicas
                codigo              
            
            @classmethod            |
            def metodoDeClase(cls):  > se puede accesder a las variables dinamicas
                codigo              |

            persona = Persona("nombre","apellido")      => crea objeto con la clase
            persona.nombreDelMetodo()                   => llama al metodo de la clase
            persona._nombre1                            => no se puede hacer 

    
        

# Estructuras
## colecciones => 
        listas = [] => ordenada y modificable
        tuplas = () => ordenada y no se puede modificar
        set    = {} => desordenada y modificable (no admite valores duplicados)
        diccionario = {key : definicion} => tiene un valor y una definicion asiciada a el
        class Clase  |
            pass      > creacion de clases
        objeto = Objeto() => declaracion de objeto

## decicion =>
        if condicion:
            codigoTrue
        elif condicion:
            codigoTrue
        else:
            codigoFalse

        codigoTrue if condicion else codigoFalse

## ciclo => 
        while condicion:
            codigoTrue
        else:
            codigoFalse
      --------------------------
        for variable in struct:
            codigoTrue
        else:
            codigoFalse
      ---------------------------
      breack => sale del ciclo
      continue => saltea codigo seleccionado
      range(valor)   => imprime un rango segun el valor colocado

## funciones
        def nombreDeLaFuncion(variable,varible2): -> returnTipoDeVariable:
            codigo
            return => lo que retorna la funcion
        
        def nombreDeLaFuncion(*variablesN):  => si no se sabe la cantidad de parametros a tomar
        def nombreDeLaFuncion(**terminos):   => si queremos que los elementos sean un diccionario

## import
        from Persona import Persona => para importart solo una clase
        from Persona import *       => para importar todas las clases del archivo

## #pruebas en archivos

        if __name__ == "__main__":
            pruebas             => esto no se va a importar

# DEFINICIONES IMPORTANTES  
## clases
        get => trae elementos fijos de clases sin romper encapsulamiento
        set => modifica elementos fijos de clases sin romper encapsulamiento
        read-only => variables que solo tienen get y no ser