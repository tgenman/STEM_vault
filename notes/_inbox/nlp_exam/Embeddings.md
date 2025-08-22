---
aliases: 
anki: false
created: 2025-01-19 23:46
parent:
  - "[[Feature Representation]]"
connected: 
tags:
  - fix/empty
---
В каждом случае эмбеддинги создают компактное векторное представление сложных данных, сохраняя их важные характеристики и семантические свойства для дальнейшего использования в ML моделях.

- Эмбеддинги для текста:
    - [[Word Embeddings]] ([[Word2Vec]], GloVe, FastText)
        - CBOW (Continuous Bag of Words)
        - Skip-gram модели
        - Contextual word embeddings (из [[BERT]] BERT, ELMo)
    - Sentence embeddings (BERT, USE, SentenceBERT)
    - Document embeddings (Doc2Vec)
    - Character embeddings
    - Subword embeddings (используются в BERT, GPT)
- Эмбеддинги для изображений:
    - CNN embeddings (извлекаются из предобученных CNN)
    - CLIP embeddings (мультимодальные эмбеддинги текст-изображение)
    - Patch embeddings (используются в Vision Transformers)
    - Facial embeddings (для распознавания лиц)
- Графовые эмбеддинги:
    - Node embeddings (Node2Vec, DeepWalk)
    - Graph embeddings (Graph2Vec)
    - Knowledge graph embeddings (TransE, RotatE)
- Временные ряды и последовательности:
    - Time series embeddings
    - Sequence embeddings (для биологических последовательностей)
    - Trajectory embeddings (для данных о движении)
- Мультимодальные эмбеддинги:
    - Аудио-визуальные эмбеддинги
    - Текст-изображение эмбеддинги
    - Кросс-модальные эмбеддинги
- Специализированные эмбеддинги:
    - User embeddings (для рекомендательных систем)
    - Product embeddings (для e-commerce)
    - Geographic embeddings (для геоданных)
    - Molecular embeddings (для химических соединений)
- Категориальные эмбеддинги:
    - Entity embeddings (для категориальных переменных с большим количеством уникальных значений)
    - [[One-hot Encoding]] -> Dense embeddings (преобразование через слой Embedding)
    - Learned category embeddings (обучаемые эмбеддинги категорий)
    - Hierarchical category embeddings (для иерархических категориальных данных)


  - Dense vector representation of categories.
  - Captures relationships and similarities between categories.

# Anki
TARGET DECK: stem::ml::core
START
math_complex
FRONT: Embedding  
BACK: A method for representing objects as dense vectors in a lower-dimensional space, where their similarity or semantic relationships are reflected by the proximity of their vectors. It is used to convert complex data into numerical formats.  
FORMULA: A vector of dimension ddd, where ddd is smaller than the number of categories. Example: "king" → $[0.25,−0.64,0.13]$, "queen" → $[0.26,−0.63,0.14]$.  
ADDITIONAL: Applied in NLP (e.g., [[Word2Vec]], [[GloVe]]), recommendation systems, and computer vision. Advantage: compactness and ability to model relationships between objects. Limitation: requires large datasets for training.   
ID: 1737306548883
END
