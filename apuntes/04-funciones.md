# Funciones

Una función es un bloque de código con un nombre asociado, que recibe cero o más argumentos como entrada, sigue una secuencia de sentencias, la cuales ejecuta una operación deseada y devuelve un valor y/o realiza una tarea, este bloque puede ser llamados cuando se necesite.

El uso de funciones es un componente muy importante del paradigma de la programación llamada estructurada, y tiene varias ventajas:

modularización: permite segmentar un programa complejo en una serie de partes o módulos más simples, facilitando así la programación y el depurado.
reutilización: permite reutilizar una misma función en distintos programas.

Python dispone de una serie de funciones integradas al lenguaje, y también permite crear funciones definidas por el usuario para ser usadas en su propios programas.

## Sentencia def
La sentencia **“def”** es una definición de función usada para crear objetos funciones definidas por el usuario.

Una definición de función es una sentencia ejecutable. Su ejecución enlaza el nombre de la función en el namespace local actual a un objeto función (un envoltorio alrededor del código ejecutable para la función). Este objeto función contiene una referencia al namespace local global como el namespace global para ser usado cuando la función es llamada.

La definición de función no ejecuta el cuerpo de la función; esto es ejecutado solamente cuando la función es llamada.

La sintaxis para una definición de función en Python es:

```python
def suma(num1, num2):
    return num1 + num2
```

## Parámetros de función
Puedo agregar parámetros a las funciones, por ejemplo num1 y num2:
```python
def suma(num1, num2):
    return num1 + num2
```

## Args Keyword
**Args:**  Puedo meter un montón de parámetros.

**Keywords:** Puedo utilizar esto para setear valores que espera una función. Es común en módulos de python.

Se explica muy bien aquí, pero está en ingles: https://realpython.com/python-kwargs-and-args/

## Closures
Llamamos “Closures” cuando una función genera dinámicamente otra función y que esta nueva función pueda acceder a las variables locales, aún cuando la primera haya finalizado.

Me encanta como se explica aquí: https://www.geeksforgeeks.org/python-closures/

## Funciones anidadas
Funciones anidadas a otras jaja. Platzi lo explica re bien en este post: https://platzi.com/tutoriales/1775-poo-python/9926-funciones-anidadas-y-como-objetos-de-primera-clase/

## Factorial de un número con recursión

Una función está siendo recursiva cuando dentro del bloque de instrucciones que la conforma se usa a sí misma.

El concepto puede sonar complicado pero es muy común su uso, por ejemplo cuando haces el calculo del factorial de un número lo haces con una función recursiva.

El factorial de un número es el número multiplicado por los números antes del, por ejemplo: **5! es 5\*4\*3\*2\*1**

Esto se puede expresar como:

```python
5*fac(4)
4*fac(3)
3*fac(2)
2*fac(1)
1*fac(0)
```

**Nota importante:** Cuando estés trabajando con recursividad siempre debes pensar en el caso base, es decir debes definir el momento en el que la función dejará de llamarse a sí misma, para que no hagas un loop infinito, por ejemplo en el caso del factorial terminas la ejecución cuando llegas a cero.

## Funciones() importantes en Python

- isinstance()
- filter()
- map()

## Funciones Lambda

freeCodeCamp lo explica genial: https://www.freecodecamp.org/espanol/news/expresiones-lambda-en-python/