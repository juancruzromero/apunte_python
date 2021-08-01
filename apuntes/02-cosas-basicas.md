# Cosas básicas
## Tipos de Datos 
Es importante saber diferenciar los tipos de datos. No es lo mismo un **string** que un **integer**. El primero es cadena de texto, el segundo números que se pueden operar. Se definen por su contenido.

```python
# String
'Hola'

# Integer
1
2
3

# Float
1,0
2,1
3,2

# Bolean
True
False
```

## Operadores ##
- Aritméticos: +,-,*,/,%,**,//.
- Comparación: <,>,=,
- Lógicos:  and, or, not.
- Asignación: =, += , -=
- Especiales: is, is not, in, not in.

## Orden de operaciones ##
Todo un clásico en las redes sociales es que alguien comparta la operación 5+4/3-1*2 y que se monte un gallinero tremendo en los comentarios con distintas soluciones. Esto se debe a que mucha gente no tiene claro cómo va la jerarquía de las operaciones y el orden de evaluación de las mismas.

Si hablamos de operaciones básicas, y de la mayoría de lenguajes de programación (Javascript, PHP, Python, Ruby, C,Visual Basic, Java…), nos regiremos por el orden de operaciones conocido por el acrónimo inglés PEMDAS, que en castellano podríamos traducir como PAPOMUDAS (PAréntesis, POtencias, MUltiplicación, División, Adición, Sustracción). En base a esto el orden de operaciones en lenguajes de programación como Python, PHP, Ruby o Javascript sería:

- Paréntesis
- Potencias y radicales
- Multiplicación, división, división entera y módulo.
- Suma y resta.

## Variables y Constantes ##

En python, las variables se escriben en minúscula. Y las constantes en mayúscula.
Palabras Reservadas
Las palabras reservadas, como su nombre lo indican, son palabras las cuales el lenguaje de programación ya ha reservado para realizar ciertas tareas. No podemos declarar una variable con el mismo nombre que una palabra reservada

Si quieres conocer todas ellas, recomiendo el siguiente post: https://www.programiz.com/python-programming/keyword-list

## Métodos de cadenas ##

Existen varios métodos ofrecidos por python para manipular strings:
```python
name = "Juan Cruz"
print(name.capitalize())
print(name.upper())
```
Este post lo explica muy bien:
https://www.programaenpython.com/fundamentos/strings-en-python/

En la documentación oficial se encuentra aquí: https://docs.python.org/3.7/library/stdtypes.html#string-methods

## Scopes and namespaces ##

En Python, un name, también conocido como identifier, es simplemente una forma de otorgarle un nombre a un objeto. Mediante el nombre, podemos acceder al objeto. Vamos a ver un ejemplo:

```python
num = 5
id(num)
id(5)
```

En este caso, el identifier my_var es simplemente una forma de acceder a un objeto en memoria (en este caso el espacio identificado por el número 4561204416). Es importante recordar que un name puede referirse a cualquier tipo de objeto (aún las funciones).

```python
def echo(value):
    return value

a = echo
a = ("Juan")
```

Ahora que ya entendimos qué es un name podemos avanzar a los namespaces (espacios de nombres). Para ponerlo en palabras llanas, un namespace es simplemente un conjunto de names.

En Python, te puedes imaginar que existe una relación que liga a los nombres definidos con sus respectivos objetos (como un diccionario). Pueden coexistir varios namespaces en un momento dado, pero se encuentran completamente aislados. Por ejemplo, existe un namespace específico que agrupa todas las variables globales (por eso puedes utilizar varias funciones sin tener que importar los módulos correspondientes) y cada vez que declaramos una módulo o una función, dicho módulo o función tiene asignado otro namespace.

A pesar de existir una multiplicidad de namespaces, no siempre tenemos acceso a todos ellos desde un punto específico en nuestro programa. Es aquí donde el concepto de scope (campo de aplicación) entra en juego.

Scope es la parte del programa en el que podemos tener acceso a un namespace sin necesidad de prefijos.

En cualquier momento determinado, el programa tiene acceso a tres scopes:
El scope dentro de una función (que tiene nombres locales)
El scope del módulo (que tiene nombres globales)
El scope raíz (que tiene los built-in names)
Cuando se solicita un objeto, Python busca primero el nombre en el scope local, luego en el global, y por último, en el raíz. Cuando anidamos una función dentro de otra función, su scope también queda anidado dentro del scope de la función padre.

```python
def funcion_externa(name1):
    def funcion_interna(name2):
        print(name1)
        print(name1)
```

Este tema se explica muy bien en un post de **Real Python**: https://realpython.com/python-scope-legb-rule/