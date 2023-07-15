
# Ancho de banda
#caracteristica
Generalmente, se refiere a la capacidad de transmisión de datos en una red, es decir, cuantos datos se puede transferir por un canal determinado periodo de tiempo, comúnmente medido en bits por segundo (bps, Kbps, Mbps, Gbps, etc.) 

# ARPANET
#historia
**Advanced Research Projects Agency Network**
Fue una de las primeras tecnologías de intercambios de paquetes ([[#Paquet Switching]]) dentro de una red de computadoras y la fundación que luego se convertiría el internet moderno. Fue desarrollado por el departamento de defensa de los Estados Unidos y llegó a operaciones en 1969. 

Fue originalmente creado para facilitar la comunicación e intercambio de información entre varios instituciones de investigación y universidades. 

Empleaba una arquitectura de red descentralizada, conectando varios ordenadores y redes mediante tecnología de conmutación de paquetes. Este enfoque permitía dividir los datos en pequeños paquetes y enviarlos a través de múltiples rutas, mejorando la fiabilidad y la eficiencia.

## Un poco más de historia
La red ARPANET inicial constaba de cuatro nodos situados en la Universidad de California, Los Ángeles (UCLA), el Instituto de Investigación de Stanford (SRI), la Universidad de California, Santa Bárbara (UCSB) y la Universidad de Utah. Con el tiempo, se añadieron más nodos y la red se amplió.

ARPANET desempeñó un papel crucial en el desarrollo de tecnologías y protocolos clave de Internet, como TCP/IP (Transmission Control Protocol/Internet Protocol). TCP/IP se convirtió en la base de la Internet moderna, permitiendo a los ordenadores comunicarse entre sí a través de diferentes redes.

En los años 80, ARPANET fue eliminada y sustituida por la National Science Foundation Network (NSFNET), que ofrecía mayor velocidad y conectividad. Sin embargo, el legado de ARPANET sentó las bases de la Internet que utilizamos hoy en día. Su impacto en la investigación, la comunicación y el intercambio de información es incalculable.


# Backbone
#concepto
$\rightarrow$ Troncal o red troncal
Es una de las principales conexiones de internet. Cada troncal está compuesta por un gran número de enrutadores interconectados comerciales, gubernamentales, universitarios y de otra índole de gran capacidad que llevan los datos a través de países, continentes y océanos del mundo mediante cables de fibra óptica.

Parte de la extrema adaptabilidad de internet se debe a su diseño estructural, ubicando las funciones de estado y control en los propios elementos de la red y relegando la mayor parte del procesamiento a los extremos finales. De esta manera se asegura la integridad, la fiabilidad y la autenticidad de los datos.

El término troncal también se refiere al cableado troncal o subsistema vertical en una instalación de red de área local que sigue la normativa de cableado estructurado.
https://es.wikipedia.org/wiki/Backbone
# Cables de par trenzado 
#hardware

En telecomunicaciones, el cable de par trenzado es un tipo de cable que tiene dos conductores eléctricos aislados y entrelazados para anular las interferencias de fuentes externas y diafonía de los cables adyacentes. Fue inventado por Alexander Graham Bell en 1881. 
El cable de par trenzado consiste en grupos de hilos de cobre entrelazados en pares en forma helicoidal. Esto se hace porque dos alambres paralelos constituyen una antena simple. Cuando se entrelazan los alambres helicoidalmente, las ondas se cancelan, por lo que la interferencia producida por los mismos es reducida lo que permite una mejor transmisión de datos.

Así, la forma entrelazada permite reducir la interferencia eléctrica tanto exterior como de pares cercanos y permite transmitir datos de forma más fiable

Existen tipos de cable trenzado. 
- [[#UTP]]
- [[#STP]]
- [[#FTP]]

## UTP
(**Unshielded twisted pair**)
**Cable de par trenzado no blindado.** 
Se trata de uno o varios pares de cables trenzados que no están blindados contra interferencias electromagnéticas. Es de bajo costo y de fácil uso pero produce más errores que otros tipos de cable y tienen limitaciones para trabajar a grandes distancias sin regeneración de la señal. Su [[#Impedancia característica|impedancia característica]] es de 100 ohmios. 

Algunos ejemplos de cables derivados de UTP son: 
- CAT5e
- CAT6

## STP
(**Shielded twisted pair**)
**Cable de par trenzado blindado**
Contiene pares trenzados rodeados cada par de una cubierta protectora de aluminio. Se utiliza en redes con [[#Cable Ethernet|Ethernet]] o Token Ring (¿?). Es una versión más cara que en [[#UTP]] y su [[#Impedancia característica|impedancia característica]] es de 150 ohmios. 

## FTP
(**Foiled twisted pair** )
**Cable por trenzado con pantalla global.** 
Contiene pares trenzados, todos rodeados de una cubierta protectora hecha de aluminio. Similar al [[#STP]] pero este es más utilizado en equipos inalámbricos en exteriores, su [[#Impedancia característica|impedancia característica]] es de 120 ohmios.

# Cable Ethernet
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

# CMTS
CMTS significa "Cable Modem Termination System" (Sistema de Terminación de Módem por Cable, en español). Es un componente de hardware que se utiliza en las redes de cable para proporcionar servicios de banda ancha, como el acceso a Internet.

El CMTS se sitúa en la central del proveedor de servicios de cable, y actúa como un enlace entre los módems de cable de los usuarios (ubicados en hogares o empresas) y la red de datos del proveedor de servicios de Internet (ISP).

El CMTS recibe las señales digitales que vienen de los módems de cable de los usuarios a través de la infraestructura de cable coaxial y las convierte en una señal de Internet que puede ser enviada a través de la red de datos del ISP. A la inversa, también toma datos de Internet del ISP y los convierte en una señal que puede ser enviada a través de la infraestructura de cable coaxial a los módems de cable de los usuarios.

En resumen, un CMTS permite que los módems de cable de los usuarios se conecten a Internet a través de la infraestructura de cable coaxial.
# Cloud Services
#aplicacion
(pendiente)
# DSL 
DSL, que significa "Digital Subscriber Line" (Línea de Suscriptor Digital, en español), es una tecnología de comunicación que se utiliza para transmitir datos digitales a través de las líneas telefónicas tradicionales. DSL es un tipo de conexión de banda ancha, que proporciona una conexión a Internet de alta velocidad.

Existen varios tipos de DSL, entre ellos ADSL (Asymmetric Digital Subscriber Line), que es la más común. El "asimétrico" se refiere a cómo la velocidad de datos de descarga (desde Internet a tu computadora) es más rápida que la velocidad de subida (desde tu computadora a Internet). Otros tipos de DSL incluyen SDSL (Symmetric Digital Subscriber Line), VDSL (Very high bitrate Digital Subscriber Line) y otros.

Uno de los beneficios clave de DSL es que puede funcionar a través de la infraestructura de línea telefónica existente en muchas áreas, por lo que a menudo está disponible en lugares donde otras opciones de Internet de alta velocidad no lo están. Sin embargo, la velocidad de DSL puede ser limitada por la distancia física entre la ubicación del usuario y la central telefónica.
# DSLAM
DSLAM significa "Digital Subscriber Line Access Multiplexer" (Multiplexor de Acceso a Línea de Suscriptor Digital, en español). Es un dispositivo de red que recibe las señales de múltiples conexiones DSL de los clientes y las pone en una sola línea de alta capacidad para enviarlas a Internet.

En un nivel alto, puedes pensar en un DSLAM como un concentrador que recopila las conexiones a Internet de muchos usuarios individuales y las combina en un enlace de Internet más grande y más rápido.

Los DSLAM son un componente crítico de las redes de telecomunicaciones porque permiten a los proveedores de servicios de Internet (ISP) manejar la gran cantidad de conexiones de los clientes. Normalmente, un DSLAM se encuentra en la central telefónica del proveedor de servicios, y conecta las líneas individuales de los clientes con la red troncal del proveedor. 

Cada línea DSL conectada al DSLAM tiene su propia conexión a Internet, lo que significa que los usuarios no compiten entre sí por el ancho de banda, al contrario de lo que sucede con algunas otras tecnologías de Internet compartidas. Sin embargo, el rendimiento total del DSLAM sí limita la cantidad de datos que todos los usuarios conectados pueden transmitir colectivamente en un momento dado.
# Ethernet
#concepto 

https://www.ionos.es/digitalguide/servidores/know-how/ethernet-ieee-8023/#:~:text=Ethernet%20designa%20a%20una%20tecnología,se%20crea%20mediante%20conexiones%20Ethernet.
https://chat.openai.com/share/e4e8abe8-3c93-4bc7-90d9-d6702b03deb5

# FTTH
Fiber to the home. 
La fibra hasta el hogar (**FTTH**), también llamada fibra hasta las instalaciones (FTTP), es la instalación y el uso de fibra óptica desde un punto central directamente a edificios individuales como residencias, edificios de apartamentos y empresas para proporcionar acceso a internet de alta velocidad.
# GNSS
GNSS son las siglas de Sistema de Navegación Global por Satélite (Global Navigation Satellite System, en inglés). Es un sistema de posicionamiento y navegación que utiliza señales emitidas por satélites para determinar la ubicación precisa de receptores en la Tierra. El GNSS permite a los receptores determinar su posición, velocidad y tiempo en cualquier lugar del mundo, siempre y cuando tengan acceso a las señales de los satélites.

El sistema GNSS más conocido y utilizado es el Sistema de Posicionamiento Global (GPS, por sus siglas en inglés), desarrollado por el Departamento de Defensa de los Estados Unidos. Sin embargo, existen otros sistemas GNSS operativos o en desarrollo, como el GLONASS (Rusia), Galileo (Unión Europea) y BeiDou (China).

Estos sistemas GNSS utilizan una constelación de satélites en órbita alrededor de la Tierra que transmiten señales de tiempo y posición. Los receptores GNSS reciben estas señales y las utilizan para calcular su ubicación mediante el trilateración, que consiste en medir la distancia entre el receptor y varios satélites para determinar la posición exacta.

El GNSS tiene una amplia variedad de aplicaciones, desde la navegación en dispositivos móviles, sistemas de navegación de vehículos y aviones, hasta aplicaciones en la agricultura, la topografía, la geodesia y la gestión de flotas. También es utilizado en aplicaciones de rescate y emergencias, así como en la sincronización de redes de comunicaciones y sistemas de control de tiempo.

# Hard coded
a

# IAB
#historia #agrupacion
La IAB, o **Internet Architecture Board**, es una comisión que se encarga de supervisar el desarrollo de la arquitectura de Internet y de sus protocolos asociados. Formada en 1983, la IAB ha desempeñado un papel importante en la dirección de los estándares y protocolos utilizados en Internet.

La IAB se ocupa de varias tareas, incluyendo:

- Supervisión del proceso de desarrollo de estándares de Internet y la aprobación de propuestas de estándares como Estándares de Internet.
- La dirección y gestión de los grupos de trabajo de la IETF (Internet Engineering Task Force) y la IRTF (Internet Research Task Force).
- La representación de la comunidad de Internet en las discusiones sobre política y estándares con otras organizaciones.
# Impedancia característica
(pendiente) https://es.wikipedia.org/wiki/Impedancia_característica
# IPv4
#tecnologia
IPv4 significa "Protocolo de Internet versión 4". Es la tecnología  que permite que los dispositivos se conecten a Internet. Un esquema de direccionamiento de **32 bits** que permite un total de 2^32 direcciones (aprox. 4.3 mil millones) Cada dispositivo necesita una dirección IP única. 

Una dirección IPv4 se compone típicamente de cuatro octetos, cada uno de los cuales consta de 8 bits, separada por puntos. (Con 8 bits se pueden representar del 0 al 255, 256 números, 2^8)

\[0-255].\[0-255]. \[0-255].\[0-255] 

Existe una estructura más detallada que divide la IP en los siguientes elementos: 
- **Identificador de red**: Este es el primer componente de una dirección IP y designa la red específica a la que pertenece la dirección.
    
- **Identificador de host**: Este es el segundo componente de una dirección IP y designa el dispositivo específico (o "host") en la red a la que se refiere la dirección.
    
- **Clases de redes**: Las direcciones IPv4 se dividen en cinco clases (A, B, C, D, y E) en función de su primer octeto. Las clases A, B y C se utilizan para redes de diferente tamaño, la clase D se utiliza para multidifusión y la clase E se reserva para uso futuro o investigación. Las clases A, B y C tienen diferentes longitudes para los identificadores de red y host.
    
- **Subredes**: En muchos casos, las direcciones de red se dividen aún más en "subredes". Esta es una manera de crear divisiones lógicas dentro de una red física para mejorar la eficiencia y la seguridad.
    
- **Direcciones especiales**: Algunas direcciones IP tienen significados especiales. Por ejemplo, la dirección 127.0.0.1 siempre se refiere al host local (también conocido como "localhost"). Las direcciones que comienzan con 192.168. son para redes privadas.
    
- **Máscara de subred**: Es un número que se utiliza para determinar la porción de la dirección IP que indica la red/subred y la porción que indica el host. Normalmente se muestra como cuatro octetos, al igual que una dirección IP. Por ejemplo, una máscara de subred común para una red de clase C es 255.255.255.0.
# IPv6
#tecnologia
IPv6, que significa "Protocolo de Internet versión 6", es la versión más reciente del protocolo IP, diseñado para reemplazar a IPv4 debido a su limitada cantidad de direcciones únicas.

IPv6 utiliza un esquema de direccionamiento de **128 bits**, que ofrece una cantidad enormemente mayor de direcciones únicas (2^128) en comparación con IPv4. Esto es especialmente importante a medida que más y más dispositivos se conectan a Internet.

A diferencia de las direcciones IPv4, que se dividen en cuatro octetos y se representan en decimal, las direcciones IPv6 se dividen en ocho grupos de cuatro caracteres hexadecimales, separados por dos puntos. Un ejemplo de una dirección IPv6 podría ser 2001:0db8:85a3:0000:0000:8a2e:0370:7334.

Los elementos clave de una dirección IPv6 incluyen:

- **Campo global/local**: El bit más significativo de la dirección determina si la dirección es global (accesible en Internet) o local (sólo se utiliza en una red local).
    
- **Campo de identificador de subred**: Este campo se utiliza para la asignación de subredes dentro de una organización. Puede ser de longitud variable, aunque el valor típico es 64 bits.
    
- **Campo de identificador de interfaz**: Este campo se utiliza para identificar una interfaz única en una subred. Al igual que con el campo de identificador de subred, puede ser de longitud variable, pero el valor típico es 64 bits.
    
- **Direcciones especiales**: Al igual que con IPv4, existen varias direcciones especiales en IPv6. Por ejemplo, la dirección ::1 es el equivalente a la dirección localhost en IPv4 (127.0.0.1). Las direcciones que comienzan con fe80:: son direcciones de enlace local, utilizadas para la comunicación en una red local.
    

Además, IPv6 introduce varios nuevos conceptos y características, incluyendo:

- **Autoconfiguración de dirección**: IPv6 permite a los dispositivos configurar automáticamente su propia dirección IP sin necesidad de un servidor DHCP.
    
- **Soporte integrado para encriptación y autenticación**: A diferencia de IPv4, IPv6 tiene soporte integrado para el Protocolo de Seguridad IP (IPSec), lo que puede mejorar la seguridad de la red.
    
- **Multicast**: Mientras que IPv4 utiliza tanto la difusión (broadcast) como la multidifusión (multicast), IPv6 elimina el uso de la difusión y se basa en su lugar en la multidifusión, que permite enviar paquetes a múltiples destinatarios con una única transmisión.
    
- **No hay fragmentación en los nodos intermedios**: En IPv4, los routers intermedios podrían fragmentar paquetes si eran demasiado grandes para el siguiente enlace. En IPv6, la fragmentación se maneja en los extremos de la comunicación, no en los nodos intermedios, lo que simplifica el procesamiento en los routers y mejora la eficiencia de la red.
# ISP
Internet Service Provider 

ISP significa "Internet Service Provider" (Proveedor de Servicios de Internet, en español). Un ISP es una compañía que proporciona servicios de acceso a Internet a los usuarios finales o a otros servidores. Dependiendo de la naturaleza y el tamaño de un ISP, este puede ser a nivel local, regional o nacional.

Los ISP pueden ofrecer Internet a través de varias tecnologías, como DSL, cable, fibra óptica, satélite, o incluso conexiones inalámbricas. Los servicios proporcionados por los ISP pueden incluir la conectividad a Internet, la creación y el alojamiento de sitios web, el alojamiento de correo electrónico y muchos otros servicios relacionados con la Internet.

Los ISP son esenciales para conectar a los usuarios de Internet con la infraestructura de la red mundial. Cuando te conectas a Internet, tu computadora se comunica con los servidores y las máquinas de tu ISP, el cual a su vez te conecta a la red más amplia de Internet.

# IXP 
IXP se refiere a "Internet Exchange Point" (Punto de Intercambio de Internet, en español). Un IXP es una infraestructura física a través de la cual los proveedores de servicios de Internet (ISPs) e incluso algunas grandes redes privadas, como las de las universidades y corporaciones, intercambian tráfico de Internet entre sus redes.

El propósito principal de un IXP es permitir que las redes se conecten directamente entre sí, en lugar de a través de una o más redes de terceros. Esto se traduce en un tráfico de Internet más rápido y eficiente, ya que reduce la distancia que los paquetes de datos necesitan viajar. Los IXP también pueden mejorar la resistencia de la red al proporcionar rutas de conexión alternativas en caso de fallos en otras partes de la red.

Los IXP suelen ser operados por terceros y se localizan en puntos con alta densidad de tráfico de red, a menudo en grandes centros de datos. Los miembros del IXP, que pueden ser ISPs, grandes empresas, proveedores de contenido y otras redes, se conectan al IXP y acuerdan intercambiar ciertos tipos de tráfico.

En resumen, los IXP son una parte crucial de la infraestructura de Internet, ya que permiten que el tráfico de Internet se transmita de manera más eficiente y fiable.
# LAN
#concepto 

# Límite de banda
#concepto 
También llamado **frecuencia** de banda, se refiere a la frecuencia máxima a la que el cable puede transmitir señales de manera efectiva. Se mide en MHz y puede ser un indicador del rendimiento global del cable.  


# Load balance
#tecnica
Load balance o balance de carga hace referencia a la distribución del tráfico en la red estrante a través de un grupo de servicios backend [[#Server Farm]] o [[#Server pool]]. Todo esto con la idea de garantizar mayor disponibilidad y velocidad de un servicio. 

Este es un servicio que podría aplicarse a tecnologías como NGINX. 

# Orden de Bytes (Byte Order)

El **orden de bytes** es el orden en que se almacenan y se representan los bytes de datos multi-byte, como los enteros de 32 bits y los números de punto flotante. Dependiendo del protocolo o la arquitectura del hardware, los bytes pueden ser leídos de izquierda a derecha (el orden más significativo primero), lo que se conoce como **Big Endian**, o de derecha a izquierda (el orden menos significativo primero), lo que se conoce como **Little Endian**.

## Big Endian

En la representación de Big Endian, el byte más significativo (MSB) se almacena en la dirección de memoria más baja. Por ejemplo, si tenemos un entero de 32 bits representado por los bytes 12 34 56 78, en Big Endian se almacenará de la misma manera: 12 34 56 78.

Ventajas de usar Big Endian:

- Facilita la comparación de números enteros.
- Es más intuitivo para la representación y visualización humanas.

Desventajas de usar Big Endian:

- Puede causar problemas al trabajar con arquitecturas que usan Little Endian.

## Little Endian

En la representación de Little Endian, el byte menos significativo (LSB) se almacena en la dirección de memoria más baja. Siguiendo el mismo ejemplo anterior, en Little Endian se almacenará de la manera opuesta: 78 56 34 12.

Ventajas de usar Little Endian:

- Las operaciones de suma y resta pueden ser un poco más eficientes.
- Es el formato estándar en las computadoras basadas en x86.

Desventajas de usar Little Endian:

- Menos intuitivo para la representación y visualización humanas.

## Ejemplos de uso

La mayoría de las arquitecturas de computadoras utilizan uno de estos dos esquemas. Las arquitecturas Intel x86 y x86_64 son Little Endian, mientras que las viejas arquitecturas Motorola eran Big Endian. ARM soporta ambos modos, lo cual puede cambiarse durante el tiempo de ejecución. En redes de comunicación, el protocolo de Internet (IP) utiliza Big Endian para transmitir direcciones y otros datos.

# OSI
El modelo OSI (Open Systems Interconnection), o modelo de Interconexión de Sistemas Abiertos, es un marco conceptual que estandariza las funciones de un sistema de comunicaciones o red de computadoras en siete categorías, llamadas capas. Este modelo fue desarrollado por la Organización Internacional de Normalización (ISO) en 1984 para facilitar la interconexión de sistemas informáticos.

Las siete capas del modelo OSI, de la capa más baja a la más alta, son las siguientes:

1. **Capa Física**: Esta capa se ocupa de las características físicas de la transmisión de datos, como los medios de transmisión, la topología de la red, el tipo de señal, etc.

2. **Capa de Enlace de Datos**: Esta capa establece, mantiene y libera conexiones de enlace de datos entre nodos. También maneja el acceso al medio y detecta errores que pueden ocurrir en la capa física.

3. **Capa de Red**: Esta capa se encarga del direccionamiento, enrutamiento y (en algunas arquitecturas de red) control del flujo de datos. Esta capa determina la ruta que los datos deben seguir desde su origen hasta su destino.

4. **Capa de Transporte**: Esta capa asegura que los mensajes se entreguen en el orden correcto y sin errores. Se ocupa de la detección y corrección de errores.

5. **Capa de Sesión**: Esta capa establece, gestiona y termina las conexiones entre las aplicaciones en cada extremo de la sesión de comunicación.

6. **Capa de Presentación**: Esta capa se ocupa de la representación de la información, la codificación y la compresión de los datos. Asegura que los datos que envía una máquina puedan ser leídos por la máquina que los recibe.

7. **Capa de Aplicación**: Esta es la capa que interactúa directamente con el software o aplicación. Esta capa se ocupa de protocolos de alto nivel y aspectos relacionados con la presentación de la información para el usuario.

Cada capa tiene una función específica en el proceso de comunicación y prepara la información antes de pasarla a la próxima capa. Al dividir las comunicaciones en capas, el modelo OSI ayuda a entender cómo las redes de computadoras operan y cómo los diferentes componentes de una red interactúan entre sí.
# Paquet Switching
Conmutación de paquetes. 
(pendiente)

# POP
Point of prescense
Punto de presencia. 
Un POP es un punto de acceso o ubicación física que permite a los usuarios conectarse a Internet con los proveedores de servicios de Internet (ISP). Este punto de presencia contiene varios equipos de red como servidores, enrutadores, conmutadores de red, y sistemas DSLAM, entre otros.

Los ISPs establecen POPs en diferentes ubicaciones geográficas, dependiendo de dónde estén sus clientes. Por ejemplo, un ISP puede tener varios POPs en una ciudad para proporcionar un acceso más amplio y estable a sus servicios de Internet para los clientes de esa área.

Un ISP también podría tener POPs en varias ciudades o países, lo que permite a la empresa proporcionar servicios a una mayor cantidad de clientes. Además, los POPs a menudo se encuentran en centros de datos, que proporcionan un entorno controlado para el equipo de red.
# Protocolos de internet
(pendiente)

# QoS
#tecnica 
Quality of Service $\rightarrow$ Calidad de servicio. 

Se refiere a la capacidad y de mecanismos y tecnologías implementadas que garantizan ciertos requisitos de rendimiento de la red para ciertos tipos de tráfico de datos.

Es un estándar/acuerdo para un servicio de transmisión de datos en la calidad donde se contempla la minimización de paquetes perdidos. 

En términos sencillos, la QoS es como tener un carril preferencial en una autopista para ciertos tipos de tráfico. Por ejemplo, si estás realizando una videollamada (que requiere un flujo de datos constante y en tiempo real para mantener la calidad de la llamada) en una red que también está siendo utilizada para descargar archivos grandes (que pueden absorber gran parte del ancho de banda de la red pero no necesitan un flujo constante), la QoS podría garantizar que la videollamada reciba el ancho de banda que necesita para operar de manera efectiva.

La QoS puede ser especialmente importante en redes donde el ancho de banda es limitado y hay muchos tipos diferentes de tráfico compitiendo por recursos, y puede ser utilizada para priorizar tráfico crítico o sensible a la latencia, garantizar un cierto nivel de rendimiento para ciertos servicios, o limitar el impacto del tráfico no crítico en el rendimiento general de la red

# RFC
Siglas para **Request For Comments**
Es un documento formal de *Internet Engineering Task Force (IETF)* que contiene las especificaciones y notas organizacionales sobre temas relacionados a internet y redes de computadoras tal como enrutamiento 
# RJ45
#hardware 
(Es el cable coloquialmente conocido como cable LAN o Ethernet $\rightarrow$ términos relacionados con red pero que no son precisamente el cable)

Es una interfaz física comúnmente utilizada para conectar redes de computadoras con cableado estructurado (5, 5E,  6, 6A, y 8.1). Posee ocho pines o conexiones eléctricas, que normalmente se usan como extremos de [[#Cables de par trenzado|cables de par trenzado]]


# Server Farm
#tecnica #aplicacion 
Una granja de servidores o cluster de servidores es una colección de servidores mantenidos por una organización específica orientados a proporcionar una funcionalidad más allá de la capacidad individual de cada uno. 

Cabe aclarar que una granja de servidores también hace referencia a una gran infraestructura con centenares o hasta miles de servidores interconectados en un mismo espacio físico y con un equipamiento para la red, dispositivos de almacenamiento y otros componentes de infraestructura. (Este segundo párrafo sirve como aclaración de la diferencia con un [[#Server pool]])

Podemos relacionarlo y considerar que son columna vertebral de los [[#Cloud Services]] como AWS. 
[Referencia](https://es.wikipedia.org/wiki/Granja_de_servidores)

# Server pool
#tecnica #aplicacion 
Es una colección de servidores que están disponibles y manejados como un recurso compartido. Puede ser un grupo de servidores físicos o un grupo de máquinas virtuales, controlados o localizados en función para cumplir distintas tareas en una misma aplicación según las necesite. Entre sí, los servidores, pueden o no tener la misma configuración pero la idea es que estén organizadas para trabajar en conjunto de manera eficiente. 

La idea de esto es tener una infraestructura flexible y escalable para gestionar distintas cargas de trabajo, mejorar tolerancia a fallos y simplificar la asignación de recursos. Las principales herramientas para un server pool son virtualizadoras como **VMWare** o **Hyper-V.**   

# Scope
Ser refiere al alcance o ámbito de una determinada configuración o conjunto de parámetros en una red. El scope se utiliza para definir los límites y las restricciones de una configuración específica, lo que permite establecer qué dispositivos o recursos están incluidos o excluidos dentro de ese alcance.

El concepto de scope es ampliamente utilizado en la configuración de direcciones IP en redes TCP/IP. En este caso, un scope define un rango de direcciones IP disponibles para ser asignadas a dispositivos dentro de una red. El administrador de red puede configurar múltiples scopes para segmentar una red en subredes más pequeñas y asignar diferentes rangos de direcciones IP a cada una de ellas.

Además de las direcciones IP, el scope también puede referirse a otras configuraciones de red, como las reglas de firewall, las políticas de acceso, las configuraciones de enrutamiento, las asignaciones de puertos, etc. Cada una de estas configuraciones puede tener su propio scope, definiendo qué dispositivos o servicios están afectados por dicha configuración.

# VPN
VPN significa "Virtual Private Network" (Red Privada Virtual, en español). Es una tecnología que permite a los usuarios crear una conexión segura y encriptada a otra red a través de Internet.

Las VPNs se utilizan comúnmente para acceder a recursos de red de una empresa de forma segura mientras se trabaja de forma remota, para proteger los datos mientras se utiliza una red Wi-Fi pública no segura, o para enmascarar la ubicación geográfica del usuario y así poder acceder a contenidos que están geográficamente restringidos.

Una VPN enmascara tu dirección IP, lo que hace que parezca que tu conexión a Internet proviene del servidor VPN en lugar de tu propia ubicación. Esto no sólo puede proporcionar más privacidad, sino que también puede permitirte eludir las restricciones geográficas en ciertos sitios web o servicios.

Las VPNs funcionan encriptando tus datos antes de que salgan de tu dispositivo. Estos datos encriptados viajan luego a través de Internet hasta el servidor VPN, donde son descifrados antes de ser enviados a su destino final. Este proceso también ocurre en sentido inverso para los datos que vienen a tu dispositivo. Este nivel de encriptación puede ayudar a proteger tus datos de ser interceptados y leídos por personas no autorizadas.
