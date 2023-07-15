
Link de referencia: 
[RFC 1958 (Architectural Principles of the Internet)](https://datatracker.ietf.org/doc/html/rfc1958)
Documento local: 
[[rfc1958.pdf]]
# Status 
El documento se presenta a sí como un memo que provee información de la *comunidad de internet* (sin entrar en formalidades, ni estándares como tal).
# Resumen
El internet y su arquitectura crecieron desde modestos inicios y no como un ambicioso *gran plan*. Aunque fue su constante evolución lo que lo hace tan atractiva tecnología, vale la pena tener *snapshots* de los **actuales principios de internet**. El artículo no se molesta en intentar definirlo con principios tan rígidos, y más bien busca ser una guía general. 
# Principios arquitectonicos de internet 
## Cambio constante
Como buen representante de la industria tecnológica, el internet ***se mantiene en un constante cambio de sus principios***. Comenzando de sus inicios más humildes ([ARPANET](https://developer.mozilla.org/es/docs/Glossary/Arpanet)) a la actualidad, se denota ha sufrido [[R Architectural Principles of the Internet - Tarea 1 lectura de RFC 1958#Cambios importantes en internet|cambios]] que inevitablemente afectan directamente los principios en su arquitectura. De manera que, principios del pasado que parecían irrevocables fueron depreciados y es alatamente probable que suceda lo mismo con los actuales. **Entre todos, el único principio que parece prevalecer es el de cambio constante**

Por tanto, el objetivo del documento no es presentar un dogma de como se debe diseñar los [[U/Redes/Glosario#Protocolos de internet|protocolos de internet]] o siquiera como deben convivir. La idea es brindar una guía de diseños que han funcionado en el pasado y que valen la pena revisar ya sea para utilizarlos o para evaluarlos. 

Algunos puntos de interés que podrían impulsar cambios en el internet son: 
1. **Límites de escalabilidad para [[U/Redes/Glosario#IPv4|IPv4]]**
	 Cada dispositivo necesita una dirección IP única, pero IPv4 tiene un número limitado de direcciones, aproximadamente 4.3 mil millones. Con el creciente número de dispositivos que acceden a Internet, **nos estamos quedando sin direcciones únicas**. Esta limitación es un motor importante para la adopción de la próxima versión, [[U/Redes/Glosario#IPv6|IPv6]], que ofrece un número de direcciones posibles mucho mayor.
2. **Las redes de gigabit por segundo y el multimedia**
	Con el auge de las redes de alta velocidad capaces de transmitir datos a velocidades de gigabit por segundo, así como la proliferación de multimedia (audio, video, VR, etc.) en Internet, **hay mucha presión sobre las redes y los protocolos de Internet para manejar este tráfico de alto volumen y alto ancho de banda de manera eficiente.** Esto ha impulsado la investigación y el desarrollo de nuevas formas de administrar el tráfico de red.
3. **Necesidad de Calidad de Servicio (QoS) y garantías de seguridad en Internet comercial.** 
	Con el papel vital de Internet en el comercio, existe una creciente necesidad de [[U/Redes/Glosario#QoS|QoS]], que asegura que ciertos tipos de datos (como VoIP, videoconferencias, etc.) tengan prioridad y se transmitan de manera confiable. Además, dada la creciente frecuencia y sofisticación de los ciberataques, también están en alta demanda las características y protocolos de seguridad mejorados.

**"Las máquinas voladoras más pesadas que el aire son imposibles"** *Lord Kelvin* 
Es decir que, aunque los principios que han descrito proporcionan una comprensión actual del campo, no deben considerarse absolutos o inmutables. La ciencia y la tecnología están en constante evolución, y nuestra comprensión y mejores prácticas deberán evolucionar también.

## ¿Existe una arquitectura del internet? - Tradición de internet

Muchos creen que no existe un arquitectura si no una **tradición**. Una tradición no escrita.  

Pero términos más generales y dónde todos suelen coincidir es que: 
- La meta es la **[[#Conectividad|conectividad]]**. 
- La herramienta es el **[[#Internet Protocol]]**
- La inteligencia/lógica está en **los extremos** (**[[#Lógica end-to-end|end to end]]**).  
### Conectividad
***El crecimiento de la red ha probado que su recompensa es la conectividad misma*** más allá de los servicios o aplicaciones que existen. La conectividad requiere cooperación entre los proveedores de servicios. 

La clave de la conectividad global es la capa de interconexión de redes. La clave para explotar esta capa sobre hardware diverso que proporcione conectividad conectividad global es el "argumento extremo a extremo".
### Internet Protocol
#### ¿Un protocolo para dominarlos a todos?
A simple vista, parece que lo ideal sería tener un único protocolo a nivel de internet, ya que permitiría operaciones uniformes y relativamente fluidas en una red pública red pública competitiva, multi-proveedor y multi-proveedor.[[#Un único protocolo tampoco tiene porque ser el único camino.|*]]

***En la realidad existen dos razones por las que más de un protocolo en la capa de red de internet pública.*** 

1. La transición gradual de una IP a otra. 
2. Unos requisitos fundamentalmente nuevos pueden dar lugar a un protocolo fundamentalmente nuevo (evolución de internet a través del cambio constante).
#### Independencia al hardware

***El protocolo a nivel de Internet debe ser independiente del hardware y del direccionamiento hardware.***

Este enfoque permite a Internet explotar cualquier nueva tecnología de transmisión digital de cualquier tipo, y a desacoplar sus mecanismos de direccionamiento del hardware. Permite a Internet sea la forma más fácil de interconectar medios de transmisión y ofrecer una plataforma única para una amplia variedad de aplicaciones y servicios de infraestructura de la información.

Nota: Se profundiza en el tema en \[Clark] The Design Philosophy of the DARPA Internet Protocols, D.D.Clark, Proc SIGCOMM 88, ACM CCR Vol 18, Number 4, August 1988, pages 106-114 (reprinted in ACM CCR Vol 25, Number 1, January 1995, pages 102-111).
Ver ... [[DesignPhilosophyOfDARPA-Clark.pdf]]

### Lógica end-to-end

***La funciones necesarias de extremo a extremo sólo pueden ser realizadas correctamente por los sistemas finales.***

#### Problemáticas asociadas
##### Por integridad de datos
Un caso concreto es que cualquier red, por más cuidadoso que sea su diseño sea sufrirá fallos de transmisión a un ritmo determinado (estadísticamente). Dado el caso, **la mejor forma de afrontarlo es aceptarlo y delegar la integridad de la comunicación a los sistemas finales**
##### Por seguridad de datos
Otro caso específico es la seguridad de extremo a extremo.
Citando a \[Saltzer], "La función en cuestión sólo puede aplicarse completa y correctamente sólo con el conocimiento y la ayuda de la aplicación que se encuentra en los extremos del sistema de comunicación. Por lo tanto, proporcionar esa función cuestionada como una característica del sistema de comunicación no es posible. (A veces, una versión incompleta de la función proporcionada por el sistema de comunicación. útil como mejora del rendimiento"). 

Nota: Se profundiza el tema en \[Saltzer] End-To-End Arguments in System Design, J.H. Saltzer, D.P.Reed, D.D.Clark, ACM TOCS, Vol 2, Number 4, November 1984, pp 277-288.

Ver... [[EndToEndArgument-Saltzer.pdf]]



#### Consecuencias
El seguimiento de este principio implica que las aplicaciones sobrevivan a fallos parciales en la red. 

Un diseño de protocolo end-to-end no debe depender del mantenimiento del estado (donde el estado es la información sobre el estado de comunicación entre las dos partes) dentro de la red. El estado debe permanecer únicamente en los endpoints. Y el estado pueda destruir cuando se rompe el punto final (lo que se conoce como fate-sharing)

Para realizar sus servicios, la red mantiene cierta información de estado: rutas, garantías de calidad de servicio que realiza, información de sesión donde se utiliza en la compresión de encabezados, historiales de compresión para la compresión de datos, y similares. Este estado debe ser auto regenerable; deben existir procedimientos o protocolos adaptables para obtener y mantener ese estado, y cambiarlo cuando cambie la topología o la actividad de la red. El volumen de este estado debe reducirse al mínimo, y la pérdida del estado no debe provocar más que una denegación temporal del servicio dado que existe conectividad.

### De nadie y para todos
Afortunadamente, nadie es dueño de Internet, no hay un control centralizado y nadie puede apagarlo. Su evolución depende de consenso sobre las propuestas técnicas y de la ejecución del código. La retroalimentación de ingeniería de las implementaciones reales es más importante que cualquier principio arquitectónico.

## Cuestiones generales de diseño
### Heterogeneidad 
***La heterogeneidad es inevitable y el diseño debe contemplarlo.***

Admitir la **variedad en hardware** que suele diferir sobre todo en: 
- **Velocidades de transmisiones**, que llegan a diferir en al menos siete ordenes de magnitud.  
- **Longitudes de palabras** (word)
- **Hosts**. Van desde microprocesadores con poca memoria hasta supercomputadoras. 

Admitir la **variedad en tipos de protocolo de aplicación** :
- **Sencillos**, como inicio de sesión remoto. 
- **Complejos**, como las bases de datos distribuidas. 
### Selecciona una solución
***Si hay varias formas de hacer lo mismo, elija una.***

Si un diseño existente ya ha solucionado el problema elíjela, a menos que alguna buena razón técnica para no hacerlo.  **La duplicación de la misma funcionalidad del protocolo debe evitarse en la medida de lo posible, sin utilizar este argumento para rechazar mejoras.**

### Escalabilidad
***Todos los diseños deben escalar fácilmente a muchos nodos por sitio y a millones de sitios.***
### Rendimiento y coste
***Deben tenerse en cuenta el rendimiento y el coste, además de la funcionalidad.***
### Simplicidad
***Hay que simplificar. En caso de duda, elija la solución más sencilla.***

### Modularidad
***La modularidad es buena. Si puede mantener las cosas separadas, hágalo.***

### Solución casi completa vs solución perfecta
***En muchos casos es mejor adoptar ahora una solución casi completa
que esperar a encontrar una solución perfecta.***

### Opciones y parámetros auto-ajustables
***Evite las opciones y los parámetros siempre que sea posible.***
Las opciones y parámetros deben configurarse o negociarse dinámicamente en lugar de manualmente.
#### Aclaración
La recomendación de que cualquier opción o parámetro se debe "configurar o negociar dinámicamente en lugar de manualmente" se refiere a la idea de que los protocolos deben ser capaces de ajustarse automáticamente a las condiciones de la red.


### Estricto al enviar, tolerante al recibir. 
***Las implementaciones deben seguir las especificaciones con precisión al enviar a a la red, y tolerar entradas defectuosas desde la red.***

En caso de duda, descarte la entrada defectuosa en silencio, sin retornar ningún error a menos que así lo exija la especificación.

### Prudencia con paquetes no solicitados
***Sea prudente con los paquetes no solicitados, especialmente las multidifusiones y las difusiones.***

### Evitar referencias circulares
Por ejemplo, el enrutamiento no debe depender de las búsquedas en el Domain Domain Name System (DNS), ya que la actualización de los servidores DNS depende del del éxito del enrutamiento.

### Objetos autodescriptivos pero no tanto
***Los objetos deben ser autodescriptivos (incluyendo tipo y tamaño), dentro de unos límites razonables.***
Usar sólo los códigos de tipo y otros números mágicos asignados
asignados por la Autoridad de Asignación de Números de Internet (IANA).
### Coherencia en especificaciones 
Todas las especificaciones deben utilizar la misma terminología y notación, y la misma convención de [[U/Redes/Glosario#Orden de Bytes (Byte Order)|orden de bits y bytes]].

### Condición de estandarización
***Nada se estandariza hasta que existan múltiples instancias de código en ejecución.***
## Cuestiones de nombre y dirección
### No direcciones volatiles o _hardcodeadas_
Evitar cualquier diseño que requiere que las direcciones sean [[U/Redes/Glosario#Hard coded|hard codeadas]] o almacenados en memoria no volátil (excepto cuando es un requerimiento esencial como en un servidor de nombres o configuración). En general, las aplicaciones de usuario deberían utilizar nombres en lugar de direcciones.
### Único tipo de estructura para nombre
Debe utilizarse una única estructura de nomenclatura para el nombre.
### LAs MaYuScUlAs NO ImPOrtan
Se establece que los nombres públicos (que son ampliamente visibles en la red) deben estar en ASCII independiente de mayúsculas y minúsculas, es decir, que no deben ser sensibles a las mayúsculas y minúsculas. Esto significa que el sistema no hará diferencia entre letras mayúsculas y minúsculas. Por ejemplo, "Example.com", "EXAMPLE.COM" y "example.com" serían tratados de la misma manera.

En términos prácticos, esto significa que si estás diseñando un sistema que utiliza nombres de DNS o elementos de protocolo transmitidos en formato de texto, debes asegurarte de que estos nombres o elementos no distingan entre mayúsculas y minúsculas. Es una buena práctica de diseño para garantizar que los sistemas sean robustos y no se vean afectados por variaciones en el uso de mayúsculas o minúsculas.
### No ambigüedad en direcciones
Las direcciones (dentro de una misma red) deben ser no ambiguas (únicos en el [[U/Redes/Glosario#Scope|scope]] en dónde estén). 

### Protocolos de capa superior y endpoints. 

***Es necesario que los protocolos de capa superior sean capaces de identificar los puntos finales de manera inequívoca. En la práctica actual, esto significa que las direcciones deben ser las mismas al inicio y al final de la transmisión.***

En el contexto de las redes, los protocolos de capa superior (como TCP, UDP, HTTP, FTP, etc.) trabajan con direcciones o identificadores que permiten la comunicación entre los puntos finales de una conexión. Para garantizar una comunicación exitosa, es esencial que los puntos finales sean identificados de manera unívoca, lo que significa que la dirección o identificador utilizado al inicio de la transmisión debe ser el mismo al final.

Esto es importante porque las direcciones o identificadores se utilizan para enrutar los paquetes de datos a los puntos finales correctos en la red. Si la dirección o identificador cambia durante la transmisión, puede provocar que los paquetes se enruten incorrectamente o que la comunicación se interrumpa.

## Asuntos externos
### Tecnología no patentada vs. patentada
Es preferible utilizar tecnología no patentada, pero si la mejor tecnología está patentada y está disponible para todos en términos razonables, entonces la incorporación de tecnología patentada es aceptable.

### Controles de exportación
La existencia de controles de exportación sobre algunos aspectos de la tecnología de Internet solo es de importancia secundaria al elegir qué tecnología adoptar en los estándares. Toda la tecnología necesaria para implementar los estándares de Internet puede fabricarse en cada país, por lo que la implementación mundial de la tecnología de Internet no depende de su exportabilidad desde un país o países particulares.

### Conformidad con el estándar
Cualquier implementación que no incluya todos los componentes requeridos no puede reclamar conformidad con el estándar.

### Diseños internacionales y localización
Los diseños deben ser completamente internacionales, con soporte para la localización (adaptación a conjuntos de caracteres locales). En particular, debe haber un enfoque uniforme para etiquetar el conjunto de caracteres para el contenido de la información.

## Confidencialidad y Autenticación

### Ajuste dentro de la arquitectura de seguridad IP
Todos los diseños deben encajar dentro de la arquitectura de seguridad IP.

### Privacidad y autenticidad del tráfico
Es altamente deseable que los proveedores de Internet protejan la privacidad y autenticidad de todo el tráfico, pero esto no es un requisito de la arquitectura. La confidencialidad y autenticación son responsabilidad de los usuarios finales y deben implementarse en los protocolos utilizados por los usuarios finales. Los puntos finales no deben depender de la confidencialidad o integridad de los proveedores. Los proveedores pueden optar por proporcionar algún nivel de protección, pero esto es secundario a la responsabilidad principal de los usuarios finales de protegerse a sí mismos.

### Alternativas de algoritmos criptográficos
Donde se requiera un algoritmo criptográfico en un protocolo, el protocolo debe diseñarse para permitir el uso de algoritmos alternativos, y el algoritmo específico utilizado en una implementación particular debe etiquetarse explícitamente. Las etiquetas oficiales para los algoritmos deben ser registradas por la IANA. (Se puede argumentar que este principio podría generalizarse más allá del área de seguridad).

### Elección de algoritmos
Al elegir algoritmos, se debe seleccionar un algoritmo que sea ampliamente considerado lo suficientemente sólido como para cumplir con su propósito. Entre las alternativas, todas las cuales son lo suficientemente sólidas, se debe dar preferencia a los algoritmos que han resistido la prueba del tiempo y que no son innecesariamente ineficientes.

### Mandato de algoritmo para la interoperabilidad
Para garantizar la interoperabilidad entre puntos finales que utilizan servicios de seguridad, se debe exigir un algoritmo (o conjunto de algoritmos) para asegurar la capacidad de negociar un contexto seguro entre implementaciones. Sin esto, las implementaciones podrían no tener un algoritmo en común y no poder comunicarse de manera segura. 


# Notas
## Cambios importantes en internet
Desde ARPANET, más de 25 años atrás, el internet ha aumentado en factores de mil su velocidad de [[U/Redes/Glosario#Backbone|backbone]] y en factores de millones en el número de dispositivos conectados. 

## Un único protocolo no es el único camino. 
Por supuesto, puede haber múltiples protocolos para satisfacer diferentes requisitos a otros niveles, y hay muchos ejemplos exitosos de grandes redes privadas con múltiples protocolos de capa de red en uso.