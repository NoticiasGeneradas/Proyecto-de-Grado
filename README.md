# Generador de Noticias Deportivas con Redes Neuronales Recurrentes (RNN)

Este repositorio contiene el código y la documentación para un modelo de generación automática de noticias deportivas utilizando Redes Neuronales Recurrentes (RNN) con Long Short-Term Memory (LSTM). El modelo combina datos textuales, históricos y simulados para producir narrativas coherentes, relevantes y personalizadas, especialmente enfocado en eventos del fútbol español.

---

## **Características Principales**

- **Entrenamiento Híbrido:** Integra datos históricos reales y simulados para enriquecer la narrativa generada.
- **Modelo Avanzado:** Arquitectura de RNN con capas de embedding, LSTM y densas, diseñada para capturar dependencias temporales y contextualizar las predicciones.
- **Personalización:** Genera contenido adaptado a estadísticas específicas de equipos y eventos.
- **Resultados Simulados:** Explora escenarios hipotéticos, incluyendo análisis predictivos de desempeño.

---

## **Estructura del Proyecto**

📂 Generador-De-Noticias-Deportivas ├── 📁 data │ ├── historical_data.csv # Datos históricos y simulados │ ├── text_data.csv # Noticias deportivas originales ├── 📁 src │ ├── preprocessing.py # Preprocesamiento de datos textuales │ ├── model.py # Definición de la arquitectura RNN │ ├── train.py # Entrenamiento del modelo │ ├── generate.py # Generación de noticias deportivas ├── 📁 notebooks │ ├── Exploratory_Data_Analysis.ipynb # Análisis exploratorio de datos │ ├── Model_Training.ipynb # Entrenamiento y evaluación del modelo ├── 📁 outputs │ ├── generated_news_examples.txt # Ejemplos de noticias generadas ├── README.md # Documentación del proyecto └── requirements.txt # Dependencias necesarias




---
## Cómo Usar el Proyecto
1. Preprocesar los Datos
Ejecuta el script de preprocesamiento para limpiar y tokenizar los datos textuales:

--python src/preprocessing.py

2. Entrenar el Modelo
Entrena el modelo utilizando el script train.py. Puedes ajustar los hiperparámetros en el archivo de configuración:

--python src/train.py

3. Generar Noticias
Una vez entrenado el modelo, genera noticias deportivas personalizadas:
python src/generate.py --seed "El equipo logró una victoria"



## Evaluación del Modelo
## Métricas Utilizadas:

-Coherencia narrativa: Evaluada por pares con un puntaje promedio de 8.5/10.
-BLEU Score: Utilizado para comparar las noticias generadas con textos reales.
-Relevancia: Incorporación efectiva de datos históricos y simulados en las predicciones.
-Resultados Clave:

## Generación de texto con un 85% de precisión narrativa.
-Integración exitosa de datos históricos, como posiciones en liga y capacidades de estadios.
## Tecnologías Utilizadas
-Python: Para el preprocesamiento, entrenamiento y generación.
-TensorFlow/Keras: Implementación de la arquitectura RNN (LSTM).
-Pandas: Manejo y análisis de datos históricos.
-NumPy: Operaciones matemáticas y manipulación de matrices.






