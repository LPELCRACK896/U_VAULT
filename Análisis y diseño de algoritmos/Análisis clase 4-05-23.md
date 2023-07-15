(falté la clase anterior así q no sé q pedo)

## Nueva instancia de Knapsack problem

Mencionó que la versión que comprobamos tenía la propiedad greedy es la versión binaria del [[Algoritmos Greedy#Knapsack problem|Knapsack problem]], es decir la versión en la que se elije todo el objeto o no, y no parte de él. El peso, es fraccionado o binario. 

Se presenta la nueva instancia donde si se puede dar ese caso. Donde se puede elegir parte del peso del objeto. 

_**Considera la siguiente instancia...**_

Lo siguiente representa el subproblema tras haber tomado la decisión de la elegir si va o no el artículo de la bolsa. Donde i representa al artículo y el W el peso inicial. Y P representa el problema. _Notar como la instancia de un problema genera la instanciación de otros dos --> De problema a subproblemas_

Consiedere lo siguiente una notación conveniente para mostrar como cambian los parametros un subproblema a otro.

### Solución 

`P[i][w] = max(P[i-1][w-w_i] + p_i, P[i-1][w])`


**Notar: El primrer parametro de max representa seleccionar el item i, y el segundo no. Para los subproblemas la selección se hace sin tomar en cuenta este elemento, y es por ello que los subproblemas tiene como parametro i-1**

(Esto se cálcula ya sea con _Top down_ o _Botton Down_, recordar que esto es así dado que tiene **Subestructura optima**)

Notar también que la aplicación de este algoritmo también depende del hecho que si `w_i<W`. Al menos para el primer parametro del max (donde si se selecciona.)


### Tabla de soluciones óptimas 

Esta tabla representa  las soluciones de los problemas. 
Donde a_n representa la selección de un artículo. 
Y la fila W son los pesos que resuelve. 
xd
En todo caso, cada columna representa la solución óptima para w_i. Comenzando con alguna w mínima en caso sea botton up.  Según Tomás, se comienza con una bolsa de tamaño w_0. :v

```
		W...>> (hasta el W que resolvemos)
	 ____________________________________________________________________
    |____________________________________________________________________
    |____________________________________________________________________
    |____________________________________________________________________
    |____________________________________________________________________
a_n |____________________________________________________________________
    |____________________________________________________________________
    |____________________________________________________________________
    |____________________________________________________________________
    |____________________________________________________________________
	    .................................................................
```


