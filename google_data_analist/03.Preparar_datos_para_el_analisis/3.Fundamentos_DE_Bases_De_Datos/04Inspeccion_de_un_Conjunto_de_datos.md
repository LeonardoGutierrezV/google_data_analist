# Inspección de un Conjunto de datos: Una visita guiada y práctica

Como Analista de datos, utilizará los datos para responder a preguntas y resolver problemas. Cuando analiza Datos y extrae conclusiones, está generando estadísticas que pueden influir en las decisiones empresariales, impulsar cambios positivos y ayudar a las partes interesadas a alcanzar sus objetivos.

Antes de comenzar un análisis, es importante inspeccionar sus datos para determinar si contienen la información específica que necesita para responder a las preguntas de sus partes interesadas. En cualquier Conjunto de datos dado, puede darse el caso de que:

* Los datos no existen (tiene datos sobre sándwiches, pero necesita datos sobre pizzas)

* Los datos sean insuficientes (tiene datos de pizza del 1 al 7 de junio, pero necesita datos de todo el mes de junio)

* Los datos son incorrectos (sus datos de pizza indican que el coste de una porción es de 250 $, lo que le hace cuestionar la validez del conjunto de datos)

La Inspección de su Conjunto de datos le ayudará a determinar qué preguntas tienen respuesta y qué datos siguen faltando. Es posible que pueda recuperar estos datos de una fuente externa o, al menos, recomendar a sus partes interesadas que utilicen otra fuente de datos.

En esta lectura, imagine que es usted un Analista de datos que inspecciona los datos de una hoja de cálculo para determinar si es posible responder a las preguntas de sus partes interesadas. 

## El escenario

Usted es un analista de datos que trabaja para una empresa de helados. La dirección está interesada en mejorar las ventas de helados de la empresa.

La empresa ha estado recopilando datos sobre sus ventas, pero no muchos. Los datos disponibles proceden de una fuente de datos interna y se basan en las ventas de 2019. Se le ha pedido que revise los datos y proporcione algunas estadísticas sobre las ventas de helados de la empresa. Idealmente, a la dirección le gustaría obtener respuestas a las siguientes preguntas:

1. ¿Cuál es el sabor de helado más popular?

2. ¿Cómo afecta la temperatura a las ventas?

3. ¿Cómo afectan a las ventas los fines de semana y los días festivos?

4. ¿En qué se diferencia la rentabilidad de los clientes nuevos de la de los que vuelven?

## Descargar los datos

Puede descargar los datos para seguir esta lectura. Para utilizar la plantilla para los datos de ventas, haga clic en el siguiente enlace y seleccione "Usar plantilla" 

Enlace a la plantilla: 
[Ventas de helados](https://docs.google.com/spreadsheets/d/1NgiKb8wCnJbUTuUkDUiNRpx9NhwncEmoKuPvgfYfOIY/template/preview?resourcekey=0-X3e7NzehG2Y74MIBhOaqeQ#gid=653912415)

O

Si no dispone de una cuenta de Google, puede descargar las hojas de cálculo directamente de los archivos adjuntos que aparecen a continuación:

[SalesByDay.xlsx](/google_data_analist/03.Preparar_datos_para_el_analisis/assets/SalesByDay.xlsx)

[SalesByFlavor.xlsx](/google_data_analist/03.Preparar_datos_para_el_analisis/assets/SalesByFlavor.xlsx)

[SalesByTemp.xlsx](/google_data_analist/03.Preparar_datos_para_el_analisis/assets/SalesByTemp.xlsx)


## Inspección de los Datos

### Pregunta 1: ¿Cuál es el sabor de helado más popular?

Para descubrir cuál es el sabor más popular, primero tiene que definir qué se entiende por "popular" ¿Es el sabor más popular el que generó más Ingresos en 2019? ¿O es el sabor que tuvo el mayor número de unidades vendidas en 2019? A veces sus opciones de medición se ven limitadas por los datos de que dispone; puede revisar su hoja de cálculo para averiguar si alguna de estas definiciones de "popular" tiene sentido en función de los datos disponibles.

Clic en la pestaña sabores de su hoja de cálculo para ver los datos relevantes. La hoja de sabores tiene tres columnas y 209 filas de datos. Los encabezados de las columnas son semana, unidades vendidas y sabor. Este Conjunto de datos no venía con una descripción de los datos, por lo que tiene que averiguar el significado de las columnas por su cuenta. Basándose en los datos, usted deduce que estas columnas proporcionan información sobre el número de unidades vendidas de cada sabor de helado, por semana, en 2019

![Captura01](/google_data_analist/03.Preparar_datos_para_el_analisis/assets/030401.png)

Una captura de pantalla de una hoja de cálculo con datos en 3 columnas etiquetadas como semana, unidades vendidas y sabor

En este caso, puede descubrir cuál es el sabor más popular utilizando las unidades vendidas como medida. En concreto, puede utilizar la columna de unidades vendidas para calcular el número total de unidades vendidas durante el año para cada sabor. Lamentablemente, el Conjunto de datos no proporciona el importe de las ventas anuales por sabor. En este caso, su siguiente paso sería preguntar a sus partes interesadas si los datos de ventas anuales por sabor están disponibles en otra fuente. Si no es así, puede añadir a su análisis una declaración sobre las limitaciones de los datos actuales.

### Pregunta 2: ¿Cómo afecta la temperatura a las ventas?

Para explorar su segunda pregunta, haga clic en la ficha de temperaturas y consulte los datos. La hoja de temperaturas tiene dos columnas y 366 filas de datos. Los encabezados de las columnas son temperatura y ventas. Los datos pueden mostrar las ventas totales de 2019 por temperatura (por ejemplo, la primera entrada podría sumar 39,69 $ en ventas durante tres días distintos que tuvieron cada uno una máxima de 60 grados). O bien, los datos pueden mostrar una instantánea de las ventas y la temperatura de cada día de 2019 (por ejemplo, la primera entrada podría referirse a un único día con una máxima de 60 grados y 39,69 dólares en ventas).

![Captura02](/google_data_analist/03.Preparar_datos_para_el_analisis/assets/030402.png)

Una captura de pantalla de una hoja de cálculo con datos en 2 columnas etiquetadas como temperatura y ventas

Entonces, ¿de qué se trata? Probablemente sea una instantánea diaria porque hay 365 entradas para la temperatura, y varias filas con la misma temperatura y diferentes valores de ventas. Esto implica que cada entrada corresponde a un solo día y no a un resumen de varios días. Sin embargo, sin más información, no puede estar seguro. Además, no sabe si los datos actuales aparecen en orden consecutivo por fecha o en un orden diferente. Su siguiente paso sería ponerse en contacto con el propietario del Conjunto de datos para que se lo aclare.

Si resulta que la temperatura sí afecta a las ventas, podrá ofrecer a sus partes interesadas una estadística como la siguiente: "Cuando las máximas diarias superan los X grados, las ventas medias de helado aumentan en Y cantidad. Así que la empresa debería planificar el aumento del inventario durante estas épocas para maximizar las ventas"

### Pregunta 3: ¿Cómo afectan los fines de semana y los días festivos a las ventas?

A continuación, haga clic en la ficha de ventas para ver los datos sobre las fechas de venta. La hoja de ventas tiene dos columnas y 366 filas de datos. Los encabezados de las columnas son fecha y ventas. Lo más probable es que estos datos sean las ventas diarias totales en 2019, ASÍ como las ventas registradas para cada fecha en 2019. 

![Captura03](/google_data_analist/03.Preparar_datos_para_el_analisis/assets/030403.png)

Una captura de pantalla de una hoja de cálculo con datos en 2 columnas etiquetadas como fecha y ventas

Puede utilizar estos datos para determinar si una fecha concreta cae en fin de semana o festivo y añadir una columna a su hoja que refleje esta información. A continuación, podrá averiguar si las ventas de los fines de semana y días festivos son mayores que las de los demás días. Le resultará útil saberlo a efectos de planificación de inventarios y de marketing.

### Pregunta 4: ¿En qué se diferencia la rentabilidad de los nuevos clientes de la de los clientes habituales?

Su Conjunto de datos no contiene datos de ventas relacionados con los nuevos clientes. Sin estos datos, no podrá responder a su pregunta final. Sin embargo, puede darse el caso de que la empresa recoja los datos de los clientes y los almacene en una tabla de datos diferente.

Si es así, su siguiente paso sería averiguar cómo acceder a los datos de los clientes de la empresa. A continuación, puede unir los datos de ventas de ingresos a la tabla de datos de clientes para categorizar cada venta como de un cliente nuevo o recurrente y analizar la diferencia de rentabilidad entre los dos conjuntos de clientes. Esta información ayudará a las partes interesadas a desarrollar campañas de marketing para tipos específicos de clientes con el fin de aumentar la fidelidad a la marca y la rentabilidad general.

### Puntos clave

Cuando trabaje en proyectos de análisis, no siempre dispondrá de todos los datos necesarios o relevantes. En muchos de estos casos, puede recurrir a otras fuentes de datos para cubrir las lagunas.

a pesar de las limitaciones de su conjunto de datos, aún es posible ofrecer a sus partes interesadas algunas estadísticas valiosas. Para los siguientes pasos, su mejor plan de acción será tomar la iniciativa de hacer preguntas, identificar otros conjuntos de datos relevantes o hacer alguna investigación por su cuenta. Independientemente de los datos con los que esté trabajando, inspeccionar cuidadosamente sus datos tiene un gran impacto en la calidad general de su análisis.



