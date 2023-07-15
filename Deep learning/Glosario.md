# Adam

# Adaline

# Aprendizaje supervisado


# Aprendizaje no supervisado 

# Aprendizaje de representaciones

# Backpropagation

# BIAS
Tambien referido como [[#Sesgo]]

# BPTT

# Cajas negras

# Celda de memoria

# Conexiones simétricas

# Convergencia


# Dendritas
Basado en el modelo McCulloh & Pitts, una dendrita es una entrada que permite números binarios que representan señales eléctricas. 

# Descenso de gradiente
El descenso de gradiente es un algoritmo de optimización que utiliza el gradiente de la función de pérdida con respecto a los parámetros del modelo para determinar cómo ajustar los parámetros de manera que la función de pérdida se minimice. Esencialmente, se toma el gradiente de la función de pérdida en el punto actual en el espacio de parámetros y se mueve en la dirección opuesta (descenso) para encontrar un mínimo.

El gradiente es esencialmente una forma de usar la información sobre el cambio local en la función de pérdida para encontrar su mínimo global (o un mínimo local, dependiendo de la naturaleza de la función y la inicialización de los parámetros).

Un problema común en este proceso es el problema del "desvanecimiento del gradiente", donde el gradiente se vuelve muy pequeño y por lo tanto el proceso de aprendizaje se vuelve muy lento. Existen diversas estrategias y modificaciones al descenso de gradiente básico para manejar estos problemas, como el uso de momentos (descenso de gradiente con momento), RMSprop, Adam, entre otros.
# Dropout

# Función de activación

# Gradiente

En el contexto de las matemáticas y la ciencia de la computación, un gradiente es una función que calcula la dirección y la tasa de cambio más rápida en un punto dado en un espacio. En el espacio de varias dimensiones, un gradiente es un vector que apunta en la dirección de la pendiente más empinada desde un punto específico.

En el aprendizaje automático y las redes neuronales, el gradiente es fundamental para optimizar las funciones de pérdida o costo. La idea es ajustar los parámetros del modelo, como los pesos de la red neuronal, para minimizar la función de pérdida. Esto se logra a través de un proceso llamado [[#Descenso de gradiente|descenso de gradiente]].


# GRU

# IEEE CIS

# IJCNN

# INNS

# Learning rate

# Lógica de umbral
La lógica de umbral se refiere a la idea de que una neurona se activará (es decir, enviará una señal) sólo cuando las señales que recibe superen cierto "umbral". En el modelo de McCulloch-Pitts, este umbral es un valor fijo y la salida es binaria (0 o 1).

## Lógica de umbral discreta
cuando hablamos de "lógica de umbral discreta", estamos hablando de una función de activación en la cual la salida de la neurona es un valor discreto (por ejemplo, 0 o 1), independientemente de cuánto superen las señales de entrada el umbral. Este es el caso del modelo de McCulloch-Pitts.
## Lógica de umbral continua
Cuando hablamos de "lógica de umbral continua", podríamos estar hablando de una función de activación en la cual la salida de la neurona puede tomar cualquier valor en un rango continuo, dependiendo de cuánto superen las señales de entrada el umbral. Una función de activación de este tipo podría ser la función sigmoidea, que produce una salida continua entre 0 y 1.
## Transición continua a discreta
Una señal analógica que se convierte en una señal digital. En la señal analógica, los valores pueden cambiar de manera continua y suave, mientras que en la señal digital, los valores cambian en pasos discretos, creando una especie de gráfica con "dientes cuadrados".
# LSTM

# Madaline

# Neuronas

# Normalización de lotes

# Parada temprana

# Perceptron

# Pesos
Cantidad numérica por la que se multiplica por la entrada que llega por la [[#Dendritas]], representando una medida de fuerza de la entrada específica. 
# Propagación hacia atrás

# Red neuronal recurrente

# Regla de perceptron

# Regla de Hebb
La regla de Hebb, a menudo resumida como "las células que se disparan juntas, se conectan", propone que la eficacia de la sinapsis entre dos neuronas aumenta cuando las neuronas se activan simultáneamente. Esta teoría proporcionó un mecanismo para el aprendizaje y la memoria en el cerebro y ha sido fundamental en el desarrollo de las redes neuronales artificiales.

La regla de Hebb ha sido esencial en el desarrollo de la teoría de las redes neuronales, ya que proporcionó una explicación de cómo las neuronas podrían cambiar sus conexiones sinápticas con el tiempo, en respuesta a la experiencia, lo que es esencial para el aprendizaje y la adaptación.

# RMSProp
# RNN

# Sesgo 
Otra forma de llamas al [[#BIAS]]. En español. 

# Sobreajuste

# Umbral