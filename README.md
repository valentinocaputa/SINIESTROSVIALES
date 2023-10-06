# :mag_right: Proyecto integrador N2 :mag:

# Introduccion
:pushpin: En este informe, se presenta un análisis de datos sobre homicidios en siniestros viales ocurridos en la Ciudad Autónoma de Buenos Aires (CABA) durante el período comprendido entre 2016 y 2021.
El objetivo principal de este proyecto es proporcionar información crucial que permita a las autoridades locales tomar medidas efectivas para reducir la cantidad de víctimas fatales en siniestros viales en la ciudad.

# Contexto 
Para llevar a cabo este proyecto, se utilizaron 2 conjuntos de datos disponibles en la página de Gobierno de la Ciudad de Buenos Aires:
_**HECHOS**_: Esta planilla contiene información detallada sobre cada siniestro vial con un ID único y diversas variables relacionadas con el tiempo, el espacio y los participantes en el incidente.

_**VICTIMAS**_: Aquí se registran los datos de cada víctima involucrada en los hechos, incluyendo edad, sexo y modo de desplazamiento. Esta pestaña está vinculada a la pestaña HECHOS a través del ID del siniestro.

# Transformaciones 
Antes de poder extraer valor de estos datos, tuve que someterlos a un proceso de ETL, 
este proceso es esencial para limpiar, transformar y preparar los datos para analizarlos posteriormente.

_**extraccion:**_ Comence cargando los archivos para poder entender cada columna y el tipo de datos que contenia.

_**transformacion:**_ Realice una transformacion de los datos, eliminando duplicados, tratando valores nulos, y 
realizando conversiones de tipos cuando fue necesario.

_**carga:**_ Una vez limpios y transformados, cargue estos datos en una estructura mas adecuada para su analisis de EDA y posterior implementacion,
creando un solo dataframe con las 2 plantillas, llamado homicidios_final.

# EDA
_**Hechos por distribucion**_

▪️En la visualización de accidentes anuales, destaca que el año 2016 tuvo el pico más alto de incidentes, registrando cerca de 145 accidentes, contrastando con esto, el año 2020 experimentó el punto más bajo en registros de accidentes.

▪️Diciembre, con sus festividades y celebraciones, crea un escenario propenso a incidentes en las vías ya que emerge como el mes con el mayor porcentaje de números de accidentes viales.

![image](https://github.com/valentinocaputa/SINIESTROSVIALES/assets/125314207/64a25a8f-612b-4eb8-8445-0000aeed1ba2)
![image](https://github.com/valentinocaputa/SINIESTROSVIALES/assets/125314207/65b4807d-033b-4aae-8ecd-04f24efacbf3)

_**Hechos por franja horaria y zonas de mayor incidencia**_

▪️Al analizar los accidentes en función de la franja horaria, es evidente que la mayoría de los incidentes suelen ocurrir en horas de la mañana. Esta tendencia puede estar relacionada con horarios pico.

▪️Es notable que las avenidas son las zonas con más accidentes, alcanzando un pico de casi 430 incidentes. Las avenidas, siendo arterias principales de tráfico, experimentan un flujo vehicular alto y constante, lo que 
puede aumentar la probabilidad de incidentes.

![image](https://github.com/valentinocaputa/SINIESTROSVIALES/assets/125314207/73aed336-9466-4a47-b1a7-faae2d46a958)
![image](https://github.com/valentinocaputa/SINIESTROSVIALES/assets/125314207/93e32572-6121-4f63-a493-a068391e6c9b)

_**Numero de incidentes por tipo de vehiculo y victimas del siniestro**_

▪️Al observar la cantidad promedio de víctimas por accidente, se evidencia que, en su mayoría, cada incidente afecta a una sola persona.

▪️De los datos, destaca que las motocicletas son las más involucradas en accidentes de tránsito.

![image](https://github.com/valentinocaputa/SINIESTROSVIALES/assets/125314207/ec7958e2-9eeb-4726-ae02-4d2b8e8fdf42)
![image](https://github.com/valentinocaputa/SINIESTROSVIALES/assets/125314207/bb3f5081-5711-43c7-b64b-e0afb2e7a4ea)

# KPIS 
▪️Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior. 

▪️Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior. 

▪️Reducir la variación de tasa de homicidios por sexo respecto al semestre anterior. 

![image](https://github.com/valentinocaputa/SINIESTROSVIALES/assets/125314207/01fac1b2-4df7-4afa-a6a2-5d0de68e30b7)

▪️La tasa de homicidios ha disminuido en un 1.40% desde el período anterior al actual, pero si nos fijamos el ultimo semestre no se llega al objetivo de reduccion del 10%, lo mismo para las motos, ya que en el año 2018 que 
ha habido una reducción del 15.625% en los accidentes de motocicletas desde el período anterior al actual pero no se llega la resultado deseado del 7% debido a un aumento del 12.5%, asi bien en el semestre 1 del 2018 es 
donde se logra la reduccion de ambos kpis, como se puede observar en la siguientes imagenes ⤵️✔️

![image](https://github.com/valentinocaputa/SINIESTROSVIALES/assets/125314207/e9dbdff5-3dce-4c9d-afd3-547bb64cc1ea)
![image](https://github.com/valentinocaputa/SINIESTROSVIALES/assets/125314207/35d4d45c-bf65-4bdc-a3c1-228644a35f0b)


