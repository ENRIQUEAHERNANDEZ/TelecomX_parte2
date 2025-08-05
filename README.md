# TelecomX_parte2
# 📊 Telecom X — Predicción de Cancelación de Clientes (Churn) | Fase Avanzada

Este proyecto retoma el análisis de churn para **Telecom X**, con un enfoque más técnico y predictivo. Aplicamos técnicas estadísticas, regresión lineal y modelos de machine learning para identificar los factores que influyen en la cancelación de clientes y predecir con mayor precisión su comportamiento.

---

## 🧠 Objetivo

Analizar, transformar y modelar los datos para:

- Predecir si un cliente cancelará su servicio.
- Identificar las variables más influyentes en esa decisión.
- Evaluar y comparar el rendimiento de diferentes modelos.
- Proponer estrategias de retención basadas en los resultados.

---

## 📁 Archivos utilizados

- `TelecomX_Data2.csv`: dataset limpio con variables relevantes para el modelado.
- Este `README.md`: resumen de la fase avanzada del proyecto.

---

## ✅ Pasos realizados

### 1. **Preparación de los datos**
- Eliminación de columnas irrelevantes como `customerID`.
- Codificación de variables categóricas con **One-Hot Encoding**.
- Detección y tratamiento de **valores nulos** con `SimpleImputer`.

### 2. **Análisis estadístico y correlación**
- Visualización de la **matriz de correlación** entre variables numéricas.
- Análisis gráfico entre variables clave (`tenure`, `TotalCharges`) y churn.
- Identificación de variables más correlacionadas con la cancelación.

### 3. **División del dataset**
- Separación en **80% entrenamiento** y **20% prueba** usando `train_test_split`.
- Estratificación para mantener el balance de clases en ambos subconjuntos.

### 4. **Modelado Predictivo**
- Modelo 1: **Regresión Logística** (requiere normalización)
- Modelo 2: **Random Forest** (no requiere normalización)
- Uso de `Pipeline` para automatizar normalización e imputación.

### 5. **Evaluación de modelos**
- Métricas utilizadas:
  - Exactitud (Accuracy)
  - Precisión
  - Recall (Sensibilidad)
  - F1-Score
  - Matriz de Confusión
- Comparación de desempeño entre los modelos.

### 6. **Interpretación de resultados**
- En Regresión Logística:
  - Análisis de **coeficientes**: muestra influencia directa de cada variable.
- En Random Forest:
  - **Importancia de variables** basada en la reducción de impureza.

---

## 🧾 Principales hallazgos

- **Contrato mensual** y **facturación electrónica** aumentan el riesgo de cancelación.
- Clientes con **menos tiempo (`tenure`)** o **cargos mensuales altos** tienen mayor probabilidad de abandonar.
- El modelo de **Random Forest** fue el que tuvo mejor desempeño predictivo en este análisis.

---

## 🚀 Herramientas utilizadas

- Python
- Pandas / NumPy
- Scikit-learn
- Seaborn / Matplotlib
- Jupyter Notebook

---

## 📌 Próximos pasos

- Ajuste de hiperparámetros con `GridSearchCV`.
- Aplicación de técnicas para **desbalance de clases** (SMOTE, `class_weight`).
- Generación de dashboards o visualizaciones interactivas para stakeholders.

---

## 👨‍💻 Autor

**Enrique A. Hernández**  
Analista de Datos | Proyecto Telecom X

