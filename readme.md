# Procesamiento de lenguaje natural


## Desafío 1: Vectorización de texto y Modelo Naïve Bayes

En este desafío, me enfrenté al desafío de clasificar documentos de texto pertenecientes al conjunto de datos "20 Newsgroups", el cual agrupa artículos de noticias en 20 categorías temáticas distintas. El objetivo principal fue construir un modelo capaz de identificar correctamente la categoría a la que pertenece un documento, basándose únicamente en su contenido textual. Para ello, implementé y evalué distintos enfoques de clasificación basados en el algoritmo Naïve Bayes, centrándome en dos variantes ampliamente utilizadas en tareas de procesamiento de lenguaje natural: Multinomial Naïve Bayes (MultinomialNB) y Complement Naïve Bayes (ComplementNB).
Ambos modelos fueron entrenados y validados con el propósito de optimizar el rendimiento medido a través del f1-score macro.

Link(esta en el repositorio también): https://colab.research.google.com/drive/1Y5HIfl4bYYJd-bzpm30e11SOt8e1DZRg 

## Desafío 2: Custom Embeddings con Gensim

Este desafío consistió en generar embeddings personalizados utilizando la biblioteca Gensim, tomando como base el texto completo de la Biblia. Para ello, se comenzó con un proceso de preprocesamiento del contenido, que incluyó tareas como la tokenización y la organización adecuada del corpus, dejándolo listo para el entrenamiento del modelo. A continuación, se utilizó Word2Vec para entrenar un modelo que permitiera obtener representaciones vectoriales de las palabras, con el objetivo de capturar las relaciones semánticas que existen entre ellas.
Una vez entrenado el modelo, se pusieron a prueba sus capacidades mediante evaluaciones de analogías entre palabras y se examinaron las similitudes semánticas a través de visualizaciones gráficas, lo cual facilitó un análisis más profundo de cómo las palabras se agrupan y se relacionan dentro del espacio vectorial generado.

Link(esta en el repositorio también): https://colab.research.google.com/drive/12Bm8a5bS1INVydwGYI-sZIpgjbnRd4Vv

## Desafío 3: Modelo de Lenguaje con Tokenización por caracteres

Este desafío tuvo como objetivo construir un modelo de lenguaje que pudiera predecir texto de manera coherente, utilizando como base el primer libro de La vuelta al mundo en 80 días. Para comenzar, se realizó un proceso de preparación del texto que incluyó la tokenización y la creación de secuencias adecuadas para entrenar el modelo. A partir de esto, se probaron distintas arquitecturas de redes neuronales recurrentes —como SimpleRNN, LSTM y GRU— con el fin de identificar cuál ofrecía mejores resultados en la generación de texto.
Durante la fase de inferencia, se implementaron métodos como greedy search y beam search para generar nuevas secuencias a partir del modelo entrenado. Finalmente, se compararon los distintos enfoques utilizando métricas como la perplejidad, lo que permitió evaluar la fluidez y precisión de las predicciones generadas por cada arquitectura.

Link(esta en el repositorio también): [https://colab.research.google.com/drive/1nHBq8mUi3BajvJFmnImoj0y9-cCSg8uD](https://colab.research.google.com/drive/1nHBq8mUi3BajvJFmnImoj0y9-cCSg8uD#scrollTo=pWCfxxDXjFod)

## Desafio 4: LSTM Bot QA

Este desafio tuvo como objetivo desarrollar un bot conversacional utilizando una arquitectura encoder-decoder basada en LSTM, diseñado para responder preguntas de forma coherente. El trabajo comenzó con el preprocesamiento del texto, que incluyó la tokenización y la construcción de diccionarios necesarios para convertir palabras en índices numéricos que el modelo pudiera interpretar. Para mejorar la calidad de las representaciones semánticas, se integraron embeddings preentrenados de FastText de 300 dimensiones, lo que permitió al modelo captar mejor el significado de las palabras en contexto.
Luego, se implementó una red neuronal del tipo encoder-decoder con capas LSTM, encargada de codificar la pregunta y generar una respuesta relevante. El sistema fue evaluado analizando las respuestas producidas frente a entradas reales del conjunto de datos, con el fin de validar su coherencia y pertinencia. Además, se experimentó con un enfoque alternativo utilizando un chatbot basado en modelos disponibles en Hugging Face, para comparar resultados y enfoques.

Link(esta en el repositorio también): https://colab.research.google.com/drive/1nHBq8mUi3BajvJFmnImoj0y9-cCSg8uD#scrollTo=pWCfxxDXjFod
