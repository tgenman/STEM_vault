---
aliases: 
publish: true
anki: false
created: 2025-02-09 22:37
parent: 
connected:
  - "#обс/linking"
tags:
  - empty
  - группа
---
[[Word Embeddings]]. [[Word2Vec]]: CBOW, skip-gram, negative sampling. Word2vec properties.

**

Word embeddings are dense vector representations of words in a continuous vector space. Unlike traditional techniques like Bag of Words (BoW) or TF-IDF, word embeddings capture the semantic meaning of words and their relationships by learning from large text corpora. Words with similar meanings or contexts are mapped to nearby points in the vector space.

Word2Vec is one of the most influential techniques for generating word embeddings. It was introduced by Tomas Mikolov et al. at Google in 2013 and offers two main models: Continuous Bag of Words (CBOW) and Skip-Gram.

  

### Word2Vec Models

2. Continuous Bag of Words (CBOW):
    

- Objective: Predict a target word given its context words.
    
- Input: The context words (surrounding words of a target word in a fixed window size).
    
- Output: The target word.
    
- Architecture:
    

- Uses a feedforward neural network.
    
- Context words are mapped to embeddings, averaged, and passed through a softmax layer to predict the target word.
    

- Example:
    

- Sentence: "The cat sat on the mat."
    
- Target: "sat"
    
- Context: ["the", "cat", "on", "the"]
    

- Characteristic: It is computationally efficient because it averages context word embeddings.
    

3. Skip-Gram:
    

- Objective: Predict the context words given a target word.
    
- Input: The target word.
    
- Output: Context words.
    
- Architecture:
    

- Learns to maximize the probability of surrounding words within a defined window size for a given target word.
    

- Example:
    

- Sentence: "The cat sat on the mat."
    
- Target: "sat"
    
- Context: ["the", "cat", "on", "the"]
    

- Characteristic: Works well for rare words and can capture complex relationships.
    

### Negative Sampling

- Purpose: Improve computational efficiency by approximating the softmax function used in Word2Vec.
    
- Challenge in Softmax:
    

4. In large vocabularies, computing the full softmax probability is computationally expensive because it requires normalization over all words.
    

- Solution:
    

5. Use a small number of "negative samples" (words not related to the target word in context) to approximate the output.
    

- Process:
    

6. Select negative samples (random words) from the vocabulary.
    
7. Train the model to distinguish between true context words and negative samples.
    

- Benefit: Reduces computational cost from O(∣V∣)(vocabulary size) to O(K), where K is the number of negative samples.
    

### Properties of Word2Vec Embeddings

8. Semantic and Syntactic Relationships:
    

- Word2Vec captures both semantic (e.g., "king" is similar to "queen") and syntactic (e.g., verb tense) relationships.
    
- Famous Example: Vector arithmetic king−man+woman≈queen
    

9. Continuous Vector Space:
    

- Embeddings are dense (low-dimensional) compared to BoW or TF-IDF.
    

10. Contextual Similarity:
    

- Words occurring in similar contexts have closer embeddings (e.g., "doctor" and "nurse").
    

11. Unsupervised Learning:
    

- Word2Vec learns embeddings directly from raw text without labeled data.
    

12. Dimensionality Reduction:
    

- Words are typically embedded in a space of 100–300 dimensions, much smaller than the original vocabulary size.
    

### Key Advantages of Word2Vec

13. Efficient Representation:
    

- Embeddings are compact and capture meaningful patterns compared to sparse vectors in BoW or TF-IDF.
    

14. Captures Word Similarity:
    

- Similar words are close in the vector space, enabling semantic understanding.
    

15. Scalability:
    

- Handles large corpora efficiently, especially with negative sampling.
    

16. Pretrained Models:
    

- Pretrained Word2Vec embeddings (e.g., Google News embeddings) can be used for downstream tasks.
    

### Limitations of Word2Vec

17. Context Independence:
    

- Word2Vec embeddings are static, meaning the same word has the same vector representation regardless of context. For example, "bank" in "river bank" and "financial bank" will have the same embedding.
    

18. Training Data Dependency:
    

- The quality of embeddings depends heavily on the quality and size of the training corpus.
    

19. Rare Words:
    

- Performs poorly on rare words not well represented in the training data.
    

20. Dimensionality Choice:
    

- Selecting the right number of dimensions for embeddings requires experimentation.
    

### Applications of Word2Vec

21. Text Classification:
    

- Sentiment analysis, spam detection, etc.
    

22. Clustering:
    

- Group similar words or documents using embeddings.
    

23. Machine Translation:
    

- Used for representing words in translation models.
    

24. Information Retrieval:
    

- Rank documents or search results based on semantic similarity.
    

25. Recommendation Systems:
    

- Embedding-based similarity can recommend items or content.
    

### Summary

- Word2Vec is a milestone in NLP for learning dense, meaningful representations of words.
    
- It has two main models:
    

- CBOW: Predicts target words from context, computationally efficient.
    
- Skip-Gram: Predicts context words from target words, effective for rare words.
    

- Negative Sampling accelerates training by approximating the softmax function.
    

Word2Vec embeddings are foundational in many NLP applications and have inspired advanced techniques like GloVe and transformer-based models (e.g., BERT).**