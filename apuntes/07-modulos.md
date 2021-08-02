# Paquetes, módulos y últimos detalles

# Módulos y paquetes
Un **módulo** es un archivo de Python cuyos objetos (funciones, clases, excepciones, etc.) pueden ser accedidos desde otro archivo. Se trata simplemente de una forma de organizar grandes códigos.

Un **paquete** es una carpeta que contiene varios módulos. Siguiendo el ejemplo anterior, podemos diseñar un paquete matematica creando una carpeta con la siguiente estructura.

Me encanta este apunte: https://tutorial.recursospython.com/modulos-y-paquetes/

# Documentar módulos

Cuando nos encontramos trabajando con módulos, es una buena práctica de programación que nosotros documentamos, más aún, cuando pensamos en liberarlos.

Para documentar un módulo requerimos trabajar con comentarios.

```python
    """
    Aquí, con doble triple comilla documento el módulo, bla, bla, bla.
    """
    def suma(num1, num2):
        return num1 + num2
```

Cómo observamos nuestro script cuenta con tres funciones, una clase y su correspondiente documentación.

El primer comentario es de suma importancia ya que es aquí donde describiremos al módulo, que es lo que hace, que es lo que no hace, cómo funciona, cómo usarlo, entre otras anotaciones que necesitemos colocar, posteriormente podemos colocar algunos metadatos. Los metadatos más comunes son los ocho que podemos observar, sin embargo, si nosotros lo necesitamos podemos agregar los nuestros.

Para que pueda considerarse un metadato debemos de colocar doble guión bajo al inicio y doble guión bajo al final.

Una vez hayamos documentado el script podemos pasar a documentar puntualmente las funciones y las clases.

Si requerimos visualizar la documentación de un módulo basta con un utilizar la función help.

```python
import mi_modulo
help(mi_modulo)
```
Para salir de la documentación basta con presionar **q**.

De esta forma estaremos documentando nuestros módulos sin requerir utilizar algún software adicional.

## Archivo .pyc

**\_\_pycache\_\_** guarda la compilación de calculadora, para que sea más rápido ejecutarlo.

Se crea al importarlo por primera vez y se modifica cuando hay modificaciones en calculadora.py (se vuelve a crear)

## Atributo \_\_name\_\_

Aquí se explica muy bien: https://es.stackoverflow.com/questions/32165/qu%C3%A9-es-if-name-main/32185

## Distribución de paquetas y ejecutables

Desarrollar. [Píldoras informáticas](https://www.youtube.com/watch?v=Zf9sN-w0BVE&list=PLU8oAlHdN5BlvPxziopYZRd55pdqFwkeS&index=36) lo explica bastante bien.