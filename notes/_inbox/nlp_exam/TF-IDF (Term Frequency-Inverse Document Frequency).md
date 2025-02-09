---
aliases:
  - TF-IDF
publish: true
anki: false
created: 2025-02-09 19:25
parent: 
connected:
  - "#обс/linking"
tags:
  - empty
  - группа
---
**

TF-IDF is a statistical measure used in Natural Language Processing (NLP) to evaluate the importance of a word in a document relative to a collection of documents (corpus). Unlike the simple Bag of Words (BoW) model, TF-IDF assigns weights to words based on their frequency in a single document and across all documents in the corpus, emphasizing rare but significant terms.

TF-IDF is a combination of two metrics:

1. Term Frequency (TF):
    

- Measures how often a term appears in a document.
    
- Formula:
$${ TF(t, d) = \frac{f(t, d)}{\sum_k f(k, d)} }$$  

- $f(t, d)$: Frequency of term $t$ in document $d$.  
- $\sum_k f(k, d)$: Total number of terms in document $d$.  

    

2. Inverse Document Frequency (IDF):
    

- Measures the rarity of a term across the corpus.
    
- Formula:
$${ IDF(t, D) = \log\left(\frac{N}{1 + | \{ d \in D : t \in d \} |}\right) }$$  

- $N$: Total number of documents in the corpus $D$.  
- $\left| \{ d \in D : t \in d \} \right|$: Number of documents containing term $t$.  
- Adding 1 in the denominator avoids division by zero.  



3. TF-IDF:
    

- Combines TF and IDF to calculate the weight of a term in a document.
    
- Formula: 
$${ TF\text{-}IDF(t, d, D) = TF(t, d) \times IDF(t, D) }$$

### Key Properties of TF-IDF

4. High Weight:
    

- A term that occurs frequently in a document but rarely in the corpus receives a high weight.
    
- This highlights terms that are specific to a document.
    

5. Low Weight:
    

- Common terms across the corpus receive lower weights, even if they appear frequently in a document (e.g., stop words like "the" or "is").
    

### Applications of TF-IDF

6. Text Classification:
    

- Used as a feature representation in tasks like spam detection and sentiment analysis.
    

7. Information Retrieval:
    

- Search engines rank documents by the relevance of terms using TF-IDF.
    

8. Keyword Extraction:
    

- Identifies significant terms in documents for summarization.
    

9. Clustering and Topic Modeling:
    

- Represents documents as vectors for clustering algorithms.
    

### Strengths of TF-IDF

10. Simplicity:
    

- Easy to calculate and understand.
    
- Widely used in traditional NLP pipelines.
    

11. Efficiency:
    

- Captures the importance of words relative to their rarity.
    

12. Flexibility:
    

- Works well for small to medium-sized datasets.
    

### Limitations of TF-IDF

13. Lack of Context:
    

- Ignores the semantic meaning of words and their order.
    

14. Sparsity:
    

- For large vocabularies, the document-term matrix becomes sparse.
    

15. Scalability:
    

- Less efficient for very large datasets with millions of documents.
    

16. Vocabulary Dependence:
    

- Sensitive to pre-processing steps like tokenization, stop word removal, and stemming.
    

### Summary

- TF-IDF improves upon Bag of Words by weighting terms based on their significance in a document and rarity across the corpus.
    
- It is foundational in many text processing pipelines and remains a competitive choice for smaller datasets and traditional NLP tasks.
    

**