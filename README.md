# Challenge-Telcom_X_2
Desarrollar modelos predictivos capaces de prever qué clientes tienen mayor probabilidad de cancelar sus servicios.

# 📌 Descripción del Proyecto

  Este proyecto desarrolla un pipeline de Machine Learning para predecir la cancelación de clientes (churn) en una empresa de      telecomunicaciones.

  El objetivo es identificar qué clientes tienen mayor probabilidad de abandonar el servicio, permitiendo a la empresa      implementar estrategias de retención proactivas.

  El proyecto incluye:

  - Preparación y limpieza de datos

  - Ingeniería de características

  - Balanceo de clases

  - Selección de variables

  - Construcción de modelos predictivos

  - Interpretación de variables importantes

  Este trabajo corresponde al Challenge Telecom X – Parte 2, enfocado en la etapa de modelado predictivo.

# 🎯 Objetivos

  - Construir modelos predictivos para identificar clientes con riesgo de cancelación.

  - Preparar los datos mediante técnicas de limpieza y transformación.

  - Manejar el desbalance de clases en la variable objetivo.

  - Comparar diferentes algoritmos de Machine Learning.

  - Analizar las variables más influyentes en el churn.

# 🗂️ Dataset

El análisis utiliza dos datasets previamente tratados:

1. Data.csv
Contiene todas las variables originales, con respuestas binarias en formato texto (Sí / No).

2. Data_binaria.csv
Versión procesada donde las variables binarias fueron convertidas a formato numérico (0 / 1), facilitando el análisis estadístico y el modelado.

# ⚙️ Preparación de los Datos
- Eliminación de variables irrelevantes

- Se eliminaron columnas que no aportaban valor predictivo o podían generar ruido en el modelo.

- Codificación de variables categóricas

- Se aplicó One-Hot Encoding a las variables nominales:

    Genero_cliente
  
    Sus_Internet
  
    Tipo_Contrato
  
    Metodo_de_Pago

- Esto permitió convertir las categorías en variables binarias para su uso en modelos de Machine Learning.

- Manejo de valores faltantes

- Se detectaron 11 valores NaN en la variable Gasto_Total, los cuales fueron imputados utilizando la media de la variable.

- Balanceo de clases

- El dataset presentaba desbalance en la variable objetivo (Permanencia / Churn).

Para corregirlo se aplicó:

- SMOTE (Synthetic Minority Over-sampling Technique)

Esto permitió equilibrar el dataset hasta obtener:

- 50% clientes que permanecen

- 50% clientes que cancelan

- Normalización de variables

Se aplicó StandardScaler a variables numéricas:

- Meses_del_Contrato

- Gasto_Mensual

- Gasto_Total

- Cuentas_Diarias

Esto garantiza que todas las variables contribuyan de forma equilibrada al modelo, especialmente en algoritmos basados en distancia como KNN.

# 🤖 Modelos Predictivos

Se desarrollaron los siguientes modelos:

- 📌 Modelo Baseline

Modelo de referencia para comparar el rendimiento de los modelos posteriores.

- 🌳 Árbol de Decisión

Modelo basado en reglas que permite interpretar fácilmente las decisiones del algoritmo.

- 📍 K-Nearest Neighbors (KNN)

Modelo basado en distancia que clasifica clientes según la similitud con otros clientes.

# 📊 Evaluación de Modelos

Los modelos fueron evaluados mediante:

- Matriz de confusión

- Recall

El recall fue priorizado porque el objetivo es identificar correctamente a los clientes que cancelarán.

# 🔑 Importancia de Variables
Variables más importantes para predecir churn

Los modelos coincidieron en varios factores clave:

1️⃣ Meses del contrato

La variable más consistente en ambos modelos.

Clientes con menos tiempo en la empresa tienen mayor probabilidad de cancelar.

2️⃣ Tipo de contrato (Mes a mes)

El predictor más fuerte en el Árbol de Decisión.

Clientes con contrato mensual presentan mayor churn.

3️⃣ Tipo de internet (Fibra óptica)

Relacionado con mayor cancelación, posiblemente por expectativas altas del servicio.

4️⃣ Método de pago (Electronic check)

Clientes que utilizan este método presentan mayor probabilidad de abandonar el servicio.

# 🛠️ Tecnologías Utilizadas

- Python

- Pandas

- NumPy

- Scikit-Learn

- Matplotlib

- Seaborn

- Imbalanced-Learn

- Jupyter Notebook

# 🚀 Cómo ejecutar el proyecto

1️⃣ Clonar el repositorio

git clone https://github.com/CarloR04/Challenge-Telcom_X_2.git

2️⃣ Entrar al directorio

cd Challenge-Telcom_X_2

3️⃣ Instalar dependencias

pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn

4️⃣ Ejecutar el notebook

jupyter notebook


## ✒️ Mentores ✒️

Con mucho agradecimiento por el conocimiento impartido a los tutores de Alura Latam: 

- Alvaro Camacho https://github.com/ahcamachod

## 👤 Autor

| [<img src="https://avatars.githubusercontent.com/u/225071618?v=4&size=64" width=115><br><sub>Carlo Robles</sub>](https://github.com/CarloR04) |  
| :---: |


Carlos Robles
Ingeniero Industrial | Data Analytics & Data Engineering Jr

📍 Colombia
