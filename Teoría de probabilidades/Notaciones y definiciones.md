# Permutación

$P^n_r$

## Definición

En combinatoria, el símbolo $P^n_r$ se utiliza para representar la permutación de 'n' elementos tomados de 'r' en 'r'.

Una permutación es una disposición de objetos sin repetición donde el orden es importante. Por ejemplo, si tienes tres elementos: A, B y C, hay seis permutaciones posibles de estos tres elementos: ABC, ACB, BAC, BCA, CAB, CBA.

## Fórmula

La fórmula para calcular la permutación de 'n' elementos tomados de 'r' en 'r' es:

$P^n_r = n! / (n-r)!$

donde "!" denota el factorial, que es el producto de todos los números enteros positivos hasta 'n'.

## Ejemplo

Por ejemplo, si quieres saber cuántas formas diferentes puedes arreglar 5 libros en una estantería de 3 espacios, usarías esta fórmula para obtener:

$P^5_3 = 5! / (5-3)! = 5\cdot4\cdot3 = 60$

Esto significa que hay 60 formas diferentes de organizar 3 libros de un total de 5 en una estantería.

# Permutaciones: Elementos en Espacios

Las permutaciones se refieren a las formas en que puedes organizar 'r' elementos en 'n' espacios, donde el orden importa.

## Perspectiva 1: Asignación de Elementos a Espacios

Estás seleccionando 'r' elementos de 'n' disponibles y decidiendo en qué orden colocarlos en 'r' espacios. En esta perspectiva, te centras en los elementos y cómo se asignan a los espacios.

Ejemplo: Estás seleccionando 3 libros de 5 disponibles y decidiendo en qué orden colocarlos en los espacios de una estantería.

## Perspectiva 2: Asignación de Espacios a Elementos

Estás seleccionando 'r' espacios y decidiendo qué elemento de 'n' disponibles colocar en cada uno. En esta perspectiva, te centras en los espacios y cómo se asignan los elementos a ellos.

Ejemplo: Estás seleccionando 3 cajas de 5 disponibles y decidiendo qué pelota colocar en cada una.

# Caso Especial: Más Espacios que Elementos

Cuando hay más espacios que elementos (n > r), las permutaciones representan las formas diferentes en que puedes colocar 'r' elementos únicos en 'n' espacios únicos, teniendo en cuenta el orden.

## Perspectiva 1: Asignación de Elementos a Espacios

Estás seleccionando 'r' elementos de 'n' disponibles y decidiendo en qué orden y en qué cajas de las 'n' disponibles colocarlos. Por ejemplo, puedes colocar la pelota 1 en la caja 2, la pelota 2 en la caja 5 y la pelota 3 en la caja 1, y así sucesivamente para cada permutación.

## Perspectiva 2: Asignación de Espacios a Elementos

Estás seleccionando 'r' cajas de las 'n' disponibles y decidiendo qué pelota de las 'r' disponibles colocar en cada una. Por ejemplo, puedes seleccionar las cajas 2, 5 y 1 y decidir colocar la pelota 1 en la caja 2, la pelota 2 en la caja 5 y la pelota 3 en la caja 1, y así sucesivamente para cada permutación

# Combinación

$C^n_r$

## Definición
En combinatoria, el símbolo $C^n_r$ se utiliza para representar la combinación de 'n' elementos tomados de 'r' en 'r'. 

Una combinación es una selección de objetos sin tener en cuenta el orden. Por ejemplo, si tienes tres elementos: A, B y C, solo hay una combinación de estos tres elementos: ABC.

## Fórmula
La fórmula para calcular la combinación de 'n' elementos tomados de 'r' en 'r' es:

$C^n_r = n! / [(n-r)! * r!]$

donde "!" denota el factorial, que es el producto de todos los números enteros positivos hasta 'n'.

## Ejemplo
Por ejemplo, si quieres saber cuántas combinaciones diferentes puedes hacer al seleccionar 3 libros de un total de 5, usarías esta fórmula para obtener:

$C^5_3 = 5! / [(5-3)! * 3!] = 10$

Esto significa que hay 10 formas diferentes de seleccionar 3 libros de un total de 5.

# Combinaciones: Selección de Elementos

Las combinaciones se refieren a las formas en que puedes seleccionar 'r' elementos de 'n' disponibles, sin tener en cuenta el orden. 

## Perspectiva 1: Selección de Elementos sin Importar el Orden

Estás seleccionando 'r' elementos de 'n' disponibles, pero a diferencia de las permutaciones, aquí el orden no importa. En esta perspectiva, te centras en los elementos y cómo se seleccionan, independientemente de su disposición.

Ejemplo: Estás seleccionando 3 libros de 5 disponibles para llevar a un viaje. No importa el orden en el que los empacaste, solo importa qué libros seleccionaste. 

# Caso Especial: Combinaciones con Repetición

Cuando se permite la repetición de elementos en las combinaciones, se utiliza una fórmula diferente. En este caso, la combinación con repetición de 'n' elementos tomados de 'r' en 'r' se calcula como:

$C^{n+r-1}_r = (n+r-1)! / [(n-1)! * r!]$

En este caso, se pueden seleccionar 'r' elementos de 'n' disponibles, y cada elemento puede ser seleccionado más de una vez.

Ejemplo: Si estás seleccionando 3 frutas para hacer un batido de un total de 5 tipos de frutas, y puedes seleccionar el mismo tipo de fruta más de una vez, usarías la fórmula de combinación con repetición.