# Algoritmos

## Índice

1. [Introducción](#introducción)
2. [Características principales de un algoritmo](#características-principales-de-un-algoritmo)
3. [Ejemplo de un algoritmo simple](#ejemplo-de-un-algoritmo-simple)
4. [Tipos de datos primitivos](#tipos-de-datos-primitivos)
5. [Variables](#variables)

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
