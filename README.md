![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png) 

# PROYECTO INDIVIDUAL III

## Descripción del proyecto: </br>  
En este proyecto realizaremos un EDA (Análisis Exploratorio de Datos) sobre un dataset que tiene información sobre los accidentes aereos que han ocurrido desde el siglo XX en adelante, esto con el fin de que la **Organización de Aviación Civil Internacional (OACI)** investigue a profundidad estos accidentes. </br>

Nuestro dataset de trabajo original sera 'AccidentesAviones.csv' pero usaremos otras fuentes de datos para complementar el analisis y la investigación de la causalidad y relacion  de los accidentes aereos para obtener mayor claridad y consistencia en la investigación a realizar.</br>

Dividiremos el proyecto en diferentes fases que nos permitiran realizar correctamente el EDA, adicional a esto realizaremos un reporte de calidad de los datos que nos permitira informar el estado en el cual recibimos los datos y que manejo le dimos a estos, un diccionario de datos donde especificaremos la informacion que almacena cada dimension, y su tipo de dato, crearemos una base de datos donde importaremos los datos limpios y transformados y por ultimo realizaremos un dashboard interactivo donde evidenciaremos los diferentes analisis que se realizaron en la investigación.</br>

Las preguntas que vamos a estar respondiendo con el dashboard son las siguientes:
+ ¿En que año hay mayor cantidad de muertes?
+ ¿Cuantós sobrevivientes hay por año?
+ ¿En que tipo de vuelo hay mayor cantidad de muertes?

## Descripción del dataset de origen: </br>
AccidentesAviones.csv : Contiene 17 dimensiones y 5008 registros.</br> 
Nuestro dataset contiene la siguiente información sobre los accidentes ocurridos desde el siglo XX hasta la actualidad (1920 - 2022)
* Todos los accidentes de aviación civil y comercial de aviones de pasajeros regulares y no regulares en todo el mundo, que resultaron en una  muerte (incluidos todos los accidentes fatales de la Parte 121 y la Parte 135 de EE. UU.)
* Todos los accidentes fatales de carga, posicionamiento, transbordadores y vuelos de prueba.
* Todos los accidentes de transporte militar con 10 o más muertes.
* Todos los accidentes de helicópteros comerciales y militares con más de 10 muertes.
* Todos los accidentes de dirigibles civiles y militares con víctimas mortales.
* Accidentes de aviación que involucran la muerte de personajes famosos.
* Accidentes o incidentes de aviación de interés destacado.

## Descripción de las dimensiones del dataset de origen: </br> 

+  Fecha: Fecha del accidente, en el formato - 01 de enero de 20
+  Hora declarada: Hora local, en 24 h. formato a menos que se especifique lo contrario
+  Ruta: Lugar del accidente
+  Operador: Tipo de operador de vuelo
+  flight_no: Número de vuelo asignado por el operador de la aeronave
+  route: Ruta completa o parcial volada antes del accidente
+  ac_type: Tipo de aeronave
+  registration : Matrícula OACI de la aeronave
+  cn_ln: Número de construcción o de serie / Número de línea o de fuselaje
+  all_aboard: Total a bordo (pasajeros/tripulación)
+  Pasajeros a bordo: Cantidad de pasajeros en el avión
+  crew_aboard: Cantidad de tripulación a bordo
+  cantidad de fallecidos: Cantidad de fallecidos en el accidente 
+  passenger_fatalities: Cantidad de pasajeros muertos
+  crew_fatalities: Cantidad de muertos de la tripulación del avión
+  ground : Total muertos en tierra
+  summary: Breve descripción del accidente y causa si se conoce

http://www.planecrashinfo.com/database.htm <---- Información obtenida en esta pagina

## Fases de realización del proyecto

1. Carga de los datasets
2. EDA (Análisis Exploratorio de Datos)
    + Transformación y limpieza de los datos
    + Resumen estadistico
    + Distribuicion de frecuencia
    + Boxplots
    + Correlación
3. Realizacion del reporte de calidad y diccionario de datos    
4. Creacion de la base de datos y carga del dataset limpio y transformado
5. Creacion del dashboard interactivo

Frameworks usados
+ `Python`: EDA + transformaciones 
+ `MySql Workbench`: base de datos
+ `Power BI`: dashboard 
