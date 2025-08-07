# ChallangeTelecomX2

## Misión

Contribuir a la retención de clientes de empresas de telecomunicaciones mediante la identificación proactiva de aquellos con alta probabilidad de cancelación (churn), permitiendo la implementación de estrategias de retención dirigidas y efectivas.

## Objetivo del Desafío

El objetivo principal de este desafío es desarrollar y evaluar modelos de machine learning capaces de predecir la cancelación de clientes basándose en datos históricos de comportamiento y características demográficas. Se busca identificar los factores clave que influyen en el churn y proponer recomendaciones para la empresa.

## Descripción del Proyecto

Este proyecto aborda el problema de la cancelación de clientes (churn) en el sector de telecomunicaciones. Se utiliza un conjunto de datos de clientes para construir modelos predictivos que permitan identificar a los clientes en riesgo de irse. El análisis incluye la preparación de los datos, la exploración de variables relevantes, la creación y evaluación de diferentes modelos de clasificación, y la interpretación de los resultados para obtener insights accionables.

## Contenido

El repositorio contiene:

*   `datos_tratados.csv`: Archivo CSV con los datos de clientes preprocesados en una etapa anterior.
*   Notebook de Jupyter/Colab: Contiene el código Python para la carga, preprocesamiento, análisis exploratorio, modelado predictivo y evaluación de los modelos.
*   `README.md`: Este archivo, que describe el proyecto.

## Objetivo

El objetivo técnico es construir un modelo de clasificación robusto que pueda predecir la probabilidad de que un cliente cancele su servicio, con un enfoque en métricas relevantes para problemas de desbalance de clases como Recall y F1-score. El objetivo de negocio es proporcionar insights que permitan a la empresa reducir su tasa de churn.

## Estructura del Proyecto

El notebook sigue la siguiente estructura:

1.  **Preparación de los Datos:** Carga del dataset, eliminación de columnas irrelevantes, codificación de variables categóricas y manejo de datos faltantes.
2.  **Correlación y Selección de Variables:** Análisis de la relación entre las variables y la variable objetivo (cancelación), y selección de las características más relevantes.
3.  **Modelado Predictivo:** División de los datos en conjuntos de entrenamiento y prueba, creación y entrenamiento de modelos de clasificación (por ejemplo, Random Forest, Árbol de Decisión), y optimización de hiperparámetros.
4.  **Interpretación y Conclusiones:** Evaluación de los modelos utilizando métricas clave (Exactitud, Precisión, Recall, F1-score, Matriz de Confusión), análisis de la importancia de las variables en los modelos seleccionados y extracción de conclusiones y recomendaciones.

## Tecnologías Usadas

*   Python
*   Pandas (para manipulación de datos)
*   NumPy (para operaciones numéricas)
*   Matplotlib y Seaborn (para visualización de datos)
*   Scikit-learn (para modelado y evaluación de machine learning)
*   Imbalanced-learn (para manejo de desbalance de clases, si aplica)

## Cómo Usar Este Repositorio

1.  Clona el repositorio: `git clone [URL del repositorio]`
2.  Abre el notebook (en Google Colab o un entorno local de Jupyter).
3.  Asegúrate de tener el archivo `datos_tratados.csv` en la ubicación correcta o actualiza la ruta en el código.
4.  Ejecuta las celdas del notebook secuencialmente para replicar el análisis y los resultados.

## Conclusiones

Basándonos en el análisis de los datos, la construcción y evaluación de los modelos predictivos de cancelación, y la interpretación de la importancia de las variables, podemos extraer las siguientes conclusiones clave sobre los factores que más influyen en la cancelación de clientes y proponer estrategias de retención:

*   **Factores Clave que Influyen en la Cancelación:** El análisis exploratorio y la importancia de variables consistentemente destacaron que los clientes con **menos meses de contrato** y aquellos con **contratos mes a mes** tienen una probabilidad significativamente mayor de cancelar. Los clientes con **gastos totales acumulados más bajos** también mostraron una mayor propensión a la cancelación. Otras variables importantes incluyeron el tipo de proveedor de internet (Fibra Óptica) y el método de pago (Cheque Electrónico).

*   **Rendimiento del Modelo Seleccionado:** El modelo de **Árbol de Decisión optimizado** fue identificado como el más adecuado para este problema, principalmente por su mejor **Recall** y **F1-score**. Esto significa que este modelo es más efectivo para identificar correctamente a los clientes que *realmente* van a cancelar, lo cual es fundamental para poder intervenir a tiempo con estrategias de retención.

## Recomendaciones

Basándonos en los factores de cancelación identificados, se proponen las siguientes estrategias de retención:

*   **Programas de Bienvenida y Seguimiento Temprano:** Implementar un programa proactivo para los nuevos clientes, especialmente aquellos con contratos mes a mes, durante sus primeros meses. Esto podría incluir llamadas de seguimiento, ofertas especiales para contratos a más largo plazo después de un período inicial, o soporte técnico prioritario para asegurar una experiencia positiva desde el principio.
*   **Incentivos para Clientes de Bajo Gasto o Corta Antigüedad:** Ofrecer promociones o beneficios a clientes con bajo gasto total o poca antigüedad para incentivarlos a utilizar más servicios o a comprometerse con contratos más largos. Esto podría aumentar su valor para la empresa y reducir su riesgo de cancelación.
*   **Análisis Profundo de la Experiencia del Cliente en Puntos Críticos:** Investigar las razones específicas por las que los clientes con contratos cortos o bajo gasto total cancelan. Realizar encuestas de salida o análisis de comentarios para identificar problemas recurrentes en la experiencia del cliente (por ejemplo, problemas de facturación, calidad del servicio, atención al cliente) que puedan abordarse.
*   **Segmentación y Ofertas Personalizadas:** Utilizar los modelos predictivos para identificar a los clientes con alto riesgo de cancelación en función de los factores clave y ofrecerles estrategias de retención personalizadas. Esto podría incluir descuentos, mejoras de servicio, o soporte dedicado.

Al enfocarse en estos factores clave y aplicar estrategias de retención basadas en el análisis predictivo, la empresa puede trabajar de manera más efectiva para reducir la tasa de cancelación de clientes.
