# ML-Exercise

---

# Análisis de Datos Sociodemográficos y Predicción de Ingresos Laborales en Lambayeque

## Descripción del Proyecto

Este proyecto forma parte de la asignatura **Laboratorio de Programación: R y Python (2024-2)** en la Facultad de Ciencias Sociales. El objetivo principal fue trabajar con datos sociodemográficos correspondientes al departamento de **Lambayeque**, enfocándonos en los ingresos laborales de los individuos encuestados.

El equipo desarrolló un enfoque basado en técnicas de **Machine Learning** para predecir ingresos laborales. Utilizamos herramientas como Python y R para analizar, procesar los datos y entrenar modelos. Además, se siguieron buenas prácticas de programación y análisis.

## Contenidos del Proyecto

1. **Estructura del Trabajo**
   - Organización de carpetas siguiendo las pautas del curso.
   - Scripts configurados para ejecutarse con la opción `Run all`.

2. **Procesamiento de Información**
   - Exploración de datos: estadísticas descriptivas, identificación y tratamiento de valores faltantes.
   - Visualización de variables: histogramas, gráficos de densidad y boxplots.
   - Detección y manejo de outliers.
   - Análisis de correlaciones y relaciones entre variables clave.

3. **Modelado Predictivo**
   - División de datos en conjuntos de entrenamiento y prueba.
   - Entrenamiento de un modelo **Lasso** para selección de variables importantes.
   - Implementación de un modelo **Random Forest** con optimización de parámetros usando **GridSearch**.
   - Validación cruzada para evaluar la robustez del modelo.
   - Métricas de desempeño: **MAPE**, **R²**, y análisis de errores en el conjunto de prueba.

## Organización de Carpetas

La organización del proyecto es la siguiente:

```
PYTHON_TF_01/
├── data/                     # Contiene datos utilizados en el proyecto
│   ├── raw/                  # Datos originales sin procesar
│   ├── intermed/             # Datos intermedios procesados
│   └── final/                # Datos finales listos para modelado
├── docs/                     # Documentación adicional del proyecto
├── graphs/                   # Visualizaciones generadas durante el análisis
├── programs/                 # Scripts de Python y R
├── .RData                    # Archivo de configuración de R
├── .Rhistory                 # Historial de comandos de R
└── README.md                 # Descripción del proyecto
```

## Equipo de Trabajo

El equipo estuvo conformado por los siguientes integrantes:

- **Zarit de la Cruz** 
- **Angelly Gutierrez** 
- **Anderson Aguila** 
- **Jose Uriol** 
- **Carlo Llerena** 

## Docente

- **Mauricio Vallejos**  
  Correo: mauricio.vallejos@pucp.edu.pe

## Cómo Ejecutar

1. Clonar el repositorio:  
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   ```
2. Instalar dependencias:
   ```bash
   pip install -r requirements.txt
   ```
3. Ejecutar los scripts de la carpeta `programs/` en el orden documentado en `docs/`.

## Licencia

Este proyecto es de uso académico y está bajo licencia MIT.

---

Si necesitas más cambios o detalles adicionales, házmelo saber. 😊
