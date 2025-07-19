# Análisis de Obesidad y Estilos de Vida mediante Minería de Datos

## Visión General del Proyecto

Este proyecto realiza un análisis exhaustivo del dataset "Estimation of Obesity Levels" para descubrir patrones y relaciones ocultas entre los hábitos de vida y los niveles de obesidad. Se aplicaron diversas técnicas de minería de datos para entrenar, evaluar y comparar diferentes modelos predictivos y de segmentación.

El resultado final es un **dashboard web interactivo** que visualiza los hallazgos de cada modelo, presentando los insights más relevantes de una manera clara y accionable.

## 📊 Dashboard Interactivo

El dashboard centraliza los resultados de todos los modelos, permitiendo una exploración visual de los datos y los insights clave.

_**[INSERTA AQUÍ UNA CAPTURA DE PANTALLA DE TU DASHBOARD, COMO LA SIGUIENTE]**_
![Dashboard Screenshot](https://raw.githubusercontent.com/Rektres/DM_Obesity/main/Images/dashboard_preview.png)  ## 🤖 Modelos Implementados

Se exploraron 5 modelos de minería de datos, cada uno con un objetivo específico:

1.  **Reglas de Asociación (Apriori):**
    * **Objetivo:** Descubrir qué hábitos o características suelen ocurrir juntos con frecuencia.
    * **Insight Clave:** Se encontró una fuerte asociación entre el sedentarismo en adultos mayores y el sobrepeso, incluso cuando el consumo de agua es alto, desafiando la creencia de que una buena hidratación compensa la falta de ejercicio en este grupo.

2.  **Regresión Lineal:**
    * **Objetivo:** Predecir la edad de una persona basándose en sus hábitos y características físicas.
    * **Insight Clave:** El modelo demostró que las variables de estilo de vida explican menos del 50% de la variabilidad de la edad, indicando que una relación lineal es insuficiente y se necesitan modelos más complejos o variables adicionales.

3.  **Naive Bayes:**
    * **Objetivo:** Clasificar a una persona como "Enferma" o "No enferma" basándose en sus datos.
    * **Insight Clave:** El modelo es muy bueno identificando a personas enfermas (Recall del 93%), pero débil para identificar a las sanas. Esto lo convierte en una excelente herramienta de **pre-diagnóstico (screening)**, pero no de diagnóstico definitivo.

4.  **Árbol de Decisión:**
    * **Objetivo:** Crear un modelo de reglas claras para predecir el nivel de obesidad.
    * **Insight Clave:** El **peso corporal actual es el predictor más importante**, superando a variables de comportamiento como la dieta o el ejercicio. Esto sugiere que las intervenciones de salud deben segmentar primero por peso y luego personalizar según los hábitos.

5.  **Clustering (K-Means):**
    * **Objetivo:** Agrupar a las personas en segmentos con características similares, sin conocer previamente su nivel de obesidad.
    * **Insight Clave:** Se identificó un clúster de alto riesgo: personas con alto peso y sedentarismo que usan el transporte público. Esto es contraintuitivo, ya que el transporte público se considera una alternativa activa al coche, revelando un nicho específico para campañas de salud.

## 🛠️ Tecnologías Utilizadas

* **Análisis y Modelado:**
    * Python 3
    * Pandas
    * Scikit-learn
    * Mlxtend
    * Jupyter Notebook
* **Visualización de Datos:**
    * Matplotlib
    * Seaborn
    * Plotly.js
* **Dashboard:**
    * HTML5
    * CSS3
    * JavaScript

## 🚀 Cómo Empezar

### 1. Análisis de Datos (Jupyter Notebook)

Para explorar el proceso de análisis y entrenamiento de modelos:

1.  Clona este repositorio:
    ```bash
    git clone [https://github.com/Rektres/DM_Obesity.git](https://github.com/Rektres/DM_Obesity.git)
    ```
2.  Asegúrate de tener instaladas las librerías necesarias:
    ```bash
    pip install pandas scikit-learn mlxtend matplotlib seaborn jupyter
    ```
3.  Ejecuta Jupyter Notebook y abre el archivo `BIY7121_001V_ET_GINI_AranedaMateo_PerezRoberto.ipynb`.

### 2. Dashboard Interactivo

Para ver el resultado final, simplemente abre el archivo `index.html` en tu navegador web preferido.

## 👥 Autores

* **Mateo Araneda**
* **Roberto Pérez**
