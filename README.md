# TP_NLP1
Trabajos Practicos de NLP_1 

Estructura del Proyecto
Desafío 1 — Preprocesamiento inicial
Carga de datos conversacionales del dataset ConvAI2.
Limpieza y normalización de texto:
Conversión a minúsculas
Eliminación de caracteres especiales
Expansión de contracciones
Generación de pares de preguntas-respuestas (input_sentences, output_sentences, output_sentences_inputs).
Ajuste de longitudes máximas de secuencias para optimizar el modelo.

Objetivo: preparar los datos de entrenamiento para las siguientes etapas de modelado.

Desafío 2 — Generación de embeddings custom con Gensim
Entrenamiento de modelos de embeddings propios:
Word2Vec
FastText (alternativo)
Creación de embeddings directamente a partir del corpus del dataset procesado.
Obtención de embedding_matrix personalizada en base al vocabulario generado.

Objetivo: entrenar embeddings adaptados al dominio conversacional específico, mejorando la representación semántica.

Desafío 3 — Entrenamiento del modelo secuencial básico
Construcción de un modelo secuencial encoder-decoder utilizando embeddings generados.
Arquitectura basada en LSTM:
Encoder con embeddings fijos
Decoder con embeddings fijos o entrenables
Preparación de los datos con padding y codificación one-hot.
Entrenamiento inicial del modelo seq2seq.

Objetivo: implementar el primer modelo funcional de pregunta-respuesta.

Desafío 4 — Desarrollo final del chatbot QA
Optimización de la arquitectura completa:
Unificación de tokenizadores (vocabulario único)
Embedding único, fijo, compartido por encoder y decoder
Inclusión de mask_zero=True para mejorar el tratamiento de padding.
Separación de modelos de inferencia (encoder_model y decoder_model) para uso práctico.
Implementación completa de la lógica de inferencia:
Entrada de texto libre
Traducción a tokens
Generación de respuesta automática.
Evaluación final del modelo.

Objetivo: versión finalizada y optimizada del chatbot seq2seq para tareas de respuesta automática.

Dependencias principales
TensorFlow / Keras
Gensim
NumPy / Pandas
scikit-learn
Matplotlib / Seaborn (visualización)
