# DataSet-k-means_HC

# Análisis de Clustering de Clientes

Este proyecto implementa dos técnicas de clustering: K-Means y Clustering Jerárquico, para segmentar clientes basándose en su ingreso anual y puntuación de gastos.

## Descripción del Proyecto

El objetivo de este proyecto es identificar segmentos distintos de clientes utilizando dos enfoques de clustering. La segmentación se basa en dos características:
- `Ingreso Anual (k$)`: Ingresos anuales del cliente en miles de dólares.
- `Puntuación de Gastos (1-100)`: Puntuación asignada al cliente basada en su comportamiento de compra y gastos.

## Herramientas y Tecnologías Utilizadas

- **Python**: Lenguaje de programación.
- **Pandas**: Biblioteca de manipulación y análisis de datos.
- **Matplotlib** y **Seaborn**: Bibliotecas de visualización de datos.
- **Scikit-learn**: Biblioteca para machine learning que proporciona implementaciones de varios algoritmos de clustering.
- **Scipy**: Biblioteca utilizada para crear dendrogramas y realizar clustering jerárquico.

## Estructura del Proyecto

- `data_preparation.ipynb`: Notebook para la preparación y normalización de los datos.
- `kmeans_clustering.ipynb`: Notebook para aplicar y visualizar el clustering K-Means.
- `hierarchical_clustering.ipynb`: Notebook para realizar el análisis de clustering jerárquico y visualización del dendrograma.

## Descripción de los Notebooks:
data_preparation.ipynb:
## Preparación de Datos: Este notebook se encarga de cargar y preparar los datos para el análisis. Esto incluye la limpieza de datos (por ejemplo, manejar valores faltantes), la exploración inicial para entender las características y distribuciones de los datos, y la normalización de los datos si es necesario. La normalización es importante en el clustering porque los algoritmos como K-Means son sensibles a la escala de las variables.
kmeans_clustering.ipynb:
## Aplicación de K-Means: Utiliza el algoritmo de K-Means para segmentar a los clientes. Este proceso comienza seleccionando un número de clusters (k) que se podría basar en el método del codo, donde se elige el k que minimiza la variación dentro de los clusters mientras maximiza la variación entre clusters.
## Visualización: Después de aplicar K-Means, este notebook visualiza los clusters utilizando gráficos de dispersión, mostrando cómo los clientes son agrupados según sus ingresos y puntuaciones de gastos.
hierarchical_clustering.ipynb:
## Clustering Jerárquico: Este notebook implementa el clustering jerárquico, un método alternativo que no requiere la especificación de la cantidad de clusters de antemano. Se construye un dendrograma que ilustra cómo cada cluster se relaciona con los demás, permitiendo una interpretación visual de la agrupación.
## Corte del Dendrograma: Se decide un punto de corte en el dendrograma para definir el número de clusters, basado en la distancia entre fusiones que indica puntos naturales para dividir los clusters.
## Herramientas y Tecnologías Utilizadas:
- Python
- Pandas 
- Matplotlib y Seaborn son utilizados para la visualización de datos, permitiendo entender mejor los patrones subyacentes en los datos y los resultados del clustering.
- Scikit-learn proporciona una implementación eficiente y sencilla de utilizar de K-Means y otras herramientas útiles para la evaluación de modelos como métricas de silueta.
- Scipy es usado para el clustering jerárquico, especialmente para la creación de dendrogramas.
  
##Flujo del Proyecto:
###El flujo general del proyecto sigue estos pasos:
Preparación y exploración de datos para entender las características que influirán en el análisis de clustering.
Aplicación del clustering K-Means para identificar grupos basados en características seleccionadas.
Utilización del clustering jerárquico como método alternativo para proporcionar una perspectiva diferente sobre la segmentación de clientes.
Visualización de los resultados de ambos métodos para comparar y entender las diferencias en la segmentación.
Evaluación de los modelos para determinar la efectividad de cada enfoque de clustering en este contexto específico.
