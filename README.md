# Análisis y Evaluación de Modelos Predictivos para Enfermedades Cardíacas

Este repositorio contiene dos notebooks diseñados para realizar un análisis exploratorio, preprocesamiento, entrenamiento y evaluación de modelos de clasificación orientados a predecir enfermedades cardíacas o eventos relacionados, utilizando tanto PySpark como bibliotecas clásicas de machine learning en Python.

## Notebooks incluidos

### 1. `Juan_Torres_PySpark_Taller_Metricas.ipynb`

Este notebook utiliza **PySpark** para el procesamiento distribuido de datos relacionados con enfermedades cardíacas. Las tareas realizadas incluyen:

- Carga de datos desde una fuente remota (CSV público).
- Verificación de valores nulos o inconsistentes.
- Análisis exploratorio mediante correlaciones.
- Visualización con mapas de calor.
- Discusión sobre posibles variables relevantes para modelado predictivo.

**Objetivo:** familiarizarse con el uso de PySpark para exploración y preparación de datos en entornos de Big Data.

---

### 2. `Juan_Torres_Stroke_Metricas.ipynb`

Este notebook aborda el entrenamiento y evaluación de un modelo de clasificación binaria para predecir eventos cardíacos:

- **Preprocesamiento**: imputación de valores faltantes y codificación de variables categóricas.
- **Entrenamiento**: modelo `DecisionTreeClassifier` con una profundidad máxima de 4.
- **Evaluación**: 
  - Matriz de confusión.
  - Cálculo de métricas como Accuracy, Sensitivity, Specificity y Precision.
  - Generación de curva ROC y cálculo de AUC.

**Resultados destacados:**

- Accuracy: 94.71 %
- Recall: 2.50 %
- Precision: 50.00 %
- AUC: 77 %

**Conclusión:** el modelo logra una alta exactitud y especificidad, pero presenta una baja sensibilidad, lo cual limita su utilidad para detectar casos positivos reales. Se sugieren estrategias como balanceo de clases o el uso de modelos más robustos.

---

## Requisitos

Para ejecutar los notebooks necesitas:

- Python 3.7+
- Bibliotecas: `pyspark`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`

Puedes instalar los requerimientos con:

```bash
pip install pyspark pandas numpy matplotlib seaborn scikit-learn
