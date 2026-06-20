# 🎬 Proyecto Películas (Sprint 03-04) — Desarrollo End-to-End Individual

Este repositorio contiene la **solución completa e independiente** del proyecto de películas del Bootcamp de AI Engineering, desarrollada íntegramente por mí en el cuaderno `AlejandraSolucionIndividual.ipynb`. 

A diferencia del flujo de trabajo en equipo (diseñado para la integración modular de componentes), este espacio representa mi desarrollo autónomo de la arquitectura completa del sistema, abarcando desde la ingesta de datos crudos hasta la puesta en marcha del pipeline de IA.

---

## 🚀 Arquitectura y Fases del Proyecto Completo

El desarrollo se divide en 5 grandes bloques interconectados dentro del cuaderno individual:

### 1. Ingesta y Extracción de Datos (TMDB API)
* Configuración de la conexión con la API de *The Movie Database* (TMDB).
* Construcción de peticiones paginadas y manejo de *rate-limiting* (límites de velocidad).
* Extracción y estructuración inicial de metadatos de películas en formato JSON y posterior conversión a DataFrames.

### 2. Análisis Exploratorio de Datos (EDA) y Limpieza
* Identificación y tratamiento de valores nulos, registros duplicados y tipos de datos inconsistentes.
* Análisis estadístico descriptivo de variables numéricas y categóricas (presupuestos, ingresos, géneros, puntuaciones).
* Visualización de distribuciones y correlaciones iniciales para entender el comportamiento de los datos.

### 3. Ingeniería de Variables y Transformación
* Preprocesamiento de texto y normalización de variables categóricas (ej. extracción de géneros y palabras clave).
* Escalado de variables numéricas y codificación (*encoding*) para preparar los datos de entrada al modelo.
* Creación de nuevas características estructuradas que maximicen el rendimiento del algoritmo.

### 4. Modelado y Entrenamiento de IA
* División del conjunto de datos en entrenamiento, validación y prueba (*train/test split*).
* Selección, configuración y entrenamiento del algoritmo principal del Sprint.
* Optimización de hiperparámetros para mejorar la capacidad de generalización del modelo.

### 5. Evaluación y Conclusiones del Negocio
* Evaluación del rendimiento utilizando métricas clave del sector (ajustadas al tipo de problema: regresión o clasificación).
* Análisis de errores para identificar sesgos o debilidades del modelo entrenado.
* Conclusiones técnicas e implicaciones prácticas de la solución de IA sobre el catálogo de películas.

---

## 🛠️ Tecnologías y Herramientas Utilizadas
* **Lenguaje:** Python 3.x
* **Entorno:** Jupyter Notebooks (`.ipynb`)
* **Librerías Clave:** Pandas, NumPy, Requests (API), Scikit-Learn, Matplotlib / Seaborn.
* **Control de Versiones:** Git & GitHub (Rama aislada `lab-ale` para desarrollo independiente).

---

## 📋 Control de Cambios Local (Protocolo)

Para mantener este desarrollo íntegro y sin interferir con las entregas del equipo en la rama `develop`, utilizo el siguiente flujo estricto de comandos:

```bash
# Asegurar que estoy en mi entorno individual antes de codificar
git checkout lab-ale

# Registrar el progreso de todo el pipeline
git add AlejandraSolucionIndividual.ipynb README.md
git commit -m "feat: implementar [Indicar la fase completada]"
git push origin lab-ale