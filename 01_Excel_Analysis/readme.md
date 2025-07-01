\# Análisis de Stock y Ventas con Microsoft Excel



Esta carpeta contiene el análisis del ciclo de vida de productos realizado íntegramente en Microsoft Excel, utilizando sus capacidades modernas de Business Intelligence.



\## 📁 Archivos



\-   `Analisis\_Stock\_Excel.xlsx`: El libro de Excel que contiene el análisis completo.



\## 🛠️ Metodología Utilizada



El enfoque de este análisis se centra en las mejores prácticas para evitar el uso de hojas de cálculo masivas y fórmulas volátiles.



1\.  \*\*Transformación de Datos (ETL) con Power Query:\*\*

&nbsp;   -   Los datos brutos del archivo `datos\_empresa.csv` se importaron y limpiaron utilizando el Editor de Power Query.

&nbsp;   -   Las operaciones de limpieza incluyeron: normalización de nombres de productos, corrección de tipos de datos y manejo de valores atípicos.



2\.  \*\*Modelado de Datos con Power Pivot y DAX:\*\*

&nbsp;   -   Los datos limpios se cargaron en el Modelo de Datos de Excel (Power Pivot).

&nbsp;   -   Se crearon columnas calculadas y medidas utilizando DAX (Data Analysis Expressions) para calcular métricas clave como:

&nbsp;       -   `Ingresos`

&nbsp;       -   `Coste\_Venta`

&nbsp;       -   `Margen`

&nbsp;       -   `Stock Final`



3\.  \*\*Visualización con Tablas y Gráficos Dinámicos:\*\*

&nbsp;   -   La hoja de cálculo `Dashboard` contiene las visualizaciones finales.

&nbsp;   -   Se utilizaron tablas y gráficos dinámicos conectados al Modelo de Datos para responder a las preguntas de negocio.

&nbsp;   -   Se implementaron segmentaciones de datos (`slicers`) para permitir la interactividad del informe.



\## 🚀 Cómo Explorar el Análisis



1\.  Abre el archivo `Analisis\_Stock\_Excel.xlsx`.

2\.  Ve a la pestaña \*\*Datos > Consultas y conexiones\*\* para ver la consulta de Power Query.

3\.  Ve a la pestaña \*\*Power Pivot > Administrar\*\* para explorar el Modelo de Datos y las fórmulas DAX.

4\.  Interactúa con los filtros en la hoja `Dashboard` para explorar los resultados.

