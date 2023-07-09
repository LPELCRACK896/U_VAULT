
## Ancho de banda
#caracteristica
Generalmente, se refiere a la capacidad de transmisión de datos en una red, es decir, cuantos datos se puede transferir por un canal determinado periodo de tiempo, comúnmente medido en bits por segundo (bps, Kbps, Mbps, Gbps, etc.) 

## ARPANET
#historia
**Advanced Research Projects Agency Network**
Fue una de las primeras tecnologías de intercambios de paquetes ([[#Paquet Switching]]) dentro de una red de computadoras y la fundación que luego se convertiría el internet moderno. Fue desarrollado por el departamento de defensa de los Estados Unidos y llegó a operaciones en 1969. 

Fue originalmente creado para facilitar la comunicación e intercambio de información entre varios instituciones de investigación y universidades. 

Empleaba una arquitectura de red descentralizada, conectando varios ordenadores y redes mediante tecnología de conmutación de paquetes. Este enfoque permitía dividir los datos en pequeños paquetes y enviarlos a través de múltiples rutas, mejorando la fiabilidad y la eficiencia.

### Un poco más de historia
La red ARPANET inicial constaba de cuatro nodos situados en la Universidad de California, Los Ángeles (UCLA), el Instituto de Investigación de Stanford (SRI), la Universidad de California, Santa Bárbara (UCSB) y la Universidad de Utah. Con el tiempo, se añadieron más nodos y la red se amplió.

ARPANET desempeñó un papel crucial en el desarrollo de tecnologías y protocolos clave de Internet, como TCP/IP (Transmission Control Protocol/Internet Protocol). TCP/IP se convirtió en la base de la Internet moderna, permitiendo a los ordenadores comunicarse entre sí a través de diferentes redes.

En los años 80, ARPANET fue eliminada y sustituida por la National Science Foundation Network (NSFNET), que ofrecía mayor velocidad y conectividad. Sin embargo, el legado de ARPANET sentó las bases de la Internet que utilizamos hoy en día. Su impacto en la investigación, la comunicación y el intercambio de información es incalculable.


## Backbone
#concepto
$\rightarrow$ Troncal o red troncal
Es una de las principales conexiones de internet. Cada troncal está compuesta por un gran número de enrutadores interconectados comerciales, gubernamentales, universitarios y de otra índole de gran capacidad que llevan los datos a través de países, continentes y océanos del mundo mediante cables de fibra óptica.

Parte de la extrema adaptabilidad de internet se debe a su diseño estructural, ubicando las funciones de estado y control en los propios elementos de la red y relegando la mayor parte del procesamiento a los extremos finales. De esta manera se asegura la integridad, la fiabilidad y la autenticidad de los datos.

El término troncal también se refiere al cableado troncal o subsistema vertical en una instalación de red de área local que sigue la normativa de cableado estructurado.
https://es.wikipedia.org/wiki/Backbone
## Cables de par trenzado 
#hardware

En telecomunicaciones, el cable de par trenzado es un tipo de cable que tiene dos conductores eléctricos aislados y entrelazados para anular las interferencias de fuentes externas y diafonía de los cables adyacentes. Fue inventado por Alexander Graham Bell en 1881. 
El cable de par trenzado consiste en grupos de hilos de cobre entrelazados en pares en forma helicoidal. Esto se hace porque dos alambres paralelos constituyen una antena simple. Cuando se entrelazan los alambres helicoidalmente, las ondas se cancelan, por lo que la interferencia producida por los mismos es reducida lo que permite una mejor transmisión de datos.

Así, la forma entrelazada permite reducir la interferencia eléctrica tanto exterior como de pares cercanos y permite transmitir datos de forma más fiable

Existen tipos de cable trenzado. 
- [[#UTP]]
- [[#STP]]
- [[#FTP]]

### UTP
(**Unshielded twisted pair**)
**Cable de par trenzado no blindado.** 
Se trata de uno o varios pares de cables trenzados que no están blindados contra interferencias electromagnéticas. Es de bajo costo y de fácil uso pero produce más errores que otros tipos de cable y tienen limitaciones para trabajar a grandes distancias sin regeneración de la señal. Su [[#Impedancia característica|impedancia característica]] es de 100 ohmios. 

Algunos ejemplos de cables derivados de UTP son: 
- CAT5e
- CAT6

### STP
(**Shielded twisted pair**)
**Cable de par trenzado blindado**
Contiene pares trenzados rodeados cada par de una cubierta protectora de aluminio. Se utiliza en redes con [[#Cable Ethernet|Ethernet]] o Token Ring (¿?). Es una versión más cara que en [[#UTP]] y su [[#Impedancia característica|impedancia característica]] es de 150 ohmios. 

### FTP
(**Foiled twisted pair** )
**Cable por trenzado con pantalla global.** 
Contiene pares trenzados, todos rodeados de una cubierta protectora hecha de aluminio. Similar al [[#STP]] pero este es más utilizado en equipos inalámbricos en exteriores, su [[#Impedancia característica|impedancia característica]] es de 120 ohmios.

## Cable Ethernet
#hardware 

Es una forma de [[#Cables de par trenzado|cable trenzado]] comúnmente utilizado para conectar una computadora a un router, utilizado para transmitir datos a alta velocidad en un contexto [[#LAN]].  

Existen múltiples tipos de cable ethernet, dividido por categorías que tienen distintas capacidades y características.  
1. **Cat5e**
	Este cable admite de hasta 1Gbps y se utiliza comúnmente para redes domésticas y empresariales. Tiene un límite de banda de 100MHz. (Usualmente de tipo [[#UTP]], pero siempre existen verisiones STP por casos con mayor interferencia electromagentica)
2. **Cat6**
	Admite velocidad de hasta 10Gbps para distancias cortas (menor a 55 metros) y tiene un límite de banda de 250MHz. (Es de tipo [[#UTP]])
3. **Cat6a**
	Es una mejora del Cat6 pero para distancias más largas (hasta 100 metros) y tiene un límite de banda de 500 MHz. 


Existen categorías de 

## Cloud Services
#aplicacion
(pendiente)
## Ethernet
#concepto 

https://www.ionos.es/digitalguide/servidores/know-how/ethernet-ieee-8023/#:~:text=Ethernet%20designa%20a%20una%20tecnología,se%20crea%20mediante%20conexiones%20Ethernet.
https://chat.openai.com/share/e4e8abe8-3c93-4bc7-90d9-d6702b03deb5

## IAB
#historia #agrupacion
La IAB, o **Internet Architecture Board**, es una comisión que se encarga de supervisar el desarrollo de la arquitectura de Internet y de sus protocolos asociados. Formada en 1983, la IAB ha desempeñado un papel importante en la dirección de los estándares y protocolos utilizados en Internet.

La IAB se ocupa de varias tareas, incluyendo:

- Supervisión del proceso de desarrollo de estándares de Internet y la aprobación de propuestas de estándares como Estándares de Internet.
- La dirección y gestión de los grupos de trabajo de la IETF (Internet Engineering Task Force) y la IRTF (Internet Research Task Force).
- La representación de la comunidad de Internet en las discusiones sobre política y estándares con otras organizaciones.
## Impedancia característica
(pendiente) https://es.wikipedia.org/wiki/Impedancia_característica
## IPv4
#tecnologia
IPv4 hace referencia al protocolo de internet versión 4. Es la tecnología que permite que los dispositivos se conecten a internet.

## IPv6
#tecnologia

## LAN
#concepto 

## Límite de banda
#concepto 
También llamado **frecuencia** de banda, se refiere a la frecuencia máxima a la que el cable puede transmitir señales de manera efectiva. Se mide en MHz y puede ser un indicador del rendimiento global del cable.  


## Load balance
#tecnica
Load balance o balance de carga hace referencia a la distribución del tráfico en la red estrante a través de un grupo de servicios backend [[#Server Farm]] o [[#Server pool]]. Todo esto con la idea de garantizar mayor disponibilidad y velocidad de un servicio. 

Este es un servicio que podría aplicarse a tecnologías como NGINX. 

## Paquet Switching
Conmutación de paquetes. 
(pendiente)

## Protocolos de internet
(pendiente)

## QoS
#tecnica 
Quality of Service $\rightarrow$ Calidad de servicio. 

Se refiere a la capacidad y de mecanismos y tecnologías implementadas que garantizan ciertos requisitos de rendimiento de la red para ciertos tipos de tráfico de datos.

En términos sencillos, la QoS es como tener un carril preferencial en una autopista para ciertos tipos de tráfico. Por ejemplo, si estás realizando una videollamada (que requiere un flujo de datos constante y en tiempo real para mantener la calidad de la llamada) en una red que también está siendo utilizada para descargar archivos grandes (que pueden absorber gran parte del ancho de banda de la red pero no necesitan un flujo constante), la QoS podría garantizar que la videollamada reciba el ancho de banda que necesita para operar de manera efectiva.

La QoS puede ser especialmente importante en redes donde el ancho de banda es limitado y hay muchos tipos diferentes de tráfico compitiendo por recursos, y puede ser utilizada para priorizar tráfico crítico o sensible a la latencia, garantizar un cierto nivel de rendimiento para ciertos servicios, o limitar el impacto del tráfico no crítico en el rendimiento general de la red

## RJ45
#hardware 
(Es el cable coloquialmente conocido como cable LAN o Ethernet $\rightarrow$ términos relacionados con red pero que no son precisamente el cable)

Es una interfaz física comúnmente utilizada para conectar redes de computadoras con cableado estructurado (5, 5E,  6, 6A, y 8.1). Posee ocho pines o conexiones eléctricas, que normalmente se usan como extremos de [[#Cables de par trenzado|cables de par trenzado]]


## Server Farm
#tecnica #aplicacion 
Una granja de servidores o cluster de servidores es una colección de servidores mantenidos por una organización específica orientados a proporcionar una funcionalidad más allá de la capacidad individual de cada uno. 

Cabe aclarar que una granja de servidores también hace referencia a una gran infraestructura con centenares o hasta miles de servidores interconectados en un mismo espacio físico y con un equipamiento para la red, dispositivos de almacenamiento y otros componentes de infraestructura. (Este segundo párrafo sirve como aclaración de la diferencia con un [[#Server pool]])

Podemos relacionarlo y considerar que son columna vertebral de los [[#Cloud Services]] como AWS. 
[Referencia](https://es.wikipedia.org/wiki/Granja_de_servidores)

## Server pool
#tecnica #aplicacion 
Es una colección de servidores que están disponibles y manejados como un recurso compartido. Puede ser un grupo de servidores físicos o un grupo de máquinas virtuales, controlados o localizados en función para cumplir distintas tareas en una misma aplicación según las necesite. Entre sí, los servidores, pueden o no tener la misma configuración pero la idea es que estén organizadas para trabajar en conjunto de manera eficiente. 

La idea de esto es tener una infraestructura flexible y escalable para gestionar distintas cargas de trabajo, mejorar tolerancia a fallos y simplificar la asignación de recursos. Las principales herramientas para un server pool son virtualizadoras como **VMWare** o **Hyper-V.**   