# HackEPS Algorithm Challenge



## First Challenge

Un número "Súper-Reversible" es aquel que se puede sumar a si mismo una vez invertidas sus cifras, y que da como resultado un número en el que todas sus cifras son iguales.

Por ejemplo:
```
54: 54 + 45 = 99
```

```
123: 123 + 321 = 444
```

```
135: 135 + 531 = 666
```
Dado un rango de números, tu programa debe calcular (ambos incluidos) cuantos números existen en dicho rango y que cumplen con la condición para ser "Súper-Reversibles". Para hacerlo un poco más difícil, vamos a darte unas cifras un poco altas.
```
1 ≤ A ≤ B ≤ 999,999
```

## Exercise 2

En este segundo reto, debes encontrar la suma de todos los números primos del rango entre A y B (ambos incluidos y que pueden no ser primos).

Por ejemplo, la suma de todos los primos entre 463 y 557 es 6587.
El fichero que te facilitaremos empieza con un número T, el número de casos. Para cada caso, hay una linea que contiene dos enteros A y B, separados por un espacio. Tu programa debe generar una salida de una linea por resultado, con el formato "Case #N: X" donde N es el número de caso y X el resultado.

```
2 ≤ A ≤ B ≤ 9,999,999
```

## Third Exercise

Teniendo en mente un teclado numérico de teléfono móvil. 
![teclado](http://challenge.semicinternet.com/reto-3/reto-3/220pxTelephonekeypad2.svg.png)

Al tener que comunicarse con nosotros, les ayudaremos a que sean un poco más modernos y vamos a hacer que nuestro programa codifique las abreviaturas más conocidas. Esta es la tabla de las que tenemos que interpretar:

```
que -> k
adios -> dw
que tal	-> ktal
te quiero -> mucho	tkm
gracias	-> thx
besos y abrazos	-> xoxo
que carajo -> wtf

```
Debes tener en cuenta otra cosa, y es que a nuestros abuelos les cuesta bastante escribir y tienen una especial predilección por la tecla espacio, por lo tanto, es bastante probable que el texto de entrada tenga muchos espacios sobrantes entre palabras. Si nos encontramos más de un espacio entre dos palabras, sólo tienes que codificar uno. Si está al principio de la frase, debes ignorarlo todo.

Por ejemplo, la palabra hola la codificaremos con 446665552

```
HackEPS se traduciría en #44#2 22255#337 7777
```
Y para terminar, también nos han pedido otra pequeña ayuda. Tenemos que indicarles el movimiento a realizar con el dedo para que puedan encontrar la tecla siguiente de la forma más ágil posible para que no pierdan demasiado tiempo. Vamos a escribir el movimiento que deben realizar. Esto se explica mejor con un ejemplo:

HackEPS se traduce definitivamente en:
```
# arriba arriba izquierda izquierda 44 abajo abajo derecha derecha # arriba arriba arriba izquierda 2 222 abajo 55 abajo abajo derecha # arriba arriba arriba 33 abajo abajo izquierda izquierda 7 7777
```

## Fourth Exercise

En Semic queremos que nuestros compañeros se muevan lo menos posible para ir de su mesa a la cafetería, y queremos diseñar un programa que nos calcule el camino más corto.

El tiempo es oro y quizá no os quede mucho, así que vamos a ir al grano:

* No puedes atravesar las paredes marcadas con un #
* Tienes que dibujar los movimientos con los caracteres del ejemplo.

```
.......#....
.........#.B
......#.#...
...#.....#..
.A....#..#..
...#.#......
```
Quedaría como:
```
.......#┌-┐.
.......┌┘#└B
......#|#...
...#.┌-┘.#..
.A---┘#..#..
...#.#......
```
