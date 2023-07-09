
Link de referencia: 
[RFC 1958 (Architectural Principles of the Internet)](https://datatracker.ietf.org/doc/html/rfc1958)

# Status 
El documento se presenta a sí como un memo que provee información de la *comunidad de internet* (sin entrar en formalidades, ni estándares como tal).

# Resumen
El internet y su arquitectura crecieron desde modestos inicios en lugar de un *gran plan*; lo que lo trajo a todo lo que es ahora fue un proceso de evolución. Mismo que hizo una gran tecnología de éxito, sin embargo, resulta útil tener un recórd (snapshot) de los **principios del internet**. Motivo por el cual este artículo no se molesta en intentar definirlo con principios tan rígidos, y más bien busca ser una guía general. 
# Contenido 

## Cambio constante
Como buen representante de la industria tecnológica, el internet se mantiene en un constante cambio de sus principios. Comenzando de sus inicios más humildes ([ARPANET](https://developer.mozilla.org/es/docs/Glossary/Arpanet)) a la actualidad, se denota ha sufrido [[R Architectural Principles of the Internet - Tarea 1 lectura de RFC 1958#Cambios importantes en internet|cambios]] que inevitablemente afectan directamente los principios de su arquitectura. Tan drásticamente que principios del pasado que parecían irrevocables fueron depreciados y lo más seguro es que pase lo mismo con los "principios actuales". Entre todos, el único principio que parece prevalecer es el de **cambio constante**

Por tanto, el objetivo del documento no es presentar un dogma de como se debe diseñar los [[U/Redes/Glosario#Protocolos de internet|protocolos de internet]] o siquiera como deben convivir. La idea es brindar una guía de diseños que han funcionado en el pasado y que valen la pena revisar ya sea para utilizarlos o para evaluarlos. 

Algunos puntos de interés que podrían impulsar cambios en el internet son: 
1. **Límites de escalabilidad para [[U/Redes/Glosario#IPv4|IPv4]]**
	IPv4 significa "Protocolo de Internet versión 4". Es la tecnología que permite que los dispositivos se conecten a Internet. Cada dispositivo necesita una dirección IP única, pero IPv4 tiene un número limitado de direcciones, aproximadamente 4.3 mil millones. Con el creciente número de dispositivos que acceden a Internet, nos estamos quedando sin direcciones únicas. Esta limitación es un motor importante para la adopción de la próxima versión, IPv6, que ofrece un número de direcciones posibles mucho mayor.
2. **Las redes de gigabit por segundo y el multimedia**
	Con el auge de las redes de alta velocidad capaces de transmitir datos a velocidades de gigabit por segundo, así como la proliferación de multimedia (audio, video, VR, etc.) en Internet, hay mucha presión sobre las redes y los protocolos de Internet para manejar este tráfico de alto volumen y alto ancho de banda de manera eficiente. Esto ha impulsado la investigación y el desarrollo de nuevas formas de administrar el tráfico de red.
3. **Necesidad de Calidad de Servicio (QoS) y garantías de seguridad en Internet comercial.** 
	Con el papel vital de Internet en el comercio, existe una creciente necesidad de [[U/Redes/Glosario#QoS|QoS]], que asegura que ciertos tipos de datos (como VoIP, videoconferencias, etc.) tengan prioridad y se transmitan de manera confiable. Además, dada la creciente frecuencia y sofisticación de los ciberataques, también están en alta demanda las características y protocolos de seguridad mejorados.

**"Las máquinas voladoras más pesadas que el aire son imposibles"**

La cita del Lord Kelvin y la siguiente declaración enfatizan la necesidad de humildad y flexibilidad frente a los avances científicos y tecnológicos. Kelvin, un famoso científico de su tiempo, afirmó famosamente que , poco antes de que los exitosos vuelos de los hermanos Wright demostraran que estaba equivocado. El autor de este pasaje sugiere que, aunque los principios que han descrito proporcionan una comprensión actual del campo, no deben considerarse absolutos o inmutables. La ciencia y la tecnología están en constante evolución, y nuestra comprensión y mejores prácticas deberán evolucionar también.

## Existe una arquitectura del internet
Muchos pueden decir que en el internet no existe una arquitectura tal cual si no una **tradición** no escrita por los primeros veinticinco años (al menos no por [[U/Redes/Glosario#IAB|IAB]])
# Notas
## Cambios importantes en internet
Desde ARPANET, más de 25 años atrás, el internet ha aumentado en factores de mil su velocidad de [[U/Redes/Glosario#Backbone|backbone]] y en factores de millones en el número de dispositivos conectados. 