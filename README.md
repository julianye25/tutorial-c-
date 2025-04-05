# Algoritmos

## Índice

1. [Introducción](#introducción)
2. [Características principales de un algoritmo](#características-principales-de-un-algoritmo)
3. [Ejemplo de un algoritmo simple](#ejemplo-de-un-algoritmo-simple)
4. [Tipos de datos primitivos](#tipos-de-datos-primitivos)
5. [Variables](#variables)
6. [Var](#uso-de-la-palabra-reservada-var)
7. [Constantes](#uso-de-constantes)
8. [Operadores Aritmeticas](#operadores-aritméticos)
9. [Operadores Logicos](#operadores-lógicos)
10. [Operadores relacionalles](#operadores-relacionales)
11. [Strings](#strings-en-c#)
12. [Condicional If](#condicional-if)

---

## Introducción

Un algoritmo es un conjunto de pasos o instrucciones definidos, ordenados y finitos que se utilizan para resolver un problema o realizar una tarea específica. Los algoritmos son fundamentales en la programación, ya que permiten estructurar soluciones de manera lógica y eficiente.

## Características principales de un algoritmo

1. **Definido**: Cada paso debe estar claramente especificado.
2. **Ordenado**: Los pasos deben seguir una secuencia lógica.
3. **Finito**: Debe tener un número limitado de pasos y terminar en algún momento.
4. **Entrada**: Puede requerir datos de entrada.
5. **Salida**: Produce uno o más resultados.

## Ejemplo de un algoritmo simple

1. Leer dos números.
2. Sumar los números.
3. Mostrar el resultado.

Los algoritmos pueden implementarse en cualquier lenguaje de programación para resolver problemas específicos.

## Tipos de datos primitivos

En C#, los **tipos de datos primitivos** son fundamentales para declarar variables y trabajar con datos. A continuación, se describen los más comunes:

1. **Enteros (`int`)**: Representan números enteros, como `-10`, `0`, `42`.
2. **Punto flotante (`float`, `double`)**: Representan números con decimales, como `3.14`, `-0.001`.
   - `float`: Precisión simple (32 bits).
   - `double`: Precisión doble (64 bits).
3. **Caracteres (`char`)**: Representan un solo carácter, como `'a'`, `'1'`, `'$'`.
4. **Cadenas de texto (`string`)**: Representan secuencias de caracteres, como `"Hola"`, `"123"`.
5. **Booleanos (`bool`)**: Representan valores lógicos, como `true` o `false`.

### Ejemplo en C#

El siguiente código muestra cómo declarar y usar estos tipos de datos en C#:

```csharp
using System;

class Program
{
    static void Main()
    {
        int numero = 42;               // Entero
        float decimalCorto = 3.14f;    // Punto flotante (precisión simple)
        double decimalLargo = 2.71828; // Punto flotante (precisión doble)
        char letra = 'A';              // Carácter
        string texto = "Hola";         // Cadena de texto
        bool esVerdadero = true;       // Booleano

        Console.WriteLine($"Entero: {numero}");
        Console.WriteLine($"Float: {decimalCorto}");
        Console.WriteLine($"Double: {decimalLargo}");
        Console.WriteLine($"Carácter: {letra}");
        Console.WriteLine($"Texto: {texto}");
        Console.WriteLine($"Booleano: {esVerdadero}");
    }
}
```

## Variables

En C#, una **variable** es un espacio en memoria que se utiliza para almacenar datos. Cada variable tiene un tipo de dato que define qué tipo de información puede contener.

### Declaración de variables

Para declarar una variable en C#, se utiliza la siguiente sintaxis:

```csharp
tipo nombreVariable = valorInicial;
```

### Uso de la palabra reservada `var`

En C#, la palabra reservada `var` se utiliza para declarar variables de tipo implícito. Esto significa que el compilador deduce automáticamente el tipo de la variable en función del valor que se le asigna.

#### Ejemplo de uso

```csharp
using System;

class Program
{
    static void Main()
    {
        var numero = 42;               // El compilador infiere que es un int
        var texto = "Hola, mundo";     // El compilador infiere que es un string
        var esVerdadero = true;        // El compilador infiere que es un bool
        var decimalCorto = 3.14f;      // El compilador infiere que es un float

        Console.WriteLine($"Número: {numero}");
        Console.WriteLine($"Texto: {texto}");
        Console.WriteLine($"Booleano: {esVerdadero}");
        Console.WriteLine($"Float: {decimalCorto}");
    }
}
```

## Uso de constantes

En C#, una **constante** es un valor que no puede cambiar durante la ejecución del programa. Las constantes se declaran utilizando la palabra clave `const` y deben ser inicializadas en el momento de su declaración.

### Declaración de constantes

La sintaxis para declarar una constante es la siguiente:

```csharp
const tipo nombreConstante = valor;
```

### Ejemplo de uso

```csharp
using System;

class Program
{
    static void Main()
    {
        const double Pi = 3.14159;      // Constante de tipo double
        const int DiasEnUnaSemana = 7; // Constante de tipo int

        Console.WriteLine($"El valor de Pi es: {Pi}");
        Console.WriteLine($"Una semana tiene {DiasEnUnaSemana} días.");
    }
}
```

En este ejemplo, las constantes `Pi` y `DiasEnUnaSemana` no pueden cambiar su valor durante la ejecución del programa.

## Operadores aritméticos

En C#, los **operadores aritméticos** se utilizan para realizar operaciones matemáticas básicas. A continuación, se describen los operadores más comunes:

| Operador | Descripción      | Ejemplo |
| -------- | ---------------- | ------- |
| `+`      | Suma             | `a + b` |
| `-`      | Resta            | `a - b` |
| `*`      | Multiplicación   | `a * b` |
| `/`      | División         | `a / b` |
| `%`      | Módulo (residuo) | `a % b` |

### Ejemplo en C#

El siguiente código muestra cómo usar los operadores aritméticos en C#:

```csharp
using System;

class Program
{
    static void Main()
    {
        int a = 10;
        int b = 3;

        Console.WriteLine($"Suma: {a} + {b} = {a + b}");
        Console.WriteLine($"Resta: {a} - {b} = {a - b}");
        Console.WriteLine($"Multiplicación: {a} * {b} = {a * b}");
        Console.WriteLine($"División: {a} / {b} = {a / b}");
        Console.WriteLine($"Módulo: {a} % {b} = {a % b}");
    }
}
```

En este ejemplo, se realizan operaciones básicas con dos números enteros, mostrando los resultados en la consola.

## Operadores lógicos

En C#, los **operadores lógicos** se utilizan para realizar operaciones booleanas, combinando o evaluando expresiones lógicas. A continuación, se describen los operadores más comunes:

| Operador | Descripción           | Ejemplo  |
| -------- | --------------------- | -------- | ------------- | --- | --- | --- |
| `&&`     | AND lógico (y)        | `a && b` |
| `        |                       | `        | OR lógico (o) | `a  |     | b`  |
| `!`      | NOT lógico (negación) | `!a`     |

### Ejemplo en C#

El siguiente código muestra cómo usar los operadores lógicos en C#:

```csharp
using System;

class Program
{
    static void Main()
    {
        bool a = true;
        bool b = false;

        Console.WriteLine($"a AND b: {a && b}");  // AND lógico
        Console.WriteLine($"a OR b: {a || b}");   // OR lógico
        Console.WriteLine($"NOT a: {!a}");        // NOT lógico
    }
}
```

En este ejemplo, se evalúan combinaciones de valores booleanos utilizando los operadores lógicos, mostrando los resultados en la consola.

## Operadores relacionales

En C#, los **operadores relacionales** se utilizan para comparar dos valores y devolver un resultado booleano (`true` o `false`). A continuación, se describen los operadores más comunes:

| Operador | Descripción       | Ejemplo  |
| -------- | ----------------- | -------- |
| `==`     | Igual a           | `a == b` |
| `!=`     | Distinto de       | `a != b` |
| `>`      | Mayor que         | `a > b`  |
| `<`      | Menor que         | `a < b`  |
| `>=`     | Mayor o igual que | `a >= b` |
| `<=`     | Menor o igual que | `a <= b` |

### Ejemplo en C#

El siguiente código muestra cómo usar los operadores relacionales en C#:

```csharp
using System;

class Program
{
    static void Main()
    {
        int a = 10;
        int b = 5;

        Console.WriteLine($"a == b: {a == b}");  // Igual a
        Console.WriteLine($"a != b: {a != b}");  // Distinto de
        Console.WriteLine($"a > b: {a > b}");    // Mayor que
        Console.WriteLine($"a < b: {a < b}");    // Menor que
        Console.WriteLine($"a >= b: {a >= b}");  // Mayor o igual que
        Console.WriteLine($"a <= b: {a <= b}");  // Menor o igual que
    }
}
```

En este ejemplo, se comparan dos números enteros utilizando los operadores relacionales, mostrando los resultados en la consola.

## Strings en C#

En C#, una **string** es una secuencia de caracteres que se utiliza para representar texto. Las cadenas de texto son inmutables, lo que significa que no se pueden cambiar después de ser creadas. Sin embargo, se pueden manipular utilizando diversos métodos y propiedades.

### Declaración de strings

Las cadenas de texto se declaran utilizando el tipo `string` y se delimitan con comillas dobles (`"`):

```csharp
string saludo = "Hola, mundo";
```

### Operaciones comunes con strings

1. **Concatenación**: Combinar dos o más cadenas.

   ```csharp
   string nombre = "Juan";
   string mensaje = "Hola, " + nombre + "!";
   Console.WriteLine(mensaje); // Salida: Hola, Juan!
   ```

2. **Interpolación de cadenas**: Insertar valores dentro de una cadena utilizando `$`.

   ```csharp
   string nombre = "Ana";
   int edad = 25;
   string mensaje = $"Mi nombre es {nombre} y tengo {edad} años.";
   Console.WriteLine(mensaje); // Salida: Mi nombre es Ana y tengo 25 años.
   ```

3. **Longitud de una cadena**: Obtener el número de caracteres con la propiedad `Length`.

   ```csharp
   string texto = "C# es genial";
   Console.WriteLine($"La longitud del texto es: {texto.Length}");
   ```

4. **Métodos comunes**:

   - `ToUpper()`: Convierte la cadena a mayúsculas.
   - `ToLower()`: Convierte la cadena a minúsculas.
   - `Trim()`: Elimina espacios en blanco al inicio y al final.
   - `Substring()`: Extrae una parte de la cadena.
   - `Contains()`: Verifica si una cadena contiene otra.

   ```csharp
   string texto = "  Hola, C#!  ";
   Console.WriteLine(texto.ToUpper());   // Salida: "  HOLA, C#!  "
   Console.WriteLine(texto.ToLower());   // Salida: "  hola, c#!  "
   Console.WriteLine(texto.Trim());      // Salida: "Hola, C#!"
   Console.WriteLine(texto.Contains("C#")); // Salida: True
   Console.WriteLine(texto.Substring(2, 4)); // Salida: "Hola"
   ```

5. **Comparación de cadenas**:

   - `Equals()`: Compara dos cadenas para verificar si son iguales.
   - `Compare()`: Compara dos cadenas y devuelve un valor indicando su orden.

   ```csharp
   string cadena1 = "Hola";
   string cadena2 = "hola";

   Console.WriteLine(cadena1.Equals(cadena2)); // Salida: False
   Console.WriteLine(string.Compare(cadena1, cadena2, true)); // Salida: 0 (ignora mayúsculas/minúsculas)
   ```

### Ejemplo completo

```csharp
using System;

class Program
{
     static void Main()
     {
          string nombre = "Carlos";
          string saludo = "Hola";
          string mensaje = $"{saludo}, {nombre}! Bienvenido a C#.";

          Console.WriteLine(mensaje); // Salida: Hola, Carlos! Bienvenido a C#.
          Console.WriteLine($"Longitud del mensaje: {mensaje.Length}");
          Console.WriteLine($"En mayúsculas: {mensaje.ToUpper()}");
          Console.WriteLine($"Contiene 'C#': {mensaje.Contains("C#")}");
     }
}
```

En este ejemplo, se demuestra cómo trabajar con cadenas en C#, utilizando concatenación, interpolación y métodos comunes.

## Condicional `if`

En C#, la estructura condicional `if` se utiliza para ejecutar un bloque de código solo si una condición específica se evalúa como `true`. Es una de las estructuras de control más comunes en la programación.

### Sintaxis básica

```csharp
if (condición)
{
    // Código a ejecutar si la condición es verdadera
}
```

### Ejemplo simple

```csharp
using System;

class Program
{
    static void Main()
    {
        int numero = 10;

        if (numero > 5)
        {
            Console.WriteLine("El número es mayor que 5.");
        }
    }
}
```

En este ejemplo, el mensaje se mostrará en la consola porque la condición `numero > 5` es verdadera.

### Uso de `if-else`

La estructura `if-else` permite ejecutar un bloque de código si la condición es `true` y otro bloque si es `false`.

```csharp
if (condición)
{
    // Código a ejecutar si la condición es verdadera
}
else
{
    // Código a ejecutar si la condición es falsa
}
```

#### Ejemplo

```csharp
using System;

class Program
{
    static void Main()
    {
        int numero = 3;

        if (numero > 5)
        {
            Console.WriteLine("El número es mayor que 5.");
        }
        else
        {
            Console.WriteLine("El número no es mayor que 5.");
        }
    }
}
```

### Uso de `if-else if-else`

Cuando hay múltiples condiciones, se puede usar `else if` para evaluar varias posibilidades.

```csharp
if (condición1)
{
    // Código a ejecutar si condición1 es verdadera
}
else if (condición2)
{
    // Código a ejecutar si condición2 es verdadera
}
else
{
    // Código a ejecutar si ninguna condición es verdadera
}
```

#### Ejemplo

```csharp
using System;

class Program
{
    static void Main()
    {
        int numero = 0;

        if (numero > 0)
        {
            Console.WriteLine("El número es positivo.");
        }
        else if (numero < 0)
        {
            Console.WriteLine("El número es negativo.");
        }
        else
        {
            Console.WriteLine("El número es cero.");
        }
    }
}
```

### Notas importantes

- Las condiciones dentro de un `if` deben evaluarse a un valor booleano (`true` o `false`).
- Se pueden combinar múltiples condiciones utilizando operadores lógicos como `&&` (AND) y `||` (OR).

#### Ejemplo con operadores lógicos

```csharp
using System;

class Program
{
    static void Main()
    {
        int edad = 20;

        if (edad >= 18 && edad <= 65)
        {
            Console.WriteLine("La persona está en edad laboral.");
        }
        else
        {
            Console.WriteLine("La persona no está en edad laboral.");
        }
    }
}
```

En este ejemplo, se verifica si la edad está dentro del rango de 18 a 65 años utilizando el operador lógico `&&`.
