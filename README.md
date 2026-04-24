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

### 3. [Desafío 3: Modelo de lenguaje con tokenización por caracteres](Desafio_3.ipynb)
Desarrollo de modelos de lenguaje basados en caracteres utilizando Redes Neuronales Recurrentes, entrenados sobre la obra literaria "La vuelta al mundo en 80 días" de Julio Verne.
* **Técnicas implementadas:**
  * Preprocesamiento y tokenización a nivel de caracteres de un corpus literario.
  * Estructuración del *dataset* para el modelado de secuencias bajo la arquitectura *Many-to-Many*.
  * Entrenamiento y evaluación comparativa de arquitecturas neuronales recurrentes (`SimpleRNN`, `GRU` y `LSTM`) utilizando `TensorFlow/Keras`.
  * Desarrollo de un *callback* personalizado para el cálculo de la métrica de Perplejidad (*Perplexity*) y detención temprana (*Early Stopping*).
  * Inferencia y generación de texto utilizando diferentes algoritmos de decodificación: *Greedy Search* y *Beam Search* (determinista y estocástico, analizando el impacto del hiperparámetro de temperatura).
 
### 4. [Desafío 4: Bot QA con Arquitectura Seq2Seq (Encoder-Decoder)](Desafio_4_SP.ipynb)
Desarrollo de un agente conversacional (Bot QA) utilizando una arquitectura profunda de secuencias *Encoder-Decoder* con celdas LSTM, entrenado sobre el *dataset* ConvAI2.
* **Técnicas implementadas:**
  * Preprocesamiento de texto conversacional (limpieza de contracciones, *tokens* de inicio/fin `<sos>`/`<eos>` y estrategias de *padding* asimétrico `pre`/`post`).
  * Integración de *Word Embeddings* pre-entrenados (GloVe) con manejo de vocabulario fuera del corpus (OOV).
  * Entrenamiento de modelo Seq2Seq utilizando la API funcional de `TensorFlow/Keras` con transferencia de estados latentes.
  * Extracción de modelos de inferencia independientes (*Encoder* y *Decoder*) para procesamiento paso a paso.
  * Implementación y comparación de múltiples estrategias de decodificación avanzadas: *Greedy Search*, *Beam Search* (con penalización de repetición) y *Temperature Sampling*.
  * Experimentación con memoria de contexto multi-turno mediante el promedio de estados latentes y análisis teórico sobre el colapso de respuestas y la necesidad de mecanismos de atención (*Cross-Attention* / *Transformers*).

---

## 🚀 Entorno de Ejecución

Los notebooks fueron desarrollados para ser ejecutados en **Google Colab**. Para reproducir los resultados:
1. Abrir los archivos `.ipynb` en Colab.
2. Ejecutar la primera celda para instalar las dependencias necesarias (`numpy`, `scikit-learn`, `gensim`, `plotly`, `tensorflow`).

---

## 👩‍💻 Autora
* **Pryszczuk, Sabrina Daiana** - Alumna de la cohorte 22Co2025 - CEIA FIUBA.
