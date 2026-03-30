# ml-esports-analysis

# 🎮 Análisis y Predicción de Rendimiento en E-Sports (Machine Learning)

## 📌 Objetivo del Proyecto
Este proyecto tiene como objetivo analizar estadísticas detalladas de partidas competitivas de E-Sports (CS:GO) y desarrollar modelos de Machine Learning capaces de estimar y predecir el desempeño individual de un jugador en tiempo real. 

El análisis se centra en dos enfoques predictivos principales:
1. **Predicción de Bajas (MatchKills):** Mediante un modelo de regresión que evalúa el impacto de variables clave como tiros a la cabeza (*Headshots*), asistencias, economía de la ronda y tipo de arma principal.
2. **Clasificación de Nivel:** Un modelo diseñado para predecir la categoría de rendimiento del jugador (ej. *Intermedio*) basándose en su comportamiento estadístico y toma de decisiones en el juego.

## 🛠️ Tecnologías y Herramientas
El proyecto fue desarrollado íntegramente en **Python** utilizando **Google Colab/Jupyter Notebook**. El ecosistema tecnológico incluye:
* **Manipulación de Datos y Limpieza:** `pandas`, `numpy`
* **Visualización de Datos:** `matplotlib`, `seaborn`
* **Machine Learning & Modelado Estadístico:** `scikit-learn` (GridSearchCV, MinMaxScaler) y `statsmodels` (Regresión OLS).
* **Despliegue de Interfaz de Usuario:** `ipywidgets` (formularios dinámicos).

## 📊 Resultados y Rendimiento de los Modelos
Tras el análisis exploratorio (EDA), la limpieza de datos atípicos y la selección de variables (mediante matrices de correlación y evaluación del Valor-P), se entrenaron los siguientes modelos:

* **Modelo de Regresión (OLS - Statsmodels):** Se logró un modelo robusto y altamente predictivo para estimar las bajas del jugador en la partida, obteniendo un coeficiente de determinación **R² de 0.754**.
* **Modelo de Clasificación (Scikit-Learn):** Tras aplicar técnicas de validación cruzada y optimización de hiperparámetros (*GridSearchCV*), el modelo alcanzó una **efectividad predictiva del 73.12%**.

## 🚀 Cómo interactuar con el modelo
Para demostrar la puesta en producción de los algoritmos, la libreta incluye **formularios interactivos** al final del documento. 

Para utilizarlos:
1. Descarga el archivo `Informe_EXAMEN.ipynb` y ábrelo en tu entorno local (Jupyter) o súbelo a Google Colab.
2. Ejecuta todas las celdas de la libreta.
3. En la sección final, ajusta los *sliders* y menús desplegables con las estadísticas simuladas de un jugador (ej. *RoundStartingEquipmentValue*, *PrimarySniperRifle*, etc.).
4. Haz clic en el botón **"Predecir MatchKills"** o **"Predecir categoría"** para ver el resultado arrojado por el modelo en tiempo real.
