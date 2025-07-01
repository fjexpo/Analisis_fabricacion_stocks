\# Dashboard Interactivo con Power BI



Esta carpeta contiene la solución al desafío de negocio implementada en Power BI, enfocada en la creación de un dashboard interactivo y visualmente atractivo.



\## 📁 Archivos



\-   `Dashboard\_Stock\_PowerBI.pbix`: El archivo de proyecto de Power BI.

\-   `screenshot\_dashboard\_powerbi.png`: Una imagen de vista previa del dashboard final.



\## 🛠️ Metodología Utilizada



Power BI permite un flujo de trabajo integrado desde la ingesta de datos hasta la presentación final.



1\.  \*\*Transformación de Datos (ETL) con Power Query:\*\*

&nbsp;   -   Al igual que en Excel, se utilizó el Editor de Power Query (`Transformar datos`) para limpiar y preparar el dataset. Los pasos de limpieza son idénticos a los del análisis en Excel.



2\.  \*\*Modelado de Datos y DAX:\*\*

&nbsp;   -   Se creó un modelo de datos relacional, incluyendo una \*\*tabla de calendario\*\* dedicada para un análisis de tiempo robusto.

&nbsp;   -   Se utilizaron \*\*columnas calculadas\*\* para métricas a nivel de fila y \*\*medidas DAX\*\* para agregaciones dinámicas y eficientes. La fórmula clave corregida para `CosteAdquisicionPromedio` fue:

&nbsp;       ```dax

&nbsp;       CosteAdquisicionPromedio =

&nbsp;       AVERAGEX(

&nbsp;           FILTER(

&nbsp;               'datos\_empresa',

&nbsp;               'datos\_empresa'\[ID\_Producto] = EARLIER('datos\_empresa'\[ID\_Producto]) \&\&

&nbsp;               ('datos\_empresa'\[Tipo\_Movimiento] = "Compra" || 'datos\_empresa'\[Tipo\_Movimiento] = "Produccion")

&nbsp;           ),

&nbsp;           'datos\_empresa'\[Costo\_Unitario]

&nbsp;       )

&nbsp;       ```



3\.  \*\*Visualización y Diseño de Informes:\*\*

&nbsp;   -   Se diseñó un dashboard en una sola página que responde a las tres preguntas de negocio.

&nbsp;   -   Se utilizaron objetos visuales de tarjeta (KPIs), gráficos de barras y un gráfico de líneas para mostrar tendencias.

&nbsp;   -   La \*\*interactividad\*\* es la característica clave: el filtrado cruzado entre visualizaciones y los segmentadores permiten una exploración profunda de los datos.



\## 🚀 Cómo Explorar el Análisis



\-   \*\*Para ver el resultado:\*\* Descarga el archivo `Dashboard\_Stock\_PowerBI.pbix` y ábrelo con Power BI Desktop (disponible de forma gratuita en la Microsoft Store).

\-   \*\*Para una vista rápida:\*\* Consulta la imagen `screenshot\_dashboard\_powerbi.png`.

