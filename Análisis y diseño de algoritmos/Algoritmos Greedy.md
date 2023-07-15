Para algunos [[Análisis y diseño de algoritmos/Glosario#Problemas de optimización|Problemas de optimización]] podemos emplear un acercamiento más económico que el de programación dinámica. Este es el acercamiento ***greedy***, llamado así por construir soluciones "en el camino", tomando cada decisión según lo que parezca mejor en el momento. Es decir, los algoritmos greedy simplemente cambian la forma en la que se toman las decisiones durante la construcción de una solución óptima. Ya no nos metemos a resolver subproblemas antes de tomar una decisión, sino que tomamos la ceisión basandonos en la información que el problema actual provee. 

La [[Programación dinámica#Subestructura optima|subestructura optima]] también es un requerimiento de los problemas de optimización a los que se aplique el acercamiento greedy porque este acercamiento producirá, en cada paso, suboproblemas que serán resueltos con base a ese mismo criterio. 

### Propiedad de la elección codiciosa  (greedy-choice property)

Se puede expresar como la combinación de  una decisión greedy y la solución óptima al subproblema que produce debería resultar en la solución óptima  al problema general.




Análisis y diseño de algoritmos clase 27/04/2023
Tomás Gálvez
## Knapsack problem

Problema de ladrón que estaba robando y que se queda sin tiempo para robar **todo** . 
¿Que hace? Roba lo que considerá más valioso. Optimiza el valor del robo. El problema se optimiza localmente en términos de tiempo. 

Se debe demostrar que es un problema que tiene subestructura óptima. 
### Definicion de problema

**Entrada**: W, k[ ], a[ ]

La estructura **k** es un arreglo que tiene el precio **unitario** de algún artículo (no necesariamente tenemos un artículo de cada artículo). 

**W** es el peso máximo soportable por el ladrón.

Nota personal: Debemos considerar que los artículos están _estandarizadas_ en función del peso. Es decir, cada unidad pesa lo mismo y lo que cambia es la cantidad de unidades que tenemos de los artículos. 

Por tanto, el arreglo **a** tiene la cantidad de _unidades_ que tenemos de cada artículo. 
 

1. Identificar las decisiones
	- **La decisión**: La selección de elementos para meter en la mochila para maximizar su valor. 
2. Identificar subproblemas
	- **El subproblema:**  : Un subproblema en el problema de la mochila fraccionada se presenta cuando se considera un subconjunto de elementos y una capacidad menor a la capacidad original de la mochila. Resolver un subproblema implica tomar decisiones similares a las del problema original, es decir, seleccionar elementos
3. Demostrar necesaria optimalidad
	- Tenemos una solución óptima que incluye el peso C1. Pero aún debe llenarse el resto de los espacios. 
	- Dado que no existe una restricción con la elección de los demás artículos (no es un subproblema que debe resolverse como estamos resolviendo este problema )


Pregunta 4
------
**Explique por qué este problema presenta la greedy-choice property.****
Para este caso, es demostrar que la solución en el subproblema _debe_, es decir, la solución local también es la solución que lleva a la optimalidad a todo el problema. 

Porbamos este punto con contradicción. 

Suponemos una solución óptima de la siguiente forma 

{ SECCION OPTIMIZADA }, __ 
A la seccíon optimizada le damos un valor U. 
Y nos queda aún un valor por ocupar para completar el problema. 
Suponemos por lo menos dos posibles elecciones: 
- p_k 
- p_c
Donde p_k>p_c.

Es decir que localmente, la solución de este problema es la elección de p_k. Pero dado que queremos demostrar que esto es necesario para encontrar la solución óptima al problema en general, elegimos el otro (p_c), para ver que sucede con la optimización de todo el problema. 

Nuestra solución "optima" con esta elección nos lleva a
*p_c + U*
¡Pero esto no es posible! Es contrdictorio. La elección de p_k  llevaría a un valor más óptimo en el problema que el encontrado con la elección de p_c. 

*p_c + U* < p_k + U

Por tanto, la propiedad greedy es una propiedad de este problema. 