# Primeros Pasos

## Cómo arrancar a programar
La verdad, este ultimo tiempo me estuve rompiendo la cabeza para poder explicar como dar los primeros pasos en **Python**. Haciendo un curso en [Platzi](https://platzi.com/) aprendí que hay varios tipos de estudiantes.

Algunos estudiantes prefieren aprender bien la teoría, para luego luego ir a la práctica, otros prefieren aprender mientras practican, otros son cracks y entienden todo de una. Yo me considero el primer "tipo de estudiante". Siempre me costó aprender, pero fuí perseverante.

Luego de varios años estudiando, me di cuenta que primero necesito aprender bien la teoría, para luego llevarlo a la práctica. Y también, me fue costando menos aprender más rápido.

Volviendo un poco al punto de ***"dar los primeros pasos"***, luego de leer varios blogs y de empezar a escribir y ordenar todo lo que quería expresar, lo encontré aquí:

[Microsoft LEARN](https://docs.microsoft.com/es-es/learn/paths/python-first-steps/)

Así es, la verdad que [Microsoft](https://www.microsoft.com/es-ar/) últimamente está haciendo todo bien, y no es de "chupa medias", pero la verdad, que está facilitando todo, desarrollar software, aprender, levantar un servidor linux, etc. Fue y es una de las empresas más controversiales de la historia, pero es de las que más hizo e invirtió por la ciencia y tecnología. Ojalá en algún momento, alguna organización de América Latina esté a la altura.

Ese apunté que comenté es bastante teoríco y a mi me re serviría para entender un poco el giro, pero si ya querés ir a la práctica podes hacer lo siguiente:
- Cómo instalar Python y configurar el entorno de desarrollo con Visual Studio Code:
https://docs.microsoft.com/es-es/learn/modules/python-install-vscode/

- Cómo crear y ejecutar mi primer línea de código:
https://docs.microsoft.com/es-es/learn/modules/python-create-first/

Ahora, si no te copa más leer y querés aprender **Python** viendo videos bien ordenados, paso a paso desde 0, te recomiendo este canal que a mi me sirvió un monton: [Píldoras informaticas - Curso Python desde 0](https://www.youtube.com/watch?v=G2FCfQj-9ig&list=PLU8oAlHdN5BlvPxziopYZRd55pdqFwkeS&ab_channel=pildorasinformaticas). La verdad que gracias a Juan, el creador de ese canal, pude entender muchas un montón de dudas que tuve siempre tuve y solo él, las explica muy bien. También, este curso [freeCodeCamp - Introducción a Programación en Python](https://www.freecodecamp.org/espanol/news/aprende-a-programar-en-python-desde-cero-curso-completo-gratis/) esta muy bueno.

Pero, si no queres ver el curso de [Youtube](https://www.youtube.com/), y queres aprender leyendo y practicando, pasito a pasito, al terminar esos tres documentos de [Microsoft](https://www.microsoft.com/es-ar/), de podes seguir leyendo mis apuntes😄

**Además, aquí voy agregando cosas nuevas o explicando cosas que me van surgiendo mientras escribo código, intentando agregar valor constantemente a este apunte✌️**
## El creador de Python 

Python es un lenguaje de programación creado en los 90 por [Guido Van Rossum](https://gvanrossum.github.io/), con una sintaxis muy limpia, ideal para enseñar a la gente a programar por primera vez. Se trata de un lenguaje de código abierto, de muy alto nivel e interpretado*.

*Sin enbargo, las compilaciones se guardan en las carpetas "\_\_pycache\_\_" que se generan al ejecutar el script en la terminal

Pero bueno, la verdad que ese chabón es un crack y recomiendo leer su código en [Github](https://github.com/gvanrossum) para copiarlo porque es super prolijo, aplica buenas prácticas y [PEP8](https://www.python.org/dev/peps/pep-0008/) que es una guía de estilo de "cómo escribir código".

## ¿Cómo funciona Python? (Explicado por Juancito)

Python se instala en algún lugar de nuestro sistema operativo.

- En **Linux** python está instalado en /usr/bin/python3 
- En **Windows** python está instalado en alguna parte del disco "C".

Todo el texto plano que escribimos en este apunte, la computadora no lo entiende por si solo. Es por esto, que necesitamos utilizar el **intérprete de Python** para poder ejecutar nuestro código.

### Proceso: ###

1)  Escribimos el código en un , por ejemplo: archivo.py.
2) Luego con el intérprete vamos a este archivo y traducimos el código y lo ejecutamos en el mismo momento.
3) El intérprete lee línea a línea y se frena al finalizar la ejecución o ante un error. 

## Documentación

La documentación oficial está en inglés: https://docs.python.org/3/
Y también en castellano: https://docs.python.org/es/3/

En Argentina hay una comunidad donde traduce la información y guía a les estudiantes de python: http://www.python.org.ar/ . Igualmente esta comunidad no está muy activa que digamos,

## Entender la documentación de Python ##

Además de tener este apunte de base para programar, es clave entender cómo está organizada la documentación de Python para cuando ya tengamos un nivel intermedio del lenguaje y queramos entender o consultar cosas, pero no sabemos a dónde recurrir.

Por eso creo, que en principio, ante dudas del lenguaje, debemos recurrir siempre a la documentación oficial y luego a otros sitios de internet que son muy buenos y la comunidad es enorme.

La documentación de Python está ordenada de la siguiente manera:
**Link:** https://docs.python.org/es/3/

Empezando de arriba a la izquierda:

### [¿Qué hay de nuevo en Python?](https://docs.python.org/es/3/whatsnew/3.9.html) ###
Aquí encontraremos las novedades de la última versión respecto a las anteriores, por ejemplo, nuevas funcionalidades.

### [Tutorial](https://docs.python.org/es/3/tutorial/index.html) ###
Es todo lo que vemos en este apunte, pero traducido y empezando por los temas más sencillos. Esta sección tiene un orden distinto, pero al fin y al cabo se puede profundizar lo visto aquí. https://docs.python.org/3/tutorial/index.html

### [Referencia de la librería](https://docs.python.org/es/3/library/index.html) ###
Las librerías son código y funciones que otros ya realizaron en el pasado, como por ejemplo la función exponencial. ¿Para que la voy a codear de nuevo si alguien más ya lo realizó? Es por esto, que una vez que aprendamos a programar bien, podemos utilizar estas librerías que vienen incluidas en el intérprete de python.

### [Referencia del lenguaje](https://docs.python.org/es/3/reference/index.html) ###
Habla del lenguaje y sus buenas prácticas para programar

## Cómo está organizado el apunte

El apunte está organizado en ir de lo más básico a cosas más complejas. Se intenta introducir a conceptos sencillos, además, a entender cómo leer la documentación oficial y finalizar con las cosas más complejas que se pueden realizar con el lenguaje.

***Ahora si, ¡Arranquemos!***