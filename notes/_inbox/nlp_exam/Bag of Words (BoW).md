---
aliases: 
publish: true
anki: false
created: 2025-02-08 16:20
parent:
  - "[[Text Feature Representation]]"
connected:
  - "#обс/linking"
tags:
  - empty
  - группа
---

> [!tip] The Bag of Words (BoW) 
is a [[Text Feature Representation]] in NLP that converts text into numerical vectors based on word frequencies, ignoring word order and grammar. 
This enables machine learning models to process text data for tasks like classification and clustering.


### How BoW Works

#### 1. Vocabulary Creation
- Build a vocabulary containing all unique words from the corpus (collection of documents)
- Assign a unique index to each word in the vocabulary

#### 2. Document Vectorization
- Convert each document into a fixed-length vector:
  - Length equals vocabulary size
  - Each position represents a word from vocabulary
  - Values show how many times each word appears

#### 3. Document-Term Matrix (DTM)
The final result is a matrix where:
- Each row represents a document
- Each column represents a word from vocabulary 
- Values show word frequencies in documents

For example, given documents:
1. "The cat sat on the mat"
2. "The dog ran on the grass"
3. "A cat and dog play"

After preprocessing and removing stopwords, the DTM would look like:

$$
\begin{bmatrix} 
\text{cat} & \text{sat} & \text{mat} & \text{dog} & \text{ran} & \text{grass} & \text{play} \\
\hline
1 & 1 & 1 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 & 1 & 1 & 0 \\
1 & 0 & 0 & 1 & 0 & 0 & 1
\end{bmatrix}
$$

Each row represents one document, and the numbers show how many times each word appears in that document.

#### 4. Key Properties
- Word order is ignored
- Only word frequencies matter
- Grammar and syntax are not preserved
- Semantic relationships between words are not captured

### Example of BoW

#### Given Corpus:

5. "I love NLP."
    
6. "NLP is fun and exciting."
    

#### Step-by-Step BoW Representation:

7. Preprocessing:
    

- Lowercased: "i love nlp", "nlp is fun and exciting".
    
- Remove stopwords (optional): "love nlp", "nlp fun exciting".
    

8. Vocabulary Construction:
    

- Vocabulary: { "love", "nlp", "fun", "exciting" }
    
- Indices: { 0: "love", 1: "nlp", 2: "fun", 3: "exciting" }
    

9. Vectorization:
    

- Document 1: [1, 1, 0, 0] ("love" and "nlp" each occur once).
    
- Document 2: [0, 1, 1, 1] ("nlp", "fun", and "exciting" each occur once).
    

  

| Document | love | nlp | fun | exciting |

|----------|------|-----|-----|----------|

| Doc1     |  1   |  1  |  0  |    0     |

| Doc2     |  0   |  1  |  1  |    1     |

  
  

### Strengths of BoW

10. Simplicity:
    

- Easy to implement and interpret.
    
- Works well for a wide range of NLP tasks.
    

11. Independence:
    

- No assumptions about the structure or grammar of the language.
    

12. Versatility:
    

- Can be applied to any textual data.
    

### Limitations of BoW

13. Loss of Context:
    

- Ignores word order and syntax, leading to a loss of semantic meaning.
    

14. Dimensionality:
    

- Vocabulary size increases with the corpus size, leading to a sparse and high-dimensional matrix.
    

15. Feature Redundancy:
    

- Synonyms and related words are treated as independent features.
    

16. Scalability:
    

- Computational inefficiency with very large vocabularies or corpora.
    



**
