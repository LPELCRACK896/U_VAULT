Deriva del [[Divide & Conquer]]. La programación dinámica es comúnmente empleada para [[Análisis y diseño de algoritmos/Glosario#Problemas de optimización|problemas de optimización]]. Para que un problema de optimización se le pueda aplicar programación dinámica debe tener dos características : 
- **[[#Subestructura optima]]**
- **[[#Problemas traslapados]]**

## Subestructura optima 
Es un concepto intuitivo pero *enredado* de explicar. 
Partimos del hecho que dado que se basa en [[Divide & Conquer|DaC]], la programación dinámica resuelve los problemas de manera recursiva. De modo que cuando 

***...la solución óptima a un problema de estos se compone, a su vez, de las soluciones óptimas a sus correspondientes subproblemas***, este problema exhibe una subestructura óptima.

Como punto de partida y referencia tenemos el **[[#rod-cutting problem]]** 

### rod-cutting problem

Esta nos presenta a una empresa que vende tubos de metal. La empresa considera un tubo de longitud *n*, y el precio de un trozo de tubo con longitud *i  = 1, 2, 3, ..., n* será p_i. 

 

#### Primera pregunta

**Si queremos cortar el tubo en pedazo vendibles ¿qué obtenemos al cortar el tubo de tamaño n en la longitud 0<=i<n? ¿De cuantas formas podemos hacer el corte?**

R// Un corte nos da dos tubos, uno de tamaño i y otro de tamaño n-i. Podemos elegir cortar el tubo en n posiciones diferentes. 

Supongamos esta tabla de precio por tamaño


Longitd. i      1      2      3      4      5      6      7      8      9      10    
______________________________________________________________________
Precio  pi      1      5      8      9     10     17    17   20     24      30    

La tabla muestra que un tubo de tamaño 4 puede producir una mejor ganancia vendiendo como dos sub-tubos de tamaño 2 que vendido entero. 

La empresa sabe que puede cortar el tubo de tamaño n de forma que los dos tubos resultantes produzcan la máxima ganancia posible. Naturalmente, podemos hacer lo mismo con los sub-tubos que pueden cortarse recursivamente hasta alcanzar la unidad de venta mínima. 

Supongamos que tenemos dos tubos tamaño m. Y que uno se corta en j y el otro en k. Quedandonos cuatro tubos. 
n-j ; j --> Para el primer tubo
n-k; k  --> Para el segundo tubo

Optimizando el valor de cada tubo y por tanto obtenemos valores g1(de la primera pareja) y g2(de la segunda pareja). Pero podría resulta que g2>g1. Evidenciando que podríamos haber obtenido mejor ganancia total su hubieramos cortado ambos tubos en la posición k, porque 2g1>g1+g2. Derivado de ese pensamiento, podemos concluir que habrá alguna posición i_p que produzca una pareja de subtubos cuyas ganancias maximizadas y combinadas sean más que las de cualquier otra pareja obtenida al cortar el tubo en cualquier otra posición. 

En el proceso de encontrar esta optimización es fundamental saber que esta solo se alcanzara siempre y que los subtubos también sea apropiadamente oprimitzados. De lo contrario no se llegará; aún cuando el "primer corte" sea el óptimo. 

De esta manera vemos la naturaleza aditiva de la maximización de ganancia. Porque...
**debemos cortar el tubo original en la posición correcta para obtener la mejor ganancia posible, pero esto requiere a la vez que lo subtubos también sean cortados de manera óptima y así *recursivamente***

En otras palabras, **La solución óptima para un problema depende de la solución óptima para los subproblema s en los que se subdivide**. Exhibiendo que el [[#rod-cutting problem]] tiene la propiedad de [[#Subestructura optima|subestructura optima]]. 

Un problema que no muestra esta propiedad por ejemplo es [[#Problema del camino más simple en un grafo sin costos]]. Pero lo dejamos para después dado que demuestra lo contrario y no es necesario (en mi opinión) para expandir el concepto si no más bien para aclarar sobre otro ejemplo. Pero si menciona la importancia de la **[[Análisis y diseño de algoritmos/Glosario#Independencia entre subproblemas|independencia entre sub-problemas]]**. 

Hay dos características que gobiernan la **subestructura óptima** de un problema: 
- **Número de decisiones** 
- **Número de subproblemas**
Para identificar la subestructura óptima de un problema normalmente seguimos los siguiente pasos. 
### Pasos para identificar la sub-estructura óptima de un problema

1. **Identificar las(s) decisión(s)**: en los problemas de [[Divide & Conquer|DaC]] debemos tomar decisiones que producen los subproblemas a resolver. Por ejemplo, ¿Dónde dividir una lista de números? Esas son las decisiones que debemos identificar. 
2. **Identificar los subproblemas**: suponiendo que tomamos la o las decisiones que nos llevan a una solución óptima, identificamos los subproblemas estas producen y las características de este conjunto de subproblemas resultante. 
3. **Demostrar la necesidad de optimalidad**: Por último, observamos que ya estamos en camino a solucionar óptimamente el problema original. Demostramos en este paso que, para solucionar el problema óptimamente, las soluciones a los subproblemas deben ser las óptimas. Para ello suponemos que tenemos la solución óptima compuesta de solución subóptimas a los subproblemas. La idea es revelar que si hubieramos obtenido las soluciones óptimas habríamos producido una mejor solución general, **contradiciendo** que podemos producir una solución óptima usando soluciones subóptimas a los subproblemas. 

----AÑADIR PREGUNTAS 3 y 4 que ejemplifican estas preguntas parar el rod-cutting problem----

## Problemas traslapados

La otra característica esencial de un problema que se desee resolver con programación dinámica es que tenga **subproblemas traslapados**. Esta es en realidad ***la*** característica que define a un problema como solucionable con programación dinámica, puesto que la subestructura óptima es también característica de paradigma de diseño **[[Algoritmos Greedy|Greedy]]**.
### Pregunta 5
Esbozemos, por ejemplo, el [[Análisis y diseño de algoritmos/Glosario#Árbol de recursión|árbol de recursión]] de la sucesión de Fibonacci. 

F(n) = F(n-1) + F(n-2)
n = 5
![[Pasted image 20230525000024.png]]

Notamos que se repiten subproblema, por ejemplo F(3) y F(2). 

### Pregunta 6
Este árbol muestra una enificencia en realizar un mismo problema más de una vez. Podríamos reesbozar este árbol evitando esta ineficiencia. 
![[Pasted image 20230525000352.png]]

Precisamente a esto se refiere la característica de **subproblemas traslapados**. A subproblemas que son engendrados y resueltos redundatemente. 

Programación dinámica refina el paradigma DaC aracando la ineficencia de subproblemas traslapados con una ente dos manera. 

### Métodos para resolver ineficiencia de subproblemas traslapados

#### Top-down with memoization (método de arriba a abjo con memoización)

Se [[Análisis y diseño de algoritmos/Glosario#Memoización|memoiza]] el método DaC agregando una tabla de soluciones que es consultada cada vez que vamos a resolver un subproblema. Si no hallamos la solución a dicho subproblema en la tabla, se computa esa solución y se almacena en la tabla. De lo contrario se usa el resultado almacenado. 

En caso no sea necesario o conveniente resolver todos los subproblemas por lo menos una vez, es más conveniente utilizar top-down porque este solo resuelve aquellos problemas que va a necesitar. Este enfoque es más intuitivo porque es un DaC con memoización. 


#### Bottom-up (método de abajo hacia arriba)

Este método requiere que identifiquemos todos los subprobelmas y los ordenemos por dependencia. Luego, comenzamos por solucionar los casos triviales y continuamos con los subproblemas que dependen de ellos; y después los subprobelmas que dependen de estos últimos, sucesivamente, hasta llegar al problema original. 

Para los problemas de programación dinámica que será necesario o conveniente resolver absolutamente todos los subproblemas por lo menos un avez es conveniente utilizar bottom-up, dado que este no es recursivo y tiene mejor manejo de la tabla de subproblemas. 


Finalmente, las diferencias de desempeño entre estos métodos será casi siempre factores constantes en ambos métodos. Asíntoticamente, tendrán la misma tasa de crecimiento por lo que decimos que normlamente son igual de eficientes. 


## Síntesis de programación dinámica hasta el momento

Considerando las dos características esenciales de la programación dinámica observamos, entonces, que el árbol de recursión que usamos con el paradigma DaC se convierte en un **grafo de subproblemas** al fusionar los subproblemas que aparecen más de una vez. 

En general, para construir un algoritmo usando programación dinámica debemos seguir cuatro pasos: 
## Pasos para construir un algoritmos usando programación dinámica

1. [[#Paso 1 Caracterizar la solución del problema|Caracterizar la solución óptima]]. 
2. [[#Paso 2 Describir el valor de la solución óptima de forma recursiva.|Describir el valor de la solución óptima de forma recursiva]]. 
3. [[#Paso 3 Computar el valor de la solución óptima.|Computar el valor de la solución óptima.]] 
4. [[#Paso 4 Construir la solución óptima|Construir la solución óptima.]] 

### Paso 1: Caracterizar la solución del problema
Identifica la subestructura óptima en el problema y, con base en ella, determina como hallar la solución  óptima de manera recursiva. Como se djio anteriormente, para alcanzar a identificar la subestructura óptima suponemos que nos es(son) dada(s) la(s) decisión(es) que hay que tomar sobre el problema para alcanzar la solución óptima. Este paso remueve esa suposición y determina cómo se va buscar la decisión correcta que nos llevará a la solución óptima. __Es como armar el esqueleto del algoritmo__. 

### Paso 2: Describir el valor de la solución óptima de forma recursiva. 
Construir la relación de recurrencia que calcula el valor de la soluciónn óptima basándose en el paso anterior. Esta relación especifica la manera en la que las soluciones a subproblemas se combinan, formando la solución para su problema "padre". El paso anterior asegura que esta relación de recurrencia expresa el valor de la solución óptima cuando la solución siendo calculada es la del problema raíz. 

### Paso 3: Computar el valor de la solución óptima.
Conlleva escribir el algoritmo que, basado en la ecuación de recurrencia del segundo paso, permita calcular el valor de la solución óptima (ya el mero valor, no sólo una definición). En este paso es donde cobra importancia la característica de los problemas traslapados, pues el algoritmo debe reconocer y evitar la re-computación de soluciones a subproblemas recurrentes. En este paso es también donde se debe elegir el método se solución entre *top_down* y *bottom_down*, siendo *top_down* normalmente más fácil de programar, pero en ocasiones menos eficiente. 

### Paso 4: Construir la solución óptima
Este paso es frecuentemente realizado pero no es necesario. Este paso se encarga de describrir la solución óptima, muestra las soluciones a los subproblemas resueltos para hallar el valor de la solución óptima general. Para lograrlo normalmente se agregan, al algoritmo del paso tres, instrucciones que almacenen información sobre los pasos en la computación del valor óptimo. 

# Extra

## Problema del camino más simple en un grafo sin costos

Pendiente

Para este problema vemos que en la búsqueda de la solución óptima a los subproblemas considerados provee una solución inválida al problema inicial. (relacionado con las condiciones y naturaleza del problema) ya que el camino deja de ser simple al intentar resolver el subproblema (un búcle que contradice el camino simple). Entonces, como la solución óptima a este problema no se puede construir a partir de soluciones óptimas a subproblemas ese es un problema **sin subestructura óptima**. 