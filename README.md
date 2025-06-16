Gracias por compartir el archivo del encargo docente. Con base en ese documento (`TRABAJO FINAL.pdf`) y en el código extenso que has desarrollado en R y Python, he actualizado el `README.md` para alinearlo con los criterios de evaluación y objetivos del curso **Laboratorio de Programación: R y Python – PUCP (2024-2)**.

Aquí tienes la versión final:

---

# 🧠 Predicción del Ingreso Laboral en Lambayeque

**Facultad de Ciencias Sociales – PUCP**
**Curso: Laboratorio de Programación – R y Python (2024-2)**

Este proyecto corresponde al **trabajo final** del curso y se enfoca en el desarrollo de un modelo predictivo de **ingresos laborales** para la región de **Lambayeque**, empleando herramientas de análisis de datos, visualización estadística y algoritmos de aprendizaje automático en **R y Python**.

---

## 👥 Integrantes

* Zarit Dafra de la Cruz (20211687)
* Angelly Gutiérrez (20210516)
* Anderson Águila (20215872)
* Jose Uriol (20203871)
* Carlo Llerena (20203126)

---

## 🎯 Objetivo del trabajo

Desarrollar un modelo de **machine learning** capaz de predecir los **ingresos laborales individuales** en base a variables sociodemográficas, educativas y laborales. Este modelo es evaluado y comparado mediante métricas como **MAPE**, **MPE**, **R²** y validación cruzada, según lo requerido en la rúbrica del curso.

---

## 🧱 Estructura del proyecto

```
ML-EXERCISE/
├── data/
│   ├── raw/                # Base original (formato Parquet)
│   ├── interm/             # Base intermedia (.csv)
│   └── final/              # Base limpia y recodificada (.xlsx)
│
├── graphs/                 # Visualizaciones (png)
├── docs/
│   └── TRABAJO FINAL.pdf   # Enunciado oficial del proyecto
│
├── programs/
│   ├── Para limpieza de base de datos.R   # Limpieza, recodificación y EDA en R
│   └── Machine Learning.ipynb             # Modelamiento en Python
│
└── README.md              # Descripción del proyecto (este archivo)
```

> ⚠️ **IMPORTANTE**: Colocar el archivo original `base_proyecto_final_.parquet` en la carpeta `data/raw/` para que los scripts se ejecuten correctamente.

---

## 🛠️ Herramientas utilizadas

### En R

* `tidyverse`, `arrow`, `corrplot`, `ggplot2`, `skimr`, `openxlsx`, `zoo`
* Análisis exploratorio, tratamiento de outliers, y visualización

### En Python

* `pandas`, `scikit-learn`, `matplotlib`, `seaborn`
* Modelos Lasso y Random Forest con `GridSearchCV`

---

## 🔍 Flujo metodológico

### 🔹 1. Limpieza y transformación de datos

* Conversión de `Parquet` a `CSV`
* Filtrado para el departamento de **Lambayeque**
* Recodificación de variables (educación, etnia, lengua materna, género, etc.)
* Eliminación selectiva de valores faltantes y tratamiento de *outliers*
* Guardado de base final como `.xlsx`

### 🔹 2. Análisis exploratorio (EDA)

* Histogramas, gráficos de densidad y barras
* Boxplots para detectar *outliers* según variables categóricas
* Matriz de correlación y detección de multicolinealidad
* Análisis bivariado (experiencia vs ingreso)

### 🔹 3. Modelado de predicción (ML)

* División **80/20** para entrenamiento y prueba
* Modelo **Lasso**:

  * Selección de variables vía `GridSearchCV`
  * Métrica principal: **MAPE**
* Modelo **Random Forest**:

  * Ajuste de hiperparámetros (`n_estimators`)
  * Reporte de métricas: MAPE, MPE, R², % dentro del ±20%
  * Evaluación de robustez con **validación cruzada**

---

## 📊 Resultados clave

* **Lasso** identificó como variables relevantes: educación, pobreza, experiencia, edad cuadrática y sector estatal.
* **Random Forest** presentó **mejor capacidad predictiva**, con menor MAPE y mayor robustez.
* Las **variables con mayor impacto positivo** sobre el ingreso fueron: educación superior, experiencia moderada, empleo en el sector privado, y trabajos altamente calificados.
* **Pobreza, edad avanzada y trabajo estatal** correlacionaron negativamente con el ingreso.

---

## 📈 Visualizaciones destacadas

Todas disponibles en `/graphs/`:

* Distribuciones: edad, ingresos, experiencia
* Frecuencias: sexo, educación, lengua materna, pobreza
* Boxplots: ingreso laboral por categorías
* Correlaciones: detección de multicolinealidad
* Dispersión ingreso vs. experiencia (lineal y cuadrática)
* Importancia de variables en Random Forest


