#tarea
# Miembros
- Esteban Aldana
- Mariano Reyes
- Andrea Lam
- Kenneth Gálvez
- Jessica Ortiz
- Luis Pedro Gonzalez
- Juan Carlos Bajan 
# Descripción
Armando el contenido del curso en grupos. Eliminando y/o sugiriendo temas para el programa. 

# Revisión de planes anteriores y el plan actual

## 2021
### Bases
**¿Qué es la Ciencia de datos?** 
La ciencia de datos es un área de trabajo emergente relacionada con la recopilación,  
preparación, análisis, visualización, administración y reserva de grandes colecciones de información” [[#Big data and data science What should we teach?|(Song & Zhu,  2016)]]

# Ideas sueltas

## Web scrapping

Referenciando [[#Big data and data science What should we teach?]] 

Sobre el trabajo de los científicos de datos: "1) They focus on extracting actionable knowledge
from data to solve business problems"

Por tanto, creo que sería de interés añadir temas orientados a la recolección de datos, y no solamente utilizar .csv como fuente. Sugiero pinceladas en como hacer requests a APIs y la trata de esa data y webscrapping para obtener data directamente de algunos sitios. 

## Map reduce hadoop --> Dask

Es un tema importante pero que se complica dado que tiene sus principales funciones en Java directamente, y es conveniente tener el curso en un mismo lenguaje. Una alternativa con funcionalidades similares es Dask. Por tanto esto mismo se aplicará. 

## Temas redundantes
Algunos de los temas no tan relevantes o repetitivos fueron omitidos para la propuesta final del programa del curso. 


# Bibliografías
## Big data and data science: What should we teach?
[Song, Il-Yeol & Zhu, Yongjun. (2015). Big data and data science: What should we teach?. Expert Systems. 33. 10.1111/exsy.12130.](https://www.researchgate.net/publication/282692841_Big_data_and_data_science_What_should_we_teach)



# Propuesta final 

## Resumen - Propuesta de curso 
1. [[#Introducción a la ciencia de datos (0.5 semana)]]
2. [[#Visualización de datos (1.5 semanas)]] 
3. [Aprendizaje automático (2 semanas)](#aprendizaje-automático)
4. [Formas alternativas de extracción de datos (3 semanas)](#formas-alternativas-de-extracción-de-datos)
5. [Aprendizaje profundo y redes neuronales (2.5 semanas)](#aprendizaje-profundo-y-redes-neuronales) 
6. [Procesamiento del lenguaje natural (PLN) (4 semanas)](#procesamiento-del-lenguaje-natural-pln)
7. [Big data y conmutación distribuida (2 semanas)](#big-data-y-conmutación-distribuida) 
8. [Ética y privacidad en la ciencia de datos (0.5 semanas)](#ética-y-privacidad-en-la-ciencia-de-datos)

## Propuesta de curso 
### Introducción a la ciencia de datos (0.5 semana)
Con el objetivo de que todos los estudiantes entiendan las bases de la ciencia de los datos es fundamental que se plantee exactamente qué es y cuál es su objetivo. Así como herramientas de apoyo en el análisis de datos que provee la estadística. 
**Temas sugeridos:**
- ¿Qué es la ciencia de datos?
- El proceso de la ciencia de datos (ciclo de vida)
- Análisis Exploratorio 
- Técnicas de estadística descriptiva e inferencial. 
**Tiempo: 0.5 semana** 
### Visualización de datos (1.5 semanas)
La visualización de datos es fundamental para la presentación de resultados y análisis de datos. Sin embargo es un tema muy sencillo y de fácil aprendizaje individual, por lo que creo que es un tema que se debe ver desde fuera, mostrando las herramientas más famosas para la presentación de datos como PowerBi, Tableau y demás, muy por encima e incursionar en mostrar herramientas que son realmente útiles para la vida laboral como los principios para presentar dashboards y métodos de graficación compleja. 
**Temas sugeridos:**
- Bibliotecas de visualización de datos (Matplotlib, Seaborn)
- Principios de visualización de datos 
- Técnicas y herramientas de visualización 
- Visualizaciones interactivas y dinámicas 
- Visualización de datos de alta dimensionalidad
- Herramientas adicionales: PowerBI o Tableau.
**Tiempo: 1.5 semanas** 
### Aprendizaje automático (2 semanas)
Por parte de la carrera de ciencias de la computación, el semestre anterior, tuvimos dos clases en donde aprendimos acerca del aprendizaje automático y los modelos por lo que no es un tema en el que se debería indagar mucho, sin embargo creo que hacer un resumen rápido de todo lo que se vió puede ser valioso. Quizás sea muy valioso hablar sobre herramientas online que puedan ser de gran utilidad para los modelos dado que ahora la mayoría de empresas necesitan modelos que puedan responder a tiempo real y, si se logran utilizar las herramientas online que existen actualmente en el mercado, se enriquecen los conocimientos y habilidades. 
**Temas sugeridos:** 
- Herramientas online de aprendizaje automático 
- Evaluación y validación de modelos
- Selección e ingeniería de características 
**Tiempo: 2 semanas** 
### Formas alternativas de extracción de datos (3 semanas)
Con el objetivo de expandir las fuentes de datos que se manejan, se propone incluir temas de uso de API 's y Web Scraping como métodos de obtención de datos a través de la web. Brindando valiosa información de lugares en donde no es suele ser tan fácilmente alcanzable descargar un dataset de datos. Esto también nos permitirá manejar información más real y que está siendo utilizada por las páginas web. 
**Temas sugeridos:**
- Datos a través de API 's.
	- API, métodos HTTP, códigos HTTP, formato JSON. Breve descripción. 
	- APIs REST y SOAP: Breve explicación de estos dos tipos comunes de APIs. Especial énfasis en API REST. 
	- Autenticación en APIs: OAuth, API keys, tokens, etc. Este es un tema crucial ya que muchas APIs requieren algún tipo de autenticación. Creo que es difícil poder hacer un ejercicio de esto pero se puede explicar como una situación común. 
	- Revisión del resultado en Postman. Herramienta de apoyo en 
	- Librería requests (python) 
	- Librería 'json' (python): Utilizada para manejar datos JSON en Python. 
	- Formatos de respuesta. 
	- Transformación de la información.
- Web Scraping 
	- Librerías de python request (para obtener página) y BeautifulSoup (para extraer información de la página). 
	- Manejo de paginación y navegación a través de enlaces: Las páginas web a menudo tienen datos distribuidos en múltiples páginas.
	- Transformación de la data.
	- Uso de Selenium para interactuar con la página web: Algunas páginas necesitan interacciones como hacer clic en un botón o llenar un formulario para mostrar ciertos datos. 
	- Ética y aspectos legales de web scraping. 
	- Robots.txt: Este archivo le dice a los rastreadores de la web qué partes de un sitio web deben evitar, es importante para entender las limitaciones del web scraping en un sitio específico. 
	- Manejo de bloqueos y CAPTCHAs: Muchas páginas web tienen medidas de seguridad para prevenir el web scraping, por lo que puede ser útil hablar sobre cómo manejar estas situaciones. 
**Tiempo: 3 semanas** 
### Aprendizaje profundo y redes neuronales (2.5 semanas) 
De nuevo, por parte de la carrera de ciencias de la computación, hay una clase dedicada única y solamente al deep learning y redes neuronales por lo que incursionar a detalle sobre este tema serán esfuerzos desperdiciados por lo que podría ser mucho más valioso tomar el punto de vista mencionado con el aprendizaje automático. Cómo utilizar el aprendizaje profundo y redes neuronales con las herramientas que existen actualmente en el mercado. Cómo encontrar los casos en los que este tipo de aprendizajes son útiles y necesarios para innovar. 

**Herramientas y temas sugeridos:** 
- Fundamentos de las redes neuronales 
- Redes neuronales feedforward - Redes neuronales convolucionales (CNN) 
- Redes neuronales recurrentes (RNN)
**Tiempo: 2.5 semanas**

### Procesamiento del lenguaje natural (PLN) (4 semanas)

El procesamiento de lenguaje natural es un tema innovador y necesario para el desarrollo del mundo actual. Sin embargo, es un tema el cual no es conveniente detallar tanto pues es tan complejo que se necesitaría toda una clase para poder analizar esta área. Habiendo mencionado esto, el mejor acercamiento que se le puede dar a este tema es, de nuevo, cómo se pueden utilizar las herramientas actuales para enriquecer el análisis y automatización del análisis y predicción de datos.

**Herramientas y temas sugeridos:**
- Herramientas de procesamiento de Lenguaje Natural
- Preprocesamiento y tokenización de texto e Incrustaciones de palabras
- Análisis de sentimientos
- Reconocimiento de entidades nombradas
- Modelado de lenguaje y generación de secuencias

**Tiempo: 4 semanas**

### Big data y conmutación distribuida (2 semanas)

Big Data es un tema que tuvo su auge en la década de los 2010 's, por lo que avanzó de tal manera que ahora las herramientas están totalmente disponibles para utilizarse. Es por esto que el mejor acercamiento es definir de qué se trata la Big Data, su importancia en Data Science y cómo se pueden utilizar las herramientas para hacer más completo el proceso de análisis de datos de cada estudiante.

**Herramientas y temas sugeridos:**
- Herramientas de procesamiento de big data
- Introducción a Big Data
  - Definición
  - Importancia en la ciencia de datos
  - Desafíos asociados.
- Herramientas de procesamiento de Big Data: Panorama general de las herramientas más comunes.
- Manejo de grandes conjuntos de datos
  - Introducción a conceptos clave como el procesamiento distribuido y el almacenamiento de datos. 
  - Cómo manejar grandes datasets en Python, introducción a Dask. (Vaex es una alternativa a Dask)
- Dask a fondo
  - Trabajar con Dask para operaciones de procesamiento de datos, uso de Dask DataFrames, programación perezosa y paralela, y computación distribuida con Dask.
- Introducción a los marcos de trabajo para computación distribuida
  - Discusión sobre Hadoop y Spark, cómo se comparan con Dask.
- Concepto de MapReduce y procesamiento paralelo
  - Explicación de cómo funciona el paradigma de MapReduce, y cómo se utiliza en Dask y Spark.
- Algoritmos de aprendizaje automático escalables
  - Utilización de bibliotecas de aprendizaje automático que pueden trabajar con Dask, como Dask-ML o Dask-XGBoost.

**Tiempo: 2 semanas**

### Ética y privacidad en la ciencia de datos (0.5 semanas)

Este es un tema que es valioso detallar, ver las distintas reglas que existen a nivel mundial y cómo se encuentra este tema actualmente en Guatemala.

**Temas sugeridos:**
- Consideraciones éticas en la ciencia de datos
- Privacidad y protección de datos
- Sesgo y equidad en el aprendizaje automático
- Marcos y pautas éticas

**Tiempo: 0.5 semanas**

**Total de semanas: 16**
