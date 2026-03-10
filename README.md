# 📊 Telecom X – Predicción de Cancelación de Clientes (Churn)

## 📌 Descripción del Proyecto:
Este proyecto tiene como objetivo desarrollar modelos de Machine Learning capaces de predecir qué clientes tienen mayor probabilidad de cancelar su servicio (churn) en la empresa Telecom X.
Este proyecto corresponde a la segunda etapa del análisis del dataset de clientes de Telecom X.
🔗 Puedes consultar esa etapa aquí:

Telecom X – Parte 1: [Análisis Exploratorio](https://github.com/olicrea/Analisis-evasion-clientes)

En esta segunda etapa se desarrollan modelos predictivos de churn utilizando técnicas de clasificación.

## 🧠 Metodología

El flujo de trabajo seguido en este proyecto fue:

1️. Carga y revisión de datos procesados

2️. Codificación de variables categóricas (One-Hot Encoding)

3️. Análisis de correlación entre variables

4️. Análisis exploratorio de variables asociadas al churn

5️. Verificación de desbalance de clases

6️. División de datos en entrenamiento y prueba

7️. Normalización de variables numéricas

8️. Entrenamiento de modelos de clasificación

9️. Evaluación mediante métricas y curva ROC

10. Análisis de importancia de variables

11. Automatización del flujo mediante Pipelines

## 🤖 Modelos Utilizados

Se entrenaron dos modelos de clasificación:

### Logistic Regression

Modelo lineal que permite interpretar la influencia de las variables en la probabilidad de cancelación.

### Random Forest

Modelo basado en árboles de decisión que permite capturar relaciones más complejas entre variables.

### 📈 Evaluación de Modelos

Ambos modelos mostraron un desempeño similar, con un Recall superior al 80%, lo cual es especialmente relevante en problemas de churn, ya que permite identificar una mayor proporción de clientes con riesgo de abandono.

La evaluación mediante Curva ROC mostró un AUC cercano a 0.85, lo que indica una buena capacidad del modelo para distinguir entre clientes que cancelan y clientes que permanecen.

Debido a su ligera ventaja en recall, se seleccionó Random Forest como modelo principal para la detección de clientes en riesgo.

## 🔍 Factores Clave que Influyen en el Churn

El análisis de importancia de variables y los coeficientes del modelo permitieron identificar los principales factores asociados a la cancelación de clientes.

### Factores que aumentan el riesgo de cancelación



Estos resultados muestran que la estabilidad contractual y el tiempo de permanencia son factores clave en la retención de clientes.

## 📊 Principales Insights del Análisis

A partir del análisis exploratorio y de los modelos predictivos se identificaron varios patrones relevantes:

- Los clientes con contratos mensuales presentan mayor probabilidad de cancelar el servicio.

- Los clientes con menor tiempo de permanencia (tenure bajo) muestran mayor riesgo de abandono.

- Los usuarios de fibra óptica presentan tasas de churn más elevadas, posiblemente asociadas a precio o expectativas de servicio.

- Los clientes con mayor gasto mensual también presentan mayor riesgo de cancelación.

Además, el análisis visual mostró que muchos clientes cancelan durante los primeros meses de servicio, lo que sugiere que la etapa inicial de la relación con el cliente es crítica.

## 💡 Estrategias de Retención Recomendadas

A partir de los resultados obtenidos, se proponen las siguientes estrategias para reducir la cancelación de clientes:

#### - Incentivar contratos de largo plazo

Ofrecer descuentos o beneficios adicionales para fomentar contratos de uno o dos años.

#### - Implementar programas de retención temprana

Los primeros meses del cliente presentan mayor riesgo de churn. Se recomienda implementar estrategias de seguimiento o beneficios iniciales para mejorar la experiencia del cliente.

#### - Revisar la propuesta de valor de los planes de fibra óptica

Analizar precios, calidad del servicio y soporte técnico para identificar posibles causas de cancelación.

#### - Programas de fidelización para clientes de alto gasto

Ofrecer beneficios exclusivos o servicios adicionales a clientes con mayor gasto mensual.

#### - Fortalecer servicios de soporte técnico

El análisis muestra que los clientes con acceso a soporte técnico presentan menor tasa de cancelación.

## ⚙️ Tecnologías Utilizadas

Python

Pandas

NumPy

Matplotlib / Seaborn

Scikit-learn

Jupyter Notebook
