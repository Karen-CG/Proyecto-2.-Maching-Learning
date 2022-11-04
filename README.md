# Proyecto-2.-Maching-Learning

En los siguientes nootbooks se mostrara el proceso de la obtención de modelos de Machine Learning para un dataset de inmuebles ubicados en Colombia donde se determinará el precio de la de propiedad a partir de otros datos otorgados que correspoden al año 2020.
El objetivo de diseñar modelos de Machine Learning que predigan el precio, es debido a que no se cuenta con una certeza sobre el valor de estos en el mercado, en este caso de los bienes inmuebles, por lo cual se trata de identificar  las tendencias durante el tiempo y estimar  el valor de la una propiedad para encontrar oportunidades de compra o de venta.

### Información de los dataset proporcionados
Se cuenta con dos datasets:

- 'properties_colombia_train.csv': Contiene 197549 registros y 26 dimensiones, el cual incluye la información numérica del precio.
- 'propiedades_colombia_test.csv': Contiene 65850 registros y 25 dimensiones, el cual no incluye la información del precio.

Descripción de las columnas:
* id - Identificador del aviso. No es único: si el aviso es actualizado por la inmobiliaria (nueva versión del aviso) se crea un nuevo registro con la misma id pero distintas fechas: de alta y de baja.
* ad_type - Tipo de aviso (Propiedad, Desarrollo/Proyecto)
* start_date - Fecha de alta del aviso.
* start_date - Fecha de alta del aviso.
* end_date - Fecha de baja del aviso.
* created_on - Fecha de alta de la primera versión del aviso.
* lat - Latitud.
* lon - Longitud.
* l1 - Nivel administrativo 1: país.
* l2 - Nivel administrativo 2: usualmente provincia.
* l3 - Nivel administrativo 3: usualmente ciudad.
* l4 - Nivel administrativo 4: usualmente barrio.
* l5 - Nivel administrativo 5.
* l6 - Nivel administrativo 6.
* rooms - Cantidad de ambientes.
* bedrooms - Cantidad de dormitorios (útil en el resto de los países).
* bathrooms - Cantidad de baños.
* surface_total - Superficie total en m².
* surface_covered - Superficie cubierta en m².
* price - Precio publicado en el anuncio.
* currency - Moneda del precio publicado.
* price_period - Periodo del precio (Diario, Semanal, Mensual)
* title - Título del anuncio.
* description - Descripción del anuncio.
* property_type - Tipo de propiedad (Casa, Departamento, PH).
* operation_type - Tipo de operación (Venta).
* geometry - Puntos geométricos formados por las coordenadas latitud y longitud.

### Obtención de datos
Las etapa en las que se divide el procesamiento de los datos son:

-Exploración de los datos: Se analiza la cantidad de valores faltantes, valores atipicos y si es necesario se normalizan los datos para su posterior procesamiento.

-Transformaciones de los datos: Se aplican lel escalado/normalización en caso necesario en columnas con datos de valor numperico; se aplicaca la codificación de variables categóricas.

-Selección de atributos relevantes: Conforme se van analizando las columnas y se aplican las transformaciones necesarias se van identificando las columnas que aportan mayor inforación a nuestro modelo

-Ingeniería de features: Si identificamos atributos que que puedan fucnionar como mejores predictores, se realiza una combinación de variables y se utiliza en el modelo

- Modelo de Machine Learning: Este de identificara  de acuerdo a los datos que se tienen y los resultados que se esperan obtener. Con los cual se estableceran parámetros que mejoren las predicciones
- 
Posterior al modelo obtenido de los datos, se tienen como resultado un archivivo .csv con valores de '0' si es barata y '1' si es cara, calculados a partir de la media 
de la columna price del archivo 'properties_colombia_train.csv'.


#### Evaluaión de los modelos

Como método de evaluación del desempeño del modelo, se utilizará la métrica de Exhaustividad (Recall) para las propiedades caras, a partir de la matriz de confusión (Confusion Matrix).Donde  son los verdaderos positivos y  los falsos negativos. Adicionalmente, se incluye la Accuracy como métrica de control. Que esta controladopor un dashbord en el cual se subiran los resultados obtenidos en formato .csv de dataset 'propiedades_colombia_test.csv'.

###### Lenguaje utilizado: Python
###### Librerias: pandas, matplotlib, numpy, seaborn, missingno, sklearn


