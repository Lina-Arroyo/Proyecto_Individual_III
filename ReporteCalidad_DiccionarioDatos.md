 >Reporte de calidad y diccionario de datos

REPORTE DE CALIDAD

Al realizar el proceso de ETL con el csv recibido por parte de la **Organización de Aviación Civil Internacional (OACI)**  se evidencio al realizar el EDA que el dataset recibido debia ser normalizado en algunas de las columnas (dimensiones), el archivo fue pasado en un tipo .csv, el delimitador mantenia la coherencia de los datos y todas las dimensiones contaban con la misma cantidad de datos</br>

En este caso el dataset no contaba con valores faltantes, estos valores estaban imputados con un signo de pregunta (?), el manejo que se le dio a estos fue reemplazar este valor (?) por: en el caso de datos de tipo cuantitavivos se reemplazo con cero (0), y en el caso de valores categoricos se reemplazo con un Sin dato. </br>

El dataset contaba con valores que parecian atipicos con respecto a los demas datos en gran parte de las dimensiones que representaban categorias, al analizarlos y visualizarlos se evidencio que estos valores aunque representaban una anormalidad, no generaban tanto ruido con respecto a los demas y que al momento de hacerles un manejo o corrección se podria perder valores de gran importancia para el analisis e investigación del caso. </br>

En la columna hora habian demasiados datos que contenian caracteres como (c, c:, Z, ;) que no correspondian con el formato de hora que tenian la gran mayoria de datos y esto ocasionaba un error al hacer la conversión al tipo de dato que corresponde, el manejo dado a este problema fue eliminar estos caracteres sin afectar el dato y su formato. </br>

No se realizo el descarte de ninguna columna ya que todas revelaban información importante para el analisis de los datos, la resolución de las incognitas propuestas y la investigación a realizar con estos </br>

DICCIONARIO DE DATOS

Columna 1 : Fecha
* Descripción: Fecha del accidente, en el formato - 01 de enero de 20
* Tipo: DateTime

Columna 2: Hora declarada
* Descripción: Hora local del accidente, en 24 h. formato a menos que se especifique lo contrario
* Tipo: Time

Columna 3: Ruta
* Descripción: Lugar del accidente
* Tipo: String

Columna 4: Operador
* Descripción: Tipo de operador de vuelo
* Tipo: String

Columna 5: flight_no
* Descripción: Número de vuelo asignado por el operador de la aeronave
* Tipo: String

Columna 6: route
* Descripción: Ruta completa o parcial volada antes del accidente
* Tipo: String

Columna 7: ac_type
* Descripción: Tipo de aereonave
* Tipo: String

Columna 8: registration
* Descripción: Matrícula OACI de la aeronave
* Tipo: String

Columna 9: cn_ln
* Descripción: Número de construcción o de serie / Número de línea o de fuselaje
* Tipo: String

Columna 10: all_aboard
* Descripción: Total a bordo (pasajeros/tripulación)
* Tipo: Int32

Columna 11: Pasajeros a bordo
* Descripción: Cantidad de pasajeros en el avión
* Tipo: Int32

Columna 12: crew_aboard
* Descripción: Cantidad de tripulación a bordo
* Tipo: Int32

Columna 13: cantidad de fallecidos
* Descripción: Cantidad de fallecidos en el accidente
* Tipo: Int32

Columna 14: passanger_fatalities
* Descripción: Cantidad de pasajeros muertos
* Tipo: Int32

Columna 15: crew_fatalities
* Descripción: Cantidad de muertos de la tripulacion del avión
* Tipo: Int32

Columna 16: ground
* Descripción: Total de muertos en tierra
* Tipo: Int32

Columna 17: summary
* Descripción: Breve descripción del accidente y causa si se conoce
* Tipo: String 




