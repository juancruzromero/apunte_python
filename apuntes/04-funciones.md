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

## Alcance de las funciones