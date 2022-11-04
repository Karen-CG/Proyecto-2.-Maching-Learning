# Proyecto-2.-Maching-Learning

En los siguientes nootbooks se mostrara el proceso de la obtención de modelos de Machine Learning para un dataset de inmuebles ubicados en Colombia donde se determinará el precio de la de propiedad a partir de otros datos otorgados que correspoden al año 2020.
El objetivo de diseñar modelos de Machine Learning que predigan el precio, es debido a que no se cuenta con una certeza sobre el valor de estos en el mercado, en este caso de los bienes inmuebles, por lo cual se trata de identificar  las tendencias durante el tiempo y estimar  el valor de la una propiedad para encontrar oportunidades de compra o de venta.

### Información de los dataset proporcionados
Se cuenta con dos datasets:

- 'properties_colombia_train.csv': Contiene 197549 registros y 26 dimensiones, el cual incluye la información numérica del precio.
- 'propiedades_colombia_test.csv': Contiene 65850 registros y 25 dimensiones, el cual no incluye la información del precio.

Descripción de las columnas:
id - Identificador del aviso. No es único: si el aviso es actualizado por la inmobiliaria (nueva versión del aviso) se crea un nuevo registro con la misma id pero distintas fechas: de alta y de baja.

ad_type - Tipo de aviso (Propiedad, Desarrollo/Proyecto)
start_date - Fecha de alta del aviso.
start_date - Fecha de alta del aviso.
end_date - Fecha de baja del aviso.


Descripción de las dimensiones
id - Identificador del aviso. No es único: si el aviso es actualizado por la inmobiliaria (nueva versión del aviso) se crea un nuevo registro con la misma id pero distintas fechas: de alta y de baja.
ad_type - Tipo de aviso (Propiedad, Desarrollo/Proyecto).
start_date - Fecha de alta del aviso.
end_date - Fecha de baja del aviso.
created_on - Fecha de alta de la primera versión del aviso.
lat - Latitud.
lon - Longitud.
l1 - Nivel administrativo 1: país.
l2 - Nivel administrativo 2: usualmente provincia.
l3 - Nivel administrativo 3: usualmente ciudad.
l4 - Nivel administrativo 4: usualmente barrio.
l5 - Nivel administrativo 5.
l6 - Nivel administrativo 6.
rooms - Cantidad de ambientes.
bedrooms - Cantidad de dormitorios (útil en el resto de los países).
bathrooms - Cantidad de baños.
surface_total - Superficie total en m².
surface_covered - Superficie cubierta en m².
price - Precio publicado en el anuncio.
currency - Moneda del precio publicado.
price_period - Periodo del precio (Diario, Semanal, Mensual)
title - Título del anuncio.
description - Descripción del anuncio.
property_type - Tipo de propiedad (Casa, Departamento, PH).
operation_type - Tipo de operación (Venta).
geometry - Puntos geométricos formados por las coordenadas latitud y longitud.​

### Obtención de datos
Posterior al modelo obtneido de lso datos, se tienen como resultado un archivi

#### Evaluaión de los modelos




