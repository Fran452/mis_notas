# leguaje de programacion C
# Estructuras
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

