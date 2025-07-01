\# Análisis de Datos con Python



Esta carpeta contiene la implementación del análisis utilizando Python y sus librerías científicas, enfocado en la reproducibilidad y la personalización del análisis.



\## 📁 Archivos



\-   `Analisis\_Stock\_Python.ipynb`: Un Jupyter Notebook con todo el código del análisis, desde la limpieza hasta la visualización.

\-   `requirements.txt`: Un archivo que lista todas las dependencias de Python necesarias para ejecutar el notebook.



\## 🛠️ Metodología Utilizada



El enfoque de Python se centra en el control total sobre cada paso del proceso a través de código.



1\.  \*\*Carga y Limpieza de Datos con Pandas:\*\*

&nbsp;   -   Se utilizó la librería `pandas` para cargar el CSV en un DataFrame.

&nbsp;   -   La limpieza de datos se realizó programáticamente, corrigiendo tipos de datos, manejando valores nulos y outliers, y normalizando datos categóricos.



2\.  \*\*Enriquecimiento de Datos (Feature Engineering):\*\*

&nbsp;   -   Se crearon nuevas columnas (`Ingresos`, `Coste\_Venta`, `Margen`, `Stock\_Acumulado`) directamente en el DataFrame para facilitar los cálculos posteriores.



3\.  \*\*Análisis y Visualización con Matplotlib y Seaborn:\*\*

&nbsp;   -   Se realizaron agrupaciones (`groupby`) y agregaciones para calcular las métricas necesarias para responder a las preguntas de negocio.

&nbsp;   -   Se utilizaron las librerías `matplotlib` y `seaborn` para generar los gráficos y el dashboard final consolidado.



\## 🚀 Cómo Replicar el Análisis



\### Prerrequisitos

\-   Python 3.8 o superior.

\-   Tener instalado `pip` (el gestor de paquetes de Python).



\### Pasos

1\.  \*\*Clona el repositorio\*\* (si aún no lo has hecho) y navega a esta carpeta.

&nbsp;   ```bash

&nbsp;   cd 03\_Python\_Analysis

&nbsp;   ```

2\.  \*\*Crea un entorno virtual (recomendado):\*\*

&nbsp;   ```bash

&nbsp;   python -m venv venv

&nbsp;   source venv/bin/activate  # En Windows: venv\\Scripts\\activate

&nbsp;   ```

3\.  \*\*Instala las dependencias:\*\*

&nbsp;   ```bash

&nbsp;   pip install -r requirements.txt

&nbsp;   ```

4\.  \*\*Ejecuta el Jupyter Notebook:\*\*

&nbsp;   ```bash

&nbsp;   jupyter notebook Analisis\_Stock\_Python.ipynb

&nbsp;   ```

