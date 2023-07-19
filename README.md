
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



## 📌  Introducción
Este proyecto corresponde al segundo de la etapa de *Lab's* del programa de **Data Science** de **Henry**. El rol a desempeñar es el de Data Analyst.


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

## 📶  KPI´s 
1. <b>Conexiones por habitante</b>: Incrementar en 1.5% anual las conexiones por habitante en las provincias Tucumán, Jujuy, Salta, Mendoza, Misiones, Catamarca, Santa Cruz, Santiago Del Estero, Corrientes, Chaco, San Juan y Formosa en los próximos cuatro años.
>> * Métrica: aumento en el número de conexiones totales dividido por la población total de cada provincia, expresado en porcentaje.

>> * Aspecto del objetivo general: alcance de red de internet.

>> * Meta:

>>>   | Provincia             | 2022-Q1  | 2026-Q1  |
>>>   |-----------------------|----------|----------|
>>>   | Jujuy                 | 0.147960 | 0.207960 |
>>>   | Catamarca             | 0.147649 | 0.207649 |
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

3. <b>Aumento del porcentaje de provincias con una vmb mínima de 30 mbps</b>: Incrementar en 20% el porcentaje de provincias con vmb de mínimo 30mbps para el año 2023; 5% trimestral.

> > * Métrica: Porcentaje actual de provincias con una velocidad mínima de 30 Mbps.

>> * Aspecto del objetivo general: calidad y alcance.

>> * Meta : 82.5% provincias.

Índice
Hago la conexión con Google Drive
Importo las librerías
E T L
I. EXTRACCIÓN DE DATOS
II. TRANSFORMACIÓN
I.I DATASETS DE INTERNET
DF: acc_velocidad_rangos
DF : acc_tecnologia_prov
DF : acc_banda_prov
DF : pen_cien_hogares
DF : velocidad_media_prov
Continuaré con los siguientes datasets correspondientes al servicio de internet en Argentina:
DF: acc_localidad
DF: conectividad_localidad
Continuaré con el último dataset relacionado al servicio de internet en Argentina:
DF: internet_ingresos
I.II DATASETS DE TELEFONÍA FIJA
DF: telf_fija_acc_prov
DF: telf_fija_ingresos
I.III DATASETS DE TELEFONÍA MOVIL
DF: telf_movil_ingresos
DF: telf_movil_portab
DF: telf_movil_acc_total
III. CARGA


