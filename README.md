# ceia-ml

# Universidad de Buenos Aires
### Carrera de Especialización en Inteligencia Artificial
### Cohorte 22 - Año 2025

# Proyecto Final de Machine Learning

## Integrantes
- [SIU a2208] Ariel Matias Cabello <arielmcabello@gmail.com>
- [SIU a2213] Ignacio Agustin Costarelli <agustin@costarellisa.com.ar>
- [SIU a2214] Alex Martín Curellich <alexcurellich@gmail.com>

<br>

## Dataset
**Tertiary Mushroom: 1 Million More Mushrooms** – [Kaggle](https://www.kaggle.com/datasets/carlmcbrideellis/tertiary-mushroom-1-million-more-mushrooms)

## 1. Descripción General
Este proyecto constituye la aplicación práctica de los conceptos aprendidos en la materia Aprendizaje Máquina. Se desarrolla el proceso completo de trabajo de Machine Learning sobre un problema de *clasificación supervisada*, con el objetivo de predecir si un hongo es comestible o venenoso a partir de sus características.


El trabajo sigue el siguiente ciclo:
1. Análisis Exploratorio de Datos (EDA)
2. Preprocesamiento y preparación de datos
3. Modelización (entrenamiento y validación)
4. Evaluación de resultados
5. Conclusiones y comunicación de hallazgos

---

## 2. Descripción del Dataset
El dataset contiene 1 millón de registros aproximadamente con descripciones de hongos, cada uno identificado por una serie de características categóricas (forma del sombrero, color, superficie, olor, etc.) y una etiqueta objetivo que indica si el hongo es **comestible (edible)** o **venenoso (poisonous)**.


**Características principales:**
- Total de instancias: ~1.000.000
- Tipo de variables: categóricas
- Variable objetivo: `class` (edible / poisonous)


**Fuente:** Kaggle – *Carl McBride Ellis (2021)*.

## 4. Estructura del Proyecto
```
ceia-ml/
│ 
├── dataset/
│ └── proyecto_mushrooms.ipynb 
├── README.md 
├── Trabajo final ML I.ipynb
├── petry.lock
└── pyproject.toml
```
---
## 5. Flujo de Trabajo

### 5.1 Análisis Exploratorio de Datos (EDA)
- Inspección de tipos de variables y valores nulos.
- Análisis de balance de clases.
- Gráficos de distribución de variables más relevantes.
- Detección de correlaciones entre características (después de codificar categorías).
- Identificación de posibles problemas de calidad de datos.


### 5.2 Preprocesamiento y Preparación
- ....


### 5.3 Modelización
Se optó por el **enfoque comparativo** (Opción B), evaluando modelos de distinta naturaleza:
1. **Regresión Logística** – Modelo base lineal.
2. **Random Forest** – Modelo basado en árboles con votación.
...


Cada modelo se entrenó y validó mediante un conjunto de prueba del 20%, manteniendo la proporción de clases. 


### 5.4 Evaluación de Resultados
Se emplearon las siguientes métricas:
- *Accuracy*
- *Precision*
- *Recall*
- *F1-score*
- *ROC-AUC*


Además, se visualizaron:
- Matrices de confusión.
- Curvas ROC comparativas.
- Importancia de características para modelos basados en árboles.