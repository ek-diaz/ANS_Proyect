# ANS_Proyect
# 🏥 Análisis de Comentarios de Pacientes en una Clínica de Maryland 🩺

¡Bienvenido al proyecto de análisis de comentarios de pacientes en **CCI Health Services**!, una clínica comunitaria ubicada en Maryland 🌎 Este proyecto utiliza técnicas avanzadas de aprendizaje no supervisado para mejorar la interpretación de las encuestas de satisfacción y, en última instancia, elevar la calidad de la atención al paciente. 💖

## 🧠 Objetivo del Proyecto

El objetivo principal es mejorar la evaluación de las encuestas de satisfacción que se envían a los pacientes después de cada visita, identificando temas recurrentes y sentimientos expresados en los comentarios. Este enfoque permitirá que la clínica tome decisiones más informadas para mejorar la experiencia de sus pacientes.

## 🚀 Introducción

En el sector de la salud, entender las necesidades y preocupaciones de los pacientes es crucial. Actualmente, la revisión de las respuestas abiertas en las encuestas de satisfacción se realiza de manera manual, lo que es ineficiente y lento. Este proyecto propone un cambio, utilizando herramientas de procesamiento del lenguaje natural (NLP) y técnicas de aprendizaje no supervisado como el clustering para analizar estos comentarios de manera más efectiva.

<div style="width:100%;height:0;padding-bottom:100%;position:relative;"><iframe src="https://giphy.com/embed/setIIIZYAz7qoWX0D3/video" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div><p><a href="https://giphy.com/clips/pandemic-setIIIZYAz7qoWX0D3">via GIPHY</a></p>

## 📊 Descripción de los Datos

La base de datos utilizada en este proyecto contiene más de 24,000 observaciones y recoge información de encuestas realizadas entre 2019 y 2024. Los datos incluyen tanto respuestas estructuradas como comentarios abiertos en inglés y español. 🔄

| Variable       | Descripción                                  |
|----------------|----------------------------------------------|
| Respondent ID  | Identificador único del encuestado           |
| End Date       | Fecha de finalización de la encuesta         |
| Language       | Idioma de la encuesta (inglés o español)     |
| Comments       | Comentarios abiertos proporcionados por el paciente |

## 🔍 Metodología

### 1. Preprocesamiento de Datos
Antes de aplicar cualquier modelo, es fundamental limpiar y preparar los datos. Algunas de las tareas incluyen:

- Conversión de texto a minúsculas
- Eliminación de signos de puntuación y caracteres especiales
- Remoción de *stopwords*
- Lematización para reducir palabras a su forma base

### 2. Vectorización
Se utiliza el vectorizador TF-IDF para convertir el texto preprocesado en representaciones numéricas, permitiendo así su procesamiento por algoritmos de aprendizaje automático.

### 3. Reducción de Dimensionalidad
- **Análisis de Componentes Principales (PCA)**: Para identificar patrones y reducir la complejidad.
- **Descomposición en Valores Singulares (SVD)**: Para manejar matrices esparsas y obtener componentes clave.

### 4. Clustering
Aplicamos diferentes algoritmos para agrupar los comentarios:

- **K-Means**: Para particionar los datos en clusters iniciales.
- **K-Medoids**: Verifica la estabilidad de los clusters obtenidos con K-Means.
- **Clustering Jerárquico**: Permite visualizar relaciones jerárquicas entre los comentarios.
- **DBSCAN**: Detecta patrones en los datos que otros métodos podrían pasar por alto.

## 📚 Tecnologías Utilizadas

- **Lenguajes de Programación:** Python
- **Frameworks y Bibliotecas:** Scikit-learn, NLTK, Pandas, Matplotlib, Seaborn
- **Herramientas:** Jupyter Notebook, Google Colab

## 🔧 Requisitos Previos

- **Python 3.x**
- **Jupyter Notebook o Google Colab**
- Instalación de bibliotecas: `scikit-learn`, `nltk`, `pandas`, `matplotlib`, `seaborn`

