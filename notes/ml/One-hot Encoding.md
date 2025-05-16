---
aliases: 
anki: false
created: 2025-01-19 23:47
parent:
  - "[[Categorical Feature Representation]]"
connected:
  - "#обс/linking"
tags:
  - empty
---


# Anki
TARGET DECK: stem::ml::core
START
math_complex
TITLE: One-hot Encoding  
DESCRIPTION: A method for representing categorical data as a binary vector where only one element is 1, and the rest are 0. It is used to encode categorical variables into a numerical format understandable by machine learning algorithms.  
FORMULA: A vector of length NNN, where NNN is the number of categories. Example: "Cat" = $[1,0,0]$, "Dog" = $[0,1,0]$, "Bird" = $[0,0,1]$.  
ADDITIONAL: Used in classification and categorization tasks. Limitation: high dimensionality with many categories. Alternatives: embedding, target encoding.    
PICTURE:
ID: 1737306432496
END