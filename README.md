
<h1 align=center> <strong>PROYECTO INDIVIDUAL Nº2</strong> </h1>
<p align=center><img style="display: block; 
           margin-left: auto;
           margin-right: auto;
           width: 50
           height=50"
        src="https://media.licdn.com/dms/image/D4D16AQFkgLIRJjy6SQ/profile-displaybackgroundimage-shrink_350_1400/0/1687728249782?e=1695254400&v=beta&t=Uhkp3KZk0aLDPW2rV1aL-k3LNBFXgUeaYGjuAhEo18k" 
        alt="DA"><p>
  <h2 align="center">Data Analytics</h2>
  <h3 align="center"> <i>Realizado por Olga Acosta </i></h3>



# 📍  Introducción
Este proyecto corresponde al segundo de la etapa de *Lab's* del programa de **Data Science** de **Henry**. 

En nuestra sociedad actual, la industria de las telecomunicaciones juega un papel esencial al facilitar el flujo de información a nivel internacional y mantener una comunicación continua, incluso en situaciones desafiantes como una pandemia mundial. La transferencia de datos y la comunicación se llevan a cabo principalmente a través de internet, líneas telefónicas fijas, telefonía móvil y otros medios que nos acompañan en prácticamente cualquier lugar del mundo. Así, se ha vuelto indispensable para los gobiernos nacionales medir el progreso de su región a través de, entre otros factores, el internet, sus conexiones, alcance y accesibilidad.

Es en este contexto en el que se gesta y desarrolla el presente proyecto: el análisis de la situación actual del sector de internet y de su comportamiento en los últimos cuatro años en Argentina, tanto a nivel nacional como provincial. Para tal efecto, he utilizado como data principal la proporcionada por [ENACOM](https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/), así como otros datasets complementarios especificados más adelante.

El análisis abarca diferentes aspectos relacionados a la conectividad a internet a nivel nacional y provincial, así como a la calidad de dicha conectividad, examinando la cantidad de accesos y abarcando las diferentes tecnologías presentes en Argentina, así como los rangos de velocidades, la velocidad media de bajada, el crecimiento porcentual de estas variables y la detección de zonas críticas respecto a éstas.

A partir del análisis realizado, he obtenido conclusiones que toman en cuenta distintos insights y oportunidades de mejora en el sector, con el fin de elaborar una propuesta de negocio  basada en la mejora del alcance y la calidad de los accesos a internet, así como la definición de indicadores de rendimiento en relación a dicho objetivo. Todo esto se desarrolla en el presente informe y se documenta con mayor especificidad en el contenido de este repositorio.

Cabe resaltar, sin ánimo de caer en la obviedad, que el rol a desempeñar es el de *Data Analyst*.

# 📍 Contenido del repositorio
En este repositorio se encuentran almacenadas cinco carpetas y dos archivos:
* En la carpeta **Datatsets** se encuentra la data a partir de la cual se ha realizado el ETL (backup proporcionado por Henry).
* En la carpeta **Datasets API** se encuentra la data obtenida a través de la API de [ENACOM](https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/), la cual presentó algunas fallas de descarga no pudiéndose descargar todos los datasets requeridos, por lo cual  no llegaron a utilizarse en el proyecto.
* En la carpeta **Data_Población** se encuentra un archivo complementario relacionado a estimaciones de población para distintos periodos y provincias de Argentina, obtenidos de [INDEC - Argentina.](https://www.indec.gob.ar/indec/web/Nivel4-Tema-2-24-85).
* En la carpeta **POST_ETL_Datasets** se encuentra la data limpia después de realizado el proceso de ETL.
* En la carpeta **POST_EDA_Datasets** se encuentra la data transformada después de realizado el proceso de EDA, la cual se ha utilizado para la realización del dashboard.
* En el archivo **ETL** se encuentra la documentación y el paso a paso del ETL.
* En el archivo **EDA** se encuentra la documentación y el paso a paso del EDA. 

# 📍 Contexto de los datos
Los datos en bruto se obtuvieron, inicialmente de la página [ENACOM](https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/) y a través de su API. Sin embargo, ésta presentó fallas de descarga y errores de ubicación, por lo que , finalmente, no se pudo trabajar a partir de ellas. 
Por este motivo, se utilizó el backup proporcionado por Henry siendo éste el principal punto de origen de la data de este proyecto.
Así también, se utilizó un archivo complementario que comprende información de la cantidad de población en Argentina por provincia y por periodo. Este archivo se obtuvo de [INDEC - Argentina.](https://www.indec.gob.ar/indec/web/Nivel4-Tema-2-24-85).
A continuación, se dejan los enlaces a google drive donde se encuentran los distintos datasets del proyecto, para su posterior descarga:

## 📁  Data
* [Obtenidos por medio de la API](https://drive.google.com/drive/folders/1nxsFvCUPy5Fx2jk0A3rBNnBG9_KDktMb?usp=sharing)
* [Provistos por Henry](https://drive.google.com/drive/folders/1lwMXU-lQVbsmR31d3G1qXkqfSro0VOe8?usp=sharing)
* [Post-ETL](https://drive.google.com/drive/folders/1mLA56sm9a16brw9xF-6WST5s0z2MqIV7?usp=sharing)
* [Post-EDA](https://drive.google.com/drive/folders/1dE0vhE55ymS-UcgFpuUruRqUoOzHqpXl?usp=sharing)
* [Complementarios - Población](https://drive.google.com/drive/folders/1r3ITs13ZhGMBvgGPSzk8Uq86c84JtCd7?usp=sharing)

## 📙  Diccionario de datos

| Campo                     | Descripción                                                                                               |
|---------------------------|-----------------------------------------------------------------------------------------------------------|
| Año                       | El año correspondiente a los datos de la fila.                                                            |
| Trimestre                 | El trimestre correspondiente a los datos de la fila.                                                      |
| Provincia                 | El nombre de la provincia para la cual se proporcionan los datos.                                         |
| ADSL                      | Número de conexiones de tipo ADSL en la provincia para el año y trimestre específicos.                   |
| Cablemodem                | Número de conexiones de tipo Cablemodem en la provincia para el año y trimestre específicos.             |
| Fibra óptica              | Número de conexiones de tipo Fibra óptica en la provincia para el año y trimestre específicos.           |
| Wireless                  | Número de conexiones de tipo Wireless en la provincia para el año y trimestre específicos.               |
| Otros                     | Número de conexiones de otros tipos en la provincia para el año y trimestre específicos.                  |
| Total_conexion            | Total de conexiones de Internet en la provincia para el año y trimestre específicos.                      |
| Accesos por cada 100 hab  | Número de accesos a Internet por cada 100 habitantes en la provincia para el año y trimestre específicos. |
| Accesos por cada 100 hog  | Número de accesos a Internet por cada 100 hogares en la provincia para el año y trimestre específicos.    |
| Banda ancha fija          | Número de conexiones de banda ancha fija en la provincia para el año y trimestre específicos.            |
| Dial up                   | Número de conexiones de tipo Dial up en la provincia para el año y trimestre específicos.                |
| Hasta 512 kbps            | Número de conexiones con velocidad hasta 512 kbps en la provincia para el año y trimestre específicos.    |
| 512 Kbps - 1 Mbps         | Número de conexiones con velocidad entre 512 Kbps y 1 Mbps en la provincia para el año y trimestre específicos. |
| 1 Mbps - 6 Mbps           | Número de conexiones con velocidad entre 1 Mbps y 6 Mbps en la provincia para el año y trimestre específicos. |
| 6 Mbps - 10 Mbps          | Número de conexiones con velocidad entre 6 Mbps y 10 Mbps en la provincia para el año y trimestre específicos. |
| 10 Mbps - 20 Mbps         | Número de conexiones con velocidad entre 10 Mbps y 20 Mbps en la provincia para el año y trimestre específicos. |
| 20 Mbps - 30 Mbps         | Número de conexiones con velocidad entre 20 Mbps y 30 Mbps en la provincia para el año y trimestre específicos. |
| 30 Mbps                   | Número de conexiones con velocidad superior a 30 Mbps en la provincia para el año y trimestre específicos. |
| Otros Mbps                | Número de conexiones con velocidad de otros tipos en la provincia para el año y trimestre específicos.    |
| Total suma Mbps           | Total de la suma de todas las conexiones de Internet por velocidad en la provincia para el año y trimestre específicos. |

# 📍 Flujo de trabajo

## 🛠️ [ETL](https://colab.research.google.com/drive/1BbIPZ5tFbL-5z8g2AsPRW4e6-6cq53Vm?usp=sharing)
* Descarga de algunos datasets a través de la API. Al no poderse descargar todos los necesarios, se optó por usar el backup de Henry.
* Cambio de tipos de datos, así como extracción de puntos en variables numéricas.
* Unión de dataframes relacionadosy elección de columnas relevantes.
* Detección de valores con errores y noormalización de los mismos.
* Detección de nulos e imputación de los mismos.
* Detección de duplicados.
Las diferentes etapas de transformación se llevaron a cabo con el propósito de obtener un conjunto de datos de excelente calidad, coherente y pertinente para su posterior análisis. Al asegurar la limpieza y estandarización de los datos, se establece una base sólida para obtener conclusiones fiables y tomar decisiones fundamentadas.

## 📊 [EDA](https://colab.research.google.com/drive/16Nlj4zOD7aJnHfpPK2QGs1Lk15Rx8416?usp=sharing)
* Revisé primero el dataset relacionado a las conexiones por rango de velocidad 


## ✍ Conclusiones

# 📍 Propuesta de negocio
Explicar la importancia

## 👔 Clientes potenciales

## 🎯 Objetivo

## 📶  KPI´s 
1. <b>Conexiones por habitante</b>: Incrementar en 1.5% anual las conexiones por habitante en las provincias Tucumán, Jujuy, Salta, Mendoza, Misiones, Catamarca, Santa Cruz, Santiago Del Estero, Corrientes, Chaco, San Juan y Formosa en los próximos cuatro años.
>> * Métrica: aumento en el número de conexiones totales dividido por la población total de cada provincia, expresado en porcentaje.

>> * Aspecto del objetivo general: alcance de red de internet.

>> * Meta:

>>>   | Provincia             | 2022-Q1  | 2026-Q1  |
>>>   |-----------------------|----------|----------|
>>>   | Jujuy                 | 0.147960 | 0.207960 |
>>>   | Catamarca             | 0.147649 | 0.207649 |
>>>   | Misiones              | 0.133109 | 0.193109 |
>>>   | Tucuman               | 0.141619 | 0.201619 |
>>>   | Corrientes            | 0.125112 | 0.185112 |
>>>   | Salta                 | 0.135342 | 0.195342 |
>>>   | Chaco                 | 0.117386 | 0.177386 |
>>>   | Formosa               | 0.088738 | 0.148738 |
>>>   | Mendoza               | 0.135555 | 0.195555 |
>>>   | Santa Cruz            | 0.127927 | 0.187927 |
>>>   | Santiago Del Estero   | 0.116684 | 0.176684 |
>>>   | San Juan              | 0.110541 | 0.170541 |
>>>
>>> 


2. <b>Aumento del porcentaje de conexiones Cablemodem por conexiones totales</b>: Incrementar en 2.5% anual las conexiones en la tecnología Cablemodem en  San Luis, Tucumán, San Juan y Formoza en los próximos cuatro años.

> > * Métrica: aumento en el número de conexiones Cablemodem dividido por las conexiones totales de cada provincia, expresado en porcentaje.

>> * Aspecto del objetivo general: calidad.

>> * Meta: 

>>> | Provincia | 2022-1  | 2026-1  |
>>> |-----------|---------|---------|
>>> | Tucuman   | 0.254072 | 0.354072 |
>>> | San Juan  | 0.163862 | 0.263862 |
>>> | Formosa   | 0.291981 | 0.391981 |
>>> | San Luis  | 0.094256 | 0.194256 |


3. <b>Aumento del porcentaje de provincias con una vmb mínima de 30 mbps</b>: Incrementar en 20% el porcentaje de provincias con vmb de mínimo 30mbps para el año 2023; 5% trimestral.

> > * Métrica: Porcentaje actual de provincias con una velocidad mínima de 30 Mbps.

>> * Aspecto del objetivo general: calidad y alcance.

>> * Meta : 82.5% provincias.

# 📍 Herramientas utilizadas





