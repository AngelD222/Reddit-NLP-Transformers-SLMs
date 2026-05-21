# Reddit-NLP-Transformers-SLMs

# End-to-End NLP Pipeline: Text Classification, Summarization & Generative AI

Este repositorio contiene un sistema completo de Procesamiento de Lenguaje Natural (NLP) aplicado a un dataset multitemático extraído de Reddit. El proyecto abarca desde la evaluación de algoritmos clásicos de *Machine Learning* hasta la implementación de técnicas en IA generativa, demostrando la capacidad de diseñar, evaluar y optimizar arquitecturas lingüísticas complejas.

## 📊 Dataset
El corpus de datos fue extraído mediante la **API de Reddit** y curado para abarcar 10 dominios de conocimiento diversos (incluyendo Medicina, Política y Tecnología). Esto permite evaluar la robustez de los modelos ante diferentes jergas y estructuras semánticas.

* **Lenguaje:** Python
* **Frameworks de Deep Learning:** PyTorch, TensorFlow / Keras
* **Ecosistema NLP:** Hugging Face (Transformers, PEFT, Datasets), NLTK, Spacy
* **Modelos Base:** BETO, RoBERTa, mT5, Gemma, Llama
* **Machine Learning Clásico:** Scikit-learn (TF-IDF, SVM)

## ⚙️ Arquitectura del Pipeline

El flujo de trabajo se divide en cuatro fases técnicas principales:

### 1. Clasificación de Texto y Benchmarking
Se estableció una base sólida de rendimiento comparando métodos tradicionales con arquitecturas de aprendizaje profundo:
* **Línea Base:** Vectorización TF-IDF acoplada a un clasificador SVM.
* **Fine-tuning de Transformers:** Ajuste fino de modelos bidireccionales de lenguaje enmascarado (BETO y RoBERTa) para la clasificación precisa de los 10 dominios temáticos.

### 2. Resumen Abstractivo y Análisis de Sentimiento
* Implementación del modelo secuencial **mT5** para la generación de resúmenes abstractivos de hilos de conversación complejos.
* Evaluación cuantitativa del rendimiento de la síntesis de texto utilizando métricas **ROUGE**.
* Extracción de polaridad y análisis de sentimiento integrado en el flujo de análisis.

### 3. Ingeniería de Prompts (Prompt Engineering)
Exploración sistemática del comportamiento de Modelos de Lenguaje Grandes (LLMs) mediante el diseño de instrucciones estructuradas:
* Estrategias de *Zero-shot* y *Few-shot prompting*.
* Aplicación de *Chain-of-Thought (CoT)* para forzar el razonamiento explícito en tareas lógicas.

### 4. Parameter-Efficient Fine-Tuning (PEFT)
Optimización de Modelos de Lenguaje Pequeños (SLMs) como **Gemma** y **Llama** para tareas específicas de *Question Answering* dentro de los dominios del dataset. Se aplicaron técnicas de cuantización y ajuste de bajo rango (**LoRA / QLoRA**) para maximizar el rendimiento reduciendo drásticamente el coste computacional y de memoria.


