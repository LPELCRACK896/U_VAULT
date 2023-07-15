### Árbol de recursión
Estructura que muestra la recursión de un problema y su relación con las llamadas que puede hacer a otros problema, usualmente con un input distinto. De esta estructura podemos distinguir varios elementos.
- **Raíz**: Muestra el problema original del cual derivan las demás llamadas a la resolucíon
- **Aristas**: Desconozco si para este contexto se le identifican como aristas pero para un grafo son las línea que unen las aristas, y sobre este contexto podemos verlo como las líneas que unen los nodos del árbol, mostrando las llamadas y por tanto dependencia que existe entre los problemas. 
- **Nodos internos**: Son los nodos que representan problemas llamados ya sea por otros nodos internos o por la misma raíz. Es el cuerpo del árbol. 
- **Hojas**: Son los nodos que terminan con la recursión y se encuentran hasta abajo del árbol representando la última llamada recursiva y una resolución a un "suproblema".

# Programación dinámica

### Problemas de optimización
Problemas con múltiples soluciones en el que buscamos la que tenga el máximo o mínimo valor según nuestras necesidades. 

### rod-cutting problem
Problemas que exhibe la subestructura óptima en un problema. 

### Paradigma
Un paradigma, en diseño de algoritmos, es una clasificación definida por la forma general que comparten los algoritmos de ese paradigma. 

### Independencia entre subproblemas
Se refiere a que computar la solución de un subproblema no depende de **recursos** de, o no se ve afectada (según las **condiciones del problema**) por, la solución para otro subproblema. En otras palabras, la solución a un subproblema no afecta la solución para un subproblema "hermano". 

### Memoización
En Informática, el término memoización es una técnica de optimización que se usa principalmente para acelerar los tiempos de cálculo, almacenando los resultados de la llamada a una subrutina en una memoria intermedia o búfer y devolviendo esos mismos valores cuando se llame de nuevo a la subrutina o función con los mismos parámetros de entrada.