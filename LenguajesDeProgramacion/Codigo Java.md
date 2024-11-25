<div id = "Indice"> <!----- Inicio de Indice ------->

# Indice

1. 
| [Titulo](#titulo) |
|:-------------------------:|
|[Subtitulo](#titulo-subtitulo)|
|[Subtitulo](#titulo-subtitulo)|
|[Subtitulo](#titulo-subtitulo)|
|[Subtitulo](#titulo-subtitulo)|


</div> <!----- Fin de indice ------->

# Estructura basica de un programa 
```java
public class NombreClase {
    public static void main (String [] args) {
    // comandos
    }
}
```
# Expreciones aritmeticas 
- Suma (+)
- Resta (-)
- Multiplicacion (*)
- Divicion (/)
  - Entera: Si los valores a dividir son enteros (4/8)
  - Fraciones: Si los valores a dividir son no enteros (4.0/5.5)
- Resto de la divicion (%)
  - Entera: Si los valores a dividir son enteros (4/8)
  - Fracciones Si los valores a dividir son no enteros (4.0/5.5)

# Variables
## Tipos de variables 
- Variables primitivas (int, short, byte, long, boolean, float, double): son las mas basicas y las cuales se compone todo el programa
- Variables referenciada a objetos (string, arreglos, etc): son un conjunto de primitivas 
## Variables primitivas
| tipo  |representacion|tamaño (en bits) |valor por defecto|
|:----: |--------------|-----------------|-----------------|
|boolean|True o False  |   1             | false           |  
| char  |caracter unico|    16           |\u0000           |
|byte   |entero con signo |8|0
|short|entero con signo|16|0
|int|entero con signo|32|0
|long|entero con signo|64|0
|float|coma flotante de precision simple Norma IEEE754|32|0.0
|doble|coma flotante de precision doble Norma IEEE754|64|0.0

## CHAR relevantes
| char  | funcion |
|:----: |--------------|
|`/n`   | Salto de linea |
|`/b`   | Retroceso |
|`/t`   | Tabulado |
|`/r`   | Principio de linea |
|`/f`   | Nueva pagina |

## Numericos en diferente formato

| Funcion  | tipo nuerico |
|:----: |--------------|
|`Integer.toBinaryString(numero)`   | Binario |
|`Integer.toHexString(numero)`   | Hexadecimal |
|`Integer.toOctalString(numero)`   | Octal |


## Convertir datos

```java
// De string a bool
Boolean.parseBoolean(string);
// De bool a string
Boolean.toString(string);

// De string a double
Double.parseDouble(string);
// De double a string
Double.toString(string);

// De string a int
Integer.parseInt(string);
// De int a string
Integer.toString(string);

// De string a float
Float.parseFloat(string);
// De float a string
Float.toString(string);
```



# Casting de tipos
## Orden de proioridad 
byte < short < char < int < long < float < double
## Declaracion de variables de menor grado
Si se quiere declar una varibale de mayor grado a una variable de menor grado o si se decea asignar un tipo especifico con espesificar despues de la asignacion el tipo java lo tranforma como se ven en el ejemplo

```java
int entero = (int) -2.03;
// se trunca -2.03 a -2
char letraC = (char) 67;
/* se asigna la letra C
cuyo codigo ASCII es 67 */
```

## Ejemplo
```java
double frac = 1 + 2.03;
// 1 puede usarse como 1.0
int entero = ’c’;
// se asigna el codigo ASCII 99
```
# Asignacion
## Asignacion simple
Es cuando se le asigna a una variable de forma normal:
```java
int valor = 2
```
## Asignacion por variable
Es cuando se le asigna a una variable y se le asigna un valor para adaptarlo a esa variable:
```java
int valor = (int) 2,3
// valor = 2
```
## Asignacion compuesta
Asignacion basda en cuentas:
```java
x += expr; // x = x + expr
x -= expr; // x = x - expr
x *= expr; // x = x * expr
x /= expr; // x = x / expr
x %= expr; // x = x % expr
```
## Asignacion unitaria
Asignacion basda en cuentas binearias (+-1):
```java
x++; // x = x + 1 si se asigna primero se asigna x y despues se suma
++x; // x = x + 1 si se asigna primero se suma y despues se asigna
x--; // x = x - 1 si se asigna primero se asigna y despues se resta
--x; // x = x - 1 si se asigna primero se resta  y despues se asigna
```
# Entrada y salida de datos
## Entrada
```java
import java.util.Scanner;
public class Echo {
    public static void main(String[] args) {
        /*inicializa el ingreso de datos
        por teclado */
        Scanner input = new Scanner (System.in);
        // espera el ingreso de un valor
        int numero = input.nextInt();
        // muestra el valor ingresado
        System.out.println(numero);
        input.close();
    }
}
```
## Salida
usando System.out.println(salida); se saca valores por consola siendo "salida" un string 
```java
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        String salida = "hola mundo" 
        System.out.println(salida);
        // hola mundo
    }
}
```

# Estructuras control
Estas estructueras se usan para evaluar y segun lo evaluado ejecutan una u otra cosa
## if else
En el caso que el codigo sea de una linea:
```java
if(bool)
    codigo
else
    codigo en caso que bool sea negativo
```

En el caso que el codigo sea de mas de una linea:
```java
if(bool){
    codigo
}else{
    codigo en caso que bool sea negativo
}
```
## swich
Se utiliza principal mente para menues ya que evalua uno por uno hasta que encuentra el valor 
```java
switch(expresion) {
    case val1:
    // bloque
    break;
    case val2:
    // bloque
    break;
    ...
    default:
    // bloque
    break;
}

```
## Operadores booleanos
| operador                  |significado|
|:-------------------------:|---|
|` `    | or (los palitos)
|` `    | or (en cortocircuitos => al primer true deja de evaluar) (doble palitos)
|`&`    | and
|`&&`   | and (en cortocircuitos => al primer false deja de evaluar)
|`^`    | XOR
|`!`    | not
|`==`   | Igual
|`!=`   | Distinto

# Estructuras repeticion
## while
Primero evalua y despues ingresa al bucle
```java
while (bool){
    // bloque
}
```
## do-while
Primero ingresa al bucle y luego evalua
```java
do{
    // bloque
}while(bool);
```
## for
se utiliza cuando ya se sabe la cantidad de veces que va a repetirce el ciclo
```java
for (inicializacion; cond; actualizacion){
    // bloque
}
```

# Funciones
## Estrucura basica
```java
public Tipobariable nombreFuncion(){
    return variable;
}
```
## Funciones Absatractas
Son funciones que tiene las clases abstractas para mantener la estructura de la funcion en las clases heredadas pero si una funcion predefinida
```java
abstract double montoDisponible(); // las clases que heredan de esta clase tiene que definir esta funcion
```

# Clases
## Estrucura basica

```java

public class Clase {
    private int variableA;  // Variable privada
    public  int variableB;  // Variable publica

    public Clase(int ingresoVariableA, int ingresoVariableB ){ // Contructor con variables
        variableA = ingresoVariableA;
        variableB = ingresoVariableB;
    }

    public Clase( ){ // Contructor sin variables

    }
    
    public int getvariableA () { // mostrar variable privada
        return variableA;
    }
}

```
## Como crear un objeto de una clase
1) se debe importar la clase que se busque usar
2) llamar a la clase como variable Clase y luego new Clase
```java
public class main {
	public static void main (String [] args) {
		Clase punto2 = new Clase(); // Se crea un objeto basado en una clase
	}
}
```
## Overloading
### Que es?
Es la capacidad de definir varios métodos con el mismo nombre
### Ejemplo
La clase contructora esta sobrecargada ya que permite el no ingreso de datos el ingreso de saldo inicial y el ingreso tanto del saldo inicial como de apertura.
```java
public class Cuenta {
    private double saldo = 0;
    private LocalDate apertura;

    public Cuenta () {
        apertura = LocalDate.now();
    }

    public Cuenta (double saldoInicial) {
        saldo = saldoInicial;
    }

    public Cuenta (double saldoInicial,LocalDate fechaApertura) {
        saldo = saldoInicial;
        apertura = fechaApertura;
    }
}
```
## This
### ¿Que es?
Referencia siempre al receptor de un mensaje
### Ejemplo
```java
public class Cuenta {
    private double saldo = 0;
    private LocalDate apertura;

    public double getSaldo () {
        return this.saldo; // hace referencia a la varibale saldo de la clase
    }
}
```
## Clases Wrappers
Permiten usar tipos primitivos como objetos, cada tipo tiene su wrapper (su clase)
| Tipo primitivo |  Wrappers  |
|:--------------:|------------|
|byte            | Byte       |       
|short           | Short      |          
|int             | Integer    |          
|long            | Long       |       
|float           | Float      |          
|double          | Double     |          
|boolena         | Boolena    |          
|char            | CHaracter  |              

## Cast de tipos


## Herencias 
### Que es?
Cuando una clase comparte estructura de otra clase para no repetir codigo se puede usar la herencia. Las clases heredadas no heredan el contructor.
#### Ejemplo

```java
public class ClasePadre {
    private String nombre;

    public ClasePadre(String nombreing){
        nombre = nombreing;
    }
}

public class ClaseHija extends ClasePadre{

    public ClaseHija(String nombreing){
        super(nombreing); // para guardar los datos que hereda de la clase padre
    }
}
```
### super
### Que es?
Se usa el super para mencionar funciones de la clase padre a la clase hija como en el en ejemplo. Usando el super 
no se puede acceeder a las variables privadas de la funcion padre solo a las publicas y a las protected

### Ejemplo
```java
public class ClasePadre {
    private String nombre;
    protected String nombre2;
    public ClasePadre(String nombreing){
        nombre = nombreing;
    }

    public String saludar(){
        return "hola " + nombre;
    }
}

public class ClaseHija extends ClasePadre{

    public ClaseHija(String nombreing){
        super(nombreing); // para guardar los datos que hereda de la clase padre
    }

    public String saludarMas(){
        return "hola " + super.saludar(); // el super.saludar() toma el retorno de la clase padre saludar 
    }
    // retunro nombre: pablo -> "hola hola pablo"

    public String saludarMas(){
        super.nombre // no existe ya que es privado
        super.nombre2 // si ya que es protected
    }
    
}
```
### redefinicion de funciones
En las clases hijas se pueden sobreescribir funciones de la clase padre

#### Ejemplo
Ahora saludar ya no es un simple hola nombre, sino que al sobre escrivirlo en la clase hijo es un hola hola nombre
```java
public class ClasePadre {
    private String nombre;

    public ClasePadre(String nombreing){
        nombre = nombreing;
    }

    public String saludar(){
        return "hola " + nombre;
    }
}

public class ClaseHija extends ClasePadre{

    public ClaseHija(String nombreing){
        super(nombreing); // para guardar los datos que hereda de la clase padre
    }

    public String saludar(){
        return "hola " + super.saludar();
    }
    // retunro nombre: pablo -> "hola hola pablo"
}
```

# Interfaces
## Que son
Una interfaz es una estructura que contiene:

- Métodos abstractos (sin cuerpo), que deben ser implementados por las clases que la usen.
- Constantes (static final por defecto).
- Desde Java 8, también puede incluir métodos predeterminados (default) y métodos estáticos (static).

## Sintaxis básica
```java
// Definición de una interfaz
public interface MiInterfaz {
    // Constante (implícitamente "public static final")
    int CONSTANTE = 100;

    // Método abstracto (implícitamente "public abstract")
    void metodoAbstracto();

    // Método con implementación predeterminada (Java 8+)
    default void metodoDefault() {
        System.out.println("Este es un método predeterminado en la interfaz.");
    }

    // Método estático (Java 8+)
    static void metodoEstatico() {
        System.out.println("Este es un método estático en la interfaz.");
    }
}
// Implementarla en clases:
// Clase que implementa la interfaz
public class MiClase implements MiInterfaz {

    @Override
    public void metodoAbstracto() {
        System.out.println("Implementación del método abstracto.");
    }
}

// Uso de la clase

public class Main {
    public static void main(String[] args) {
        MiClase obj = new MiClase();
        obj.metodoAbstracto(); // Llama al método implementado
        obj.metodoDefault();   // Llama al método predeterminado

        MiInterfaz.metodoEstatico(); // Llama al método estático directamente desde la interfaz
    }
}
```
## Comparación VS Clases Abstractas
- Interfaces: No pueden tener atributos de instancia (solo constantes) y permiten múltiples implementaciones.
- Clases abstractas: Pueden tener atributos, métodos con implementación, y solo una clase abstracta puede ser heredada por una clase concreta.

# Exepciones
## Que son??
Una excepción en Java es un evento que ocurre durante la ejecución de un programa y que interrumpe el flujo normal del
programa. Estas situaciones generalmente representan errores

## Sintaxis basica
### Manejo basico
```java
public class ManejoExcepciones {
    public static void main(String[] args) {
        try {
            int resultado = 10 / 0; // Provoca una ArithmeticException
            System.out.println("Resultado: " + resultado);
        } catch (ArithmeticException e) {
            System.out.println("Error: División entre cero.");
        } finally {
            System.out.println("Bloque finally siempre se ejecuta.");
        }
    }
}
```
### Manejo con clases
```java
// Crear la Clase que va a tener la exepcion
public class MontoInvalidoException extends Exception {
    public MontoInvalidoException(String mensaje) {
        super(mensaje);
    }
}

// Como aplicarla en la clase 
public class CuentaBancaria {
    private double saldo;

    public CuentaBancaria(double saldoInicial) {
        this.saldo = saldoInicial;
    }

    public void depositar(double monto) throws MontoInvalidoException { // con el throws y el nombre de la exepcion
        if (monto <= 0) {
            throw new MontoInvalidoException("El monto a depositar debe ser mayor que cero."); // throw new se crea la exepcio
        }
        saldo += monto;
    }
}
```
## Propagación de excepciones
Una excepción puede ser lanzada y manejada en otro nivel del programa usando la palabra clave throws.
```java
public class PropagacionExcepciones {
    public static void metodoA() throws Exception {
        throw new Exception("Excepción desde metodoA");
    }

    public static void metodoB() throws Exception {
        metodoA();
    }

    public static void main(String[] args) {
        try {
            metodoB();
        } catch (Exception e) {
            System.out.println("Excepción capturada: " + e.getMessage());
        }
    }
}
```


# Definiciones
## Polimorfismo 
Es la posibilidad de enviar mensajes sintácticamente iguales a objetos de distintos tipos