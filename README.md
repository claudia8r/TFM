# Detección de Alimentos mediante modelos de visión por computadora

Este proyecto corresponde al Trabajo de Fin de Máster (TFM) y tiene como objetivo el desarrollo de un sistema capaz de detectar alimentos en imágenes mediante visión por computador y, a partir de los resultados obtenidos, recomendar recetas utilizando modelos de lenguaje locales (LLM).

El proyecto se estructura en dos archivos Jupyter Notebook (.ipynb). La estructura del Proyecto es la siguiente:

├── README.md

├── comparadorLLM.ipynb

└── modelo_final.ipynb

## 1. modelo_final.ipynb

Este notebook contiene el sistema final desarrollado, integrando todas las fases del proyecto. En él se pueden encontrar los siguientes apartados:

### Análisis y preparación del dataset

-Exploración inicial del conjunto de datos.
-Análisis de clases y distribución de alimentos.

### Entrenamiento del modelo de detección

- Entrenamiento del modelo de detección de objetos utilizando YOLOv8.
- Evaluación del rendimiento del modelo.

### Visualización de métricas

- Precisión (Precision)
- Recall
- mAP
- Matriz de confusión

### Predicciones sobre imágenes externas

- Rendimiento del modelo sobre imágenes no pertenecientes al dataset.
- Visualización de resultados de detección de alimentos.

### Integración con modelos de lenguaje (LLM)

- Creación de dos listas a partir de los alimentos detectados:
- Llamada a una API local de Ollama.
- Uso del modelo LLaMA 3.1 para recomendar una receta y organizar la lista de ingredientes.
  

## 2. comparativa_llm.ipynb

Este notebook está dedicado a la comparación de distintos modelos de lenguaje locales (LLM) con el fin de seleccionar el más adecuado para el sistema final.

En él se realiza:

- Evaluación de diferentes modelos ejecutados localmente mediante Ollama.
- Comparación de aspectos como: Claridad, coherencia y creatividad.


## Tecnologías Utilizadas

- Python
- Jupyter Notebook
- YOLOv8 (detección de objetos)
- Ultralytics
- Roboflow
- Ollama
- LLaMA 3.1
