12/07/2023
Esto es un resumen del libro [[Pacheco.pdf]]

# Prefacio
Indica que el temas de computadoras y procesamiento paralelos es un tema actual que no ha tomado tant relevancia en los pensum de carreras universitarias de computación (2011). Se debe sacar todo el provecho que provee la programación paralela en hilos por la mejora en rendimiento que está puede dar a diferencia de un programa que corre en un solo núcleo.

Por este motivo se escribió este libro, siendo una introducción a la programación paralela utilizando las siguientes API's: 
- MPI
- PThreads
- OpenMP

Es requisito un conocimiento básico en matemática y programación secuencial en C. 

## Sobre el libro
El libro enseña programación paralela sobre las tres API's pero si el lector lo desea puede omitir las que desea y aún aprender sobre algún otro sin mayor esfuerzo puesto que los tres capítulos de las API's son ampliamente independientes entre sí; no tiene orden. 

### Chapter 1
Para los menos experimentados, el primer capítulo sirve como base para una explicación no-técnica de un sistema paralelo así como una introducción a sistemas paralelos y programación paralela. 

### Chapter 2
Provee material más técnico sobre el hardware y software computacional. 

### Chapter 3, 4 y 5
Son introducciones a la programación a través de las API's. 
- Capítulo 3 $\rightarrow$ MPI
- Capítulo 4 $\rightarrow$ PThreads
- Capítulo 5$\rightarrow$ OpenMP

### Chapter 6
Se desarrollan dos programas largos. 
1. "A parrallel n-body solver"
2. "Parrallel tree searcher"
Ambos programas utilizando las 3 apis. 

### Chapter 7
Una listado de información adicional sobre varios aspectos en torno a la computación paralela. 



# Capítulo 1: ¿Por qué computación paralela?

De 1986 a 2002 el rendimiento de microprocesadores aumentaba en promedio un 50% al año, sin embargo, llegado el 2002 el ritmo de crecimiento desaceleró a un 20% por año.  Este decrecimiento se asoció con el gran cambio en el diseño del procesador. A partir del 2005, la mayoría de manufacturers se fue por el camino del **paralelismo** para aumentar su rendimiento rápido, en lugar de insistir conn aumentar el rendimiento de **procesadores monolíticos**.  **Comenzaron a poner múltiples procesadores completos en una solo circuito integrado**. 

Este cambio tendría un impacto para los desarrolladores de software. El hecho de añadir más procesadores no aumentaría mágicamente el rendimiento de sus programas secuenciales. Dichos programas no eran consientes del multiprocesador, de manera que finalmente que, efectivamente, tenían el mismo rendimiento que en los procesadores de un solo núcleo. 

Derivado de ello, surgieron las preguntas: 
- ¿Por qué molestarse? ¿Un solo procesador no era suficientemente rápido? Después de todo, el incremento de 20% anual aún representa un incremento significativo. 
- ¿Por que los manufacturadores de microprocesadores no pueden seguir desarrollando procesadores monolíticos mucho más rápidos? ¿Por qué construir sistemas paralelos? ¿Por qué construir sistemas con multi-procesador?
- ¿Por qué no podemos crear programas que transformen programas secuenciales en programas paralelos? Para poder aprovechar los recursos de un procesador multinúcleo. 

## ¿Por que necesitamos mejorar el rendimiento?
(de momento omitiré esta parte)

# Capítulo 2: Hardware y software paralelo

Página PDF: 36
Página libro: 15

## Resumen
Para hacer programas paralelas de la forma más eficiente se requiere:  
1. Conocimiento del hardware subyacente y software del sistema. 
2. Conocimiento de los distintos tipos de software paralelo. 
3. Saber como evaluar el rendimiento de un programa paralelo y métodos para desarrollar programas paralelos. 

## Marco de referencia
Hardware y software paralelo surgen d hardware y software secuencial (que corre una tarea a la vez), por tanto es necesario hacer una revisión a estos para empezar. 
### La arquitectura Von Neumann
La clásica arquitectura Von Neumann consiste en
- Una memoria principal  ([[#Main memory|main memory]])
- [[#CPU|Una una central de procesamiento]](**Central Processing Unit $\rightarrow$ CPU**)/Procesador/Core (Núcleo) 
- Un **[[#Canal de interconexión (bus)|canal de interconexión]]** entre la memoria principal y el CPU. 

Una máquina Von Neuman ejecutas una instrucción a la vez y cada instrucción opera sobre una secciones de la data. 



![[Arch. Von Neuman.png]]
#### Main memory
Consiste en una colección de locaciones, cada una capaz de almacenar instrucciones o datos. 

Cada locación consiste de 
- Una dirección: Utilizado para acceder al registro. 
- Contenido. 

#### CPU
La unidad central de procesamiento está divido en unidades de:
- [[#Unidad de control|Control]] 
- [[#Unidad aritmética y lógica (ALU)|Aritmética y Lógica]]
##### Unidad de control
Es la encargada de decidir que instrucción en un programa debe ser ejecutada. 
##### Unidad aritmética y lógica (ALU)
Es la responsable de ejecutar las instrucciones. 

Data del CPU e información sobre el estado de ejecución de un programa están almacenados en unidades de almacenamiento extremadamente rápidos llamados **registros**: 

La [[#Unidad de control]] tiene un registro especial llamado **Program Counter (PC)**, que almacena la dirección de la siguiente instrucción a ser ejecutada. 

#### Canal de interconexión (bus)

Tradicionalmente, el canal de interconexión (que transfiere datos e instrucciones entre CPU y memoria principal) ha sido un **bus**. Que consiste en una colección de cables en paralelo  y algunos (hardware) controladores de acceso para los cables. 

$MM \rightarrow CPU$
Cuando data/instrucciones transferida de la memoria al CPU se dice que se obtuvo o leyó (**fetched**) de la memoria. 

$CPU \rightarrow MM$
La transferencia de data del CPU a la memoria es referido como **escritura en memoria o almacenamiento**. 

#### Cuello de botella

La separación de la memoria y CPU es muchas veces referido como el **cuello de botella Von Neumann**, considerando que la interconexión determina el ritmo al que las instrucciones y datos son accesados. La gran cantidad de datos e instrucciones necesarias para ejecutar un programa están aisladas del CPU. Para 2010, los CPU's son capaces de ejecutar instrucciones más de cien veces más rápido de lo que pueden obtener items de la memoria principal. 

Para abordar este problema, y, más general, mejorar el rendimiento del CPU, investigadores experimentaron distintas modificaciones del modelo básico Von Neumann. 

Algunos aspectos relevantes respecto a estas modificaciones requieren un estudio previo a algunos conceptos. 


#### Procesos, multitasking e hilo
$\rightarrow$seguir en página 38 del pdf$\leftarrow$
