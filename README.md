# Especialización en Inteligencia Artificial (CEIA - FIUBA)
## Procesamiento del Lenguaje Natural I

Este repositorio contiene los trabajos prácticos y desafíos correspondientes a la materia **Procesamiento del Lenguaje Natural I** dictada en el Laboratorio de Sistemas Embebidos de la Facultad de Ingeniería de la Universidad de Buenos Aires (FIUBA).

---

## 📚 Contenido del Repositorio

### 1. [Desafío 1: Vectorización de Texto y Clasificación Bayesiana](Desafio_1.ipynb)
Implementación de técnicas estadísticas clásicas de NLP para la agrupación y clasificación de documentos utilizando el dataset *20 Newsgroups*.
* **Técnicas implementadas:**
  * Vectorización de documentos mediante `CountVectorizer` y `TfidfVectorizer`.
  * Optimización de hiperparámetros (`stop_words`, `min_df`, `max_df`) para reducción de ruido.
  * Análisis de similaridad coseno para recuperación de documentos y construcción de matrices término-documento (*Word Embeddings* estadísticos primitivos).
  * Entrenamiento y comparación de modelos predictivos (`MultinomialNB` y `ComplementNB`).

### 2. [Desafío 2: *Custom Word Embeddings* con Gensim](Desafio_2.ipynb)
Desarrollo y entrenamiento desde cero de *Word Embeddings* personalizados, utilizando como corpus de entrenamiento las letras de las canciones de **Adele**.
* **Técnicas implementadas:**
  * Preprocesamiento y tokenización de corpus de texto sin diccionarios previos.
  * Entrenamiento de modelo de redes neuronales Word2Vec (arquitectura Skip-gram) utilizando la librería `Gensim`.
  * Implementación de *callbacks* personalizados para el resguardo dinámico del mejor modelo en memoria.
  * Análisis de similaridad semántica y sintáctica latente.
  * Reducción de dimensionalidad y visualización interactiva del espacio vectorial en 2D utilizando `t-SNE` y `Plotly`.

---

## 🚀 Entorno de Ejecución

Los notebooks fueron desarrollados para ser ejecutados en **Google Colab**. Para reproducir los resultados:
1. Abrir los archivos `.ipynb` en Colab.
2. Ejecutar la primera celda para instalar las dependencias necesarias (`numpy`, `scikit-learn`, `gensim`, `plotly`, `tensorflow`).

---

## 👩‍💻 Autora
* **Pryszczuk, Sabrina Daiana** - Alumna de la cohorte 22Co2025 - CEIA FIUBA.
