---
aliases: 
publish: true
anki: false
created: 2025-01-19 23:46
parent:
  - "[[Categorical Feature Representation]]"
connected: 
tags:
  - empty
---

  - Dense vector representation of categories.
  - Captures relationships and similarities between categories.

#### Anki
> [!question]- Embedding
TARGET DECK: ML::Core
START
Math_ONE_side
TITLE: Embedding  
DESCRIPTION: A method for representing objects as dense vectors in a lower-dimensional space, where their similarity or semantic relationships are reflected by the proximity of their vectors. It is used to convert complex data into numerical formats.  
FORMULA: A vector of dimension ddd, where ddd is smaller than the number of categories. Example: "king" → $[0.25,−0.64,0.13]$, "queen" → $[0.26,−0.63,0.14]$.  
ADDITIONAL: Applied in NLP (e.g., [[Word2Vec]], [[GloVe]]), recommendation systems, and computer vision. Advantage: compactness and ability to model relationships between objects. Limitation: requires large datasets for training.   
ID: 1737306548883
END
