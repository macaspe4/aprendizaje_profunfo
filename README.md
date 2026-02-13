# Análisis de Agotamiento y Aislamiento Social (2026)
Este proyecto utiliza técnicas de Deep Learning para clasificar el nivel de burnout en trabajadores remotos.

## 1. Problema a resolver
El objetivo es predecir la categoría de agotamiento (Bajo, Medio, Alto) basándose en métricas de actividad y aislamiento. 

## 2. Dataset
- Nombre: Agotamiento de trabajo remoto y aislamiento social (2026)
- Variables de entrada (X): user_id, day_type, work_hours, screen_time_hours, meetings_count, breaks_taken, after_hours_work, app_switches, sleep_hours, task_completion, isolation_index, fatigue_score, burnout_score,
- Variable de salida (y): Nivel de Burnout (burnout_risk)

## 3. Estado del Arte
| Modelo              | Accuracy | F1-Macro | Tipo            |
| ------------------- | -------- | -------- | --------------- |
| Logistic Regression | 74%      | 0.72     | Baseline lineal |
| XGBoost             | 84%      | 0.81     | Boosting        |
| Random Forest       | 96.8%    | 0.93     | Ensemble        |
| MLP (objetivo)      | >95%     | >0.93    | Deep Learning   |

Según la documentación del dataset en Kaggle, modelos tradicionales como Logistic Regression alcanzan aproximadamente un 74% de accuracy, mientras que métodos de boosting como XGBoost alcanzan en torno al 84%.
Algunos usuarios han reportado resultados superiores utilizando Random Forest, llegando hasta 96% de accuracy, lo que sugiere que el dataset presenta patrones altamente separables.

## 4. Estructura del proyecto
- notebooks/: Contiene el Análisis Exploratorio de Datos (EDA).
- data/: Datos del proyecto.
- requirements.txt: Librerías necesarias.
