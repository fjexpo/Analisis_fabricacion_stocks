\# Análisis de Ciclo de Vida de Producto: De la Compra a la Venta





\_Ejemplo del dashboard final generado con Python y Matplotlib.\_



\## 🚀 Resumen del Proyecto



Este repositorio contiene un \*\*análisis de datos de extremo a extremo\*\* que simula el ciclo operativo de una empresa de electrónica de consumo. El objetivo es evaluar y comparar la eficacia de tres herramientas líderes en Business Intelligence: \*\*Excel (con Power Query/Pivot)\*\*, \*\*Power BI\*\* y \*\*Python (Pandas, Matplotlib)\*\*, para resolver problemas de negocio reales.



El análisis abarca desde la \*\*limpieza y transformación\*\* de datos brutos hasta la creación de un \*\*dashboard ejecutivo\*\* que responde a preguntas estratégicas sobre rentabilidad, gestión de inventario y tendencias de mercado.



---



\## 🎯 Desafío de Negocio



La dirección de la empresa necesita respuestas claras a las siguientes preguntas para guiar su estrategia en el próximo trimestre:



1\.  \*\*Análisis de Rentabilidad:\*\* ¿Cuáles son nuestros \*\*3 productos más rentables y los 2 menos rentables\*\* en términos de margen bruto total durante el último año fiscal (2023)?

2\.  \*\*Gestión de Inventario:\*\* ¿Qué productos tienen una \*\*baja rotación de stock\*\*, sugiriendo un posible exceso de inventario, y cuáles corren riesgo de \*\*rotura de stock\*\*?

3\.  \*\*Detección de Anomalías:\*\* ¿Existe alguna \*\*tendencia de ventas preocupante\*\* o anómala para algún producto en el último semestre que requiera atención inmediata?



---



\## 🗃️ El Dataset



Para abordar este desafío, se generó un dataset sintético (`datos\_empresa.csv`) que simula transacciones reales.



\-   \*\*Tamaño:\*\* 6,000 filas y 10 columnas.

\-   \*\*Periodo:\*\* 01 de Enero de 2022 a 31 de Mayo de 2024.

\-   \*\*Contenido:\*\* Registros de `Compra` de componentes, `Producción` de productos finales y `Ventas` a clientes.



\### ⚠️ Problemas Inyectados Deliberadamente



Para que el desafío fuera realista, se introdujeron 4 problemas de calidad de datos que cualquier analista se encontraría en el mundo real:



| # | Tipo de Problema | Descripción del Desafío | Habilidad Puesta a Prueba |

| :-- | :--- | :--- | :--- |

| 1 | \*\*Consistencia\*\* | El producto "Procesador Gamma" aparece como "Procesador Gama". | Normalización de datos categóricos. |

| 2 | \*\*Outlier\*\* | Una venta se registra con una cantidad irreal de -5000 unidades. | Detección y manejo de valores atípicos. |

| 3 | \*\*Tipo de Dato\*\* | El `Costo\_Unitario` contiene valores de texto como "NO DISPONIBLE". | Limpieza y conversión de tipos de datos. |

| 4 | \*\*Anomalía\*\* | Las ventas de un producto caen a cero en los últimos 4 meses. | Análisis de series temporales y detección de insights. |



---



\## 🛠️ Metodología de Análisis



El análisis sigue un flujo de trabajo estructurado, replicado en cada una de las tres herramientas evaluadas.



\### 1. Carga y Exploración de Datos

\-   Importación del archivo CSV.

\-   Inspección inicial para identificar tipos de datos incorrectos, valores nulos y estadísticas descriptivas anómalas.



\### 2. Limpieza y Transformación (ETL)

\-   \*\*Corrección de Errores:\*\* Se aplicaron técnicas de reemplazo, imputación y normalización para resolver los problemas de calidad de datos.

\-   \*\*Enriquecimiento de Datos (Feature Engineering):\*\* Se crearon nuevas columnas calculadas para habilitar el análisis de negocio:

&nbsp;   -   `Ingresos`: `Precio de Venta \* Unidades Vendidas`

&nbsp;   -   `Coste\_Venta`: `Costo Promedio de Adquisición \* Unidades Vendidas`

&nbsp;   -   `Margen`: `Ingresos - Coste\_Venta`

&nbsp;   -   `Stock\_Acumulado`: Cálculo del inventario disponible a lo largo del tiempo por producto.



\### 3. Visualización y Creación de Dashboards

\-   Se diseñaron visualizaciones específicas para responder a cada una de las preguntas de negocio.

\-   Los gráficos y KPIs clave se consolidaron en un dashboard final para facilitar la toma de decisiones.



---



\## 📊 Resultados y Hallazgos Clave



El análisis reveló insights críticos para la estrategia de la compañía:



\#### \*\*Insight 1: La Rentabilidad está Altamente Concentrada\*\*

\-   El \*\*"Portátil Z1 Pro"\*\* es el principal motor de rentabilidad de la empresa.

\-   La \*\*"Tarjeta Gráfica Eco"\*\* genera márgenes negativos, erosionando la rentabilidad global.

\-   \*\*Acción Recomendada:\*\* Revisar la estructura de costes y precios de los productos de bajo rendimiento o considerar su descontinuación.



&nbsp;<!-- Reemplaza con la URL de tu gráfico de rentabilidad -->



\#### \*\*Insight 2: Desequilibrios Críticos en el Inventario\*\*

\-   \*\*Exceso de Stock:\*\* El \*\*"Monitor Curvo 27''"\*\* presenta un inventario acumulado excesivo debido a una caída en la demanda no gestionada.

\-   \*\*Riesgo de Rotura:\*\* El \*\*"SSD 512GB"\*\* muestra ventas que superan su ritmo de aprovisionamiento, arriesgando pérdida de ventas.

\-   \*\*Acción Recomendada:\*\* Ajustar los planes de compra y producción basándose en la rotación real del stock.



&nbsp;<!-- Reemplaza con la URL de tu gráfico de stock -->



\#### \*\*Insight 3: ¡ALERTA ROJA! Anomalía de Ventas Detectada\*\*

\-   El \*\*"Monitor Curvo 27''"\*\* ha sufrido un \*\*colapso total en sus ventas\*\* en los últimos 4 meses del periodo analizado.

\-   \*\*Acción Urgente:\*\* Iniciar una investigación inmediata para determinar la causa raíz (problema de calidad, acción de la competencia, fallo en el canal de venta) y \*\*detener la producción\*\* de este artículo.



&nbsp;<!-- Reemplaza con la URL de tu gráfico de tendencias -->



---



\## 💻 Cómo Ejecutar este Análisis



\### Prerrequisitos

\-   Python 3.8+

\-   Jupyter Notebook / Google Colab (recomendado)



\### Instalación

1\.  Clona este repositorio:

&nbsp;   ```bash

&nbsp;   git clone https://github.com/tu-usuario/tu-repositorio.git

&nbsp;   cd tu-repositorio

&nbsp;   ```

2\.  Instala las dependencias necesarias:

&nbsp;   ```bash

&nbsp;   pip install -r requirements.txt

&nbsp;   ```



\### Ejecución

1\.  Abre el archivo `Analisis\_Productos.ipynb` en tu entorno de Jupyter.

2\.  Asegúrate de que el archivo `datos\_empresa.csv` está en el mismo directorio.

3\.  Ejecuta las celdas del notebook en orden para replicar el análisis completo.



---

\_Este proyecto demuestra la capacidad de transformar datos brutos y complejos en insights de negocio accionables, una habilidad clave para cualquier rol de Data Analyst.\_

