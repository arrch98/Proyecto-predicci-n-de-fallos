# Detección de Anomalías y Predicción de Fallos en el Sistema de Producción de Aire (APU) 
## Descripción del proyecto
Este proyecto aplica técnicas de machine learning para detectar anomalías y predecir fallos en el sistema de producción de aire (APU) de trenes, una unidad crítica que alimenta sistemas como los frenos y la suspensión neumática. El trabajo se desarrolla en el contexto de la asignatura Modelos Predictivos, integrando análisis de datos, modelado y visualización en Python.
## Objetivo
Desarrollar modelos de clasificación que permitan anticipar fallos en la APU de trenes urbanos, optimizando el mantenimiento predictivo y reduciendo interrupciones en el servicio.
## Dataset
- Nombre: Railway Air Compressor Dataset. 
- Registros: 1,516,948 observaciones
- Variables: 15 señales sensóricas (presiones, temperatura, corriente, señales binarias de válvulas, etc.)
- Variable objetivo: Failure (1 si hubo falla, 0 si no)

Fuente: UCI Machine Learning Repository https://archive.ics.uci.edu/dataset/791/metropt+3+dataset
## Herramientas utilizadas
- Python (Jupyter Notebook): limpieza de datos, ingeniería de variables, visualización y modelado.
- Pandas / NumPy / Scikit-learn / Matplotlib / Seaborn: librerías clave para manipulación y análisis.
- Excel: revisión de estructuras de datos y comprensión del comportamiento del sistema.

## Pasos del proyecto

1. Revisión técnica de la base de datos y documentación de fallos históricos.
2. Preprocesamiento:
   - Generación de la variable objetivo (Failure) según intervalos de tiempo registrados.
   - Verificación de valores nulos y análisis de outliers.
3. Análisis descriptivo:
   - Estadísticas generales.
   - Correlaciones relevantes con la variable objetivo.
   - Visualización de tendencias antes, durante y después de fallos.
4. Selección de variables predictoras.
5. Entrenamiento de modelos de clasificación:
   - Regresión logística
   - Random Forest
   - K-Nearest Neighbors (KNN)
6. Evaluación de modelos mediante métricas como Accuracy, Precision, Recall, ROC AUC, RMSE, MAE y MAPE seguro.
7. Conclusión
8. Propuestas de mejoras.

## Descubrimientos principales
- La presión diferencial (DV_pressure) mostró alta correlación con los fallos.
- Las señales binarias como DV_electric y COMP reflejan claramente los estados operativos del compresor.
- Random Forest fue el modelo con mejor rendimiento, alcanzando un ROC AUC de 0.999 y un MAPE seguro de solo 1.14%.
 
## Recomendaciones y trabajos futuros

- Ajustar el enfoque hacia la predicción anticipada del fallo (no solo su detección).
- Incorporar agregaciones de ventanas temporales y modelos secuenciales.
- Explorar el uso de autoencoders o modelos LSTM para identificar desviaciones tempranas.
- Enriquecer el dataset con variables contextuales como carga operativa o condiciones externas.
- Crear dashboards para monitoreo en tiempo real de APU.
  
## Autor
**Ángel Reyes**


Universidad Tecnológica de Panamá
