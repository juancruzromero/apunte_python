# Estructura de Datos #

## Listas[] ##

Son una secuencia de elementos
Son parecidos a los arrays. Tienen la misma utilidad.
Permiten almacenar varios valores.

Documentación oficial - Sección: Tutorial de Python:

Aquí se hace una pequeña introducción a las listas:
https://docs.python.org/es/3/tutorial/introduction.html#lists
Métodos de las listas:
https://docs.python.org/es/3/tutorial/datastructures.html#more-on-lists

### Sintaxis ###
```python
mi_lista = [0,1,2,"a","b","c"]
```

### Métodos para manipular Listas[] ###
- append()
- extend()
- insert()
- index()
- remove()

### SubListas:
Estas son las formas en las cuales podemos crear una nueva lista (sublistas) a partir de otra.

[:] Todos los elementos.
[start:] Todos los elementos desde el índice establecido(start).
[:end] Todos los elementos desde el índice cero hasta el índice establecido(end).
[start:end] Todos los elementos de un rango de índices.
[start:end:step] Todos los elementos de un rango de índices con saltos.
## Tuplas() ##

No pueden modificarse. Son inmutables. No hay búsquedas.
Son más óptimas y rápidas que una lista. Claves en un diccionario.

### Desempaquetado de tuplas
En ciertas ocasiones tendremos la necesidad de obtener algunos elementos de nuestras tuplas, por ejemplo, teniendo la siguiente tupla.

tupla = (10, 20, 30, 40, 50)
Necesito obtener el primero, el segundo y el último elemento; Para lograr esto tendremos un par de opciones; trabajando con índices y sin ellos. Veamos.

Si trabajamos con índices podemos hacerlo lo siguiente.

primero = tupla[0]
segundo = tupla[1]
ultimo = tupla[-1]
o simplemente podemos reducir las líneas de código y dejarlo en una sola.

primero, segundo, ultimo = tupla[0], tupla[1], tupla[-1]
La segunda opción es dejar de trabajar con las los índices y utilizar el guión bajo _.

primero, segundo, _, _, ultimo = tupla
Como observamos he colocado dos guiones bajos que hacen referencia a el número 30 y el número 40, valores que no necesitamos, por en de, no necesito almacenarlos en alguna variable; simplemente los ignoramos.

Ahora, que pasa si tengo una tupla mucho más grande y nuevamente necesito obtener esos tres elementos (el primero, el segundo y el último).

tupla = (10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 200, 300, 400)
Lo que podemos hacer es utilizar el guión bajo _ junto con el asterisco * y aplicar lo que hemos visto anteriormente.

primero, segundo, *_, ultimo = tupla
De esta forma podemos trabajar de una forma más eficiente con las tuplas.

## Diccionarios {}

Puedo almacenar todo tipo de datos y listas dentro de diccionarios.
Asociación “Clave - Valor”.
Los elementos almacenados no están ordenados.


## Optimización

### Búsqueda binaria
Los algoritmos son una serie de instrucciones que nos llevan a un resultado, por ejemplo que tal si queremos saber si un número se encuentra en una lista.

Una forma es buscar un ítem tras otro, pero sí la lista es muy larga esta forma no es la más eficiente, una forma más eficiente de solucionar este problema es usar una búsqueda binaria.

Con el algoritmo de búsqueda binaria partimos de la lista ordenada, nosotros sabemos que hay números mayores y menores que el número que estamos buscando.

Seleccionamos un número aleatorio para dividir la lista, puedes escoger cualquier número, en éste caso sumamos el primer y el último índice de la lista, los sumamos y dividimos en dos (por eso se llama binario), luego comparamos el número que está en el índice, de esta manera ya eliminamos la mitad de las opciones. Podemos continuar dividiendo la lista y comparando hasta que lleguemos al resultado esperado.

## Conjuntos y listas (set())

Los conjuntos o sets evitan duplicados

## Comprehension
Básicamente son una forma de crear listas de una manera elegante simplificando el código al máximo. Muy loco, Python define una estructura que permite crear listas de un modo un tanto especial. Te lo mostraré con un ejemplo:

Aquí lo explican muy bien: https://j2logo.com/list-comprehensions-en-python/