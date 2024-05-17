# leguaje de programacion C|
# Estructuras
<<<<<<< HEAD
```c
#include <stdio.h>
#include <stdlib.h>

#define max(a,b)  ((a) > (b) ? a : b)

void main(arvc, arvb){

        fprinrf()
}
```
## definicion de variables 

# Librerias
```c
#include <stdio.h>
```

| Funcion | Utilidad | variables | ejemplo |
|:---------:|:----------:|:------------:|:-----|
|`printf(texto,...variables)`|Muestra el texto con las variables en pantalla | texto: texto plano con %A que permite dictar el tipo de varibales ...variables: x cantidad de variables en el orden declarado en el texto | `printf("hola mundo %d", a)` -> muestra el hola mundo con la a como numerico|
|`scanf(texto,variable) ` | se le pide al usuario algo| texto : texto plano que ve el usuario variable: valor donde se va a alamacenar la variable | `scanf("ingrese valor %d",&a)` se envia la informacion del puntero a la variable a en formato entero|
=======
## Estrcutura basica
```C
#include <stdio.h>
#include <stdlio.h>

int main(int argc, char *argv[]){

    return 0;
}
```
## Definicion de macros
### ¿Que es?
Es una variable que se remplaza en todo el codigo, puede ser desde una costante hasta una funcion.
### Como se utiliza
Se agrega un #define para definir que es un macro al costado el nombre del macro y luego su utiliza <br>
```c
#define cargaMaxima 50000 // ejemplo de una macro constante
#define suma(a,b) a+b // ejemplo macro funcion
```
## Comandos utiles
|comando | utilidad |
|--------|----------|
|gcc -E codigo.c -o salida | Se utiliza para la pre compilacion
|gcc -S codigo.c  | Ejecuta el codigo a nivel sintactico

>>>>>>> abafb164bda442ffd11a87dcc79f695517289a3b
