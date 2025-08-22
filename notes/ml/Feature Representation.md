---
aliases: 
created: 2025-01-19 23:42
parent: "[[Machine Learning MOC|ML MOC]]"
connected: []
tags:
  - content/MOC
---

![[Categorical Feature Representation]] 



- **Numerical Feature Representation**
  - Methods for scaling and transforming numerical data:
    - **Normalization**: Scales data to a range of [0, 1].
    - **Standardization**: Scales data to have a mean of 0 and a standard deviation of 1.
    - **Log Transformation**: Reduces skewness in data distributions.
    - **Polynomial Features**: Generates new features by raising data to powers.
    - **Discretization**: Converts numerical data into categories (e.g., using quantiles).


![[Text Feature Representation]]


- **Time Series Representation** [[Time Series ML]]
  - Methods for analyzing sequential data over time:
    - **Lag Features**: Uses past values as features.
    - **Rolling Statistics**: Calculates moving averages, standard deviations, etc.
    - **Fourier Transform**: Analyzes frequency components of time-series data.
    - **Trend and Seasonality Features**: Extracts long-term trends and seasonal patterns.

- **Image Feature Representation** [[notes/ml/Computer Vision]]
  - Techniques for processing image data:
    - **Pixel Intensities**: Directly uses pixel values as features.
    - **Feature Extraction**: Extracts meaningful features using methods like SIFT, HOG, or CNNs.
    - **Embeddings**: Converts images into dense vector representations (e.g., using deep learning models like CNNs).
    - **Color Histograms**: Analyzes color distribution in an image.

- **Graph Feature Representation** [[Graph ML]]
  - Methods for processing graph data:
    - **Adjacency Matrix**: Represents graphs as matrices showing node connections.
    - **Node Embeddings**: Converts graph nodes into vector representations (e.g., Node2Vec, GraphSAGE).
    - **Edge Features**: Creates features based on edges in the graph.
    - **Graph Kernels**: Compares graphs using kernel functions.

- **Date and Time Feature Representation**
  - Techniques for processing temporal data:
    - **Extracting Components**: Extracts features like day of the week, month, quarter, etc.
    - **Cyclical Features**: Converts temporal data into cyclic representations (e.g., sin/cos for time of day).
    - **Elapsed Time**: Me
