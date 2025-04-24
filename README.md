<p align="center">
  <img src="assets/topiq.png" alt="TopiQ Logo" style="width: 900px; height: 300px;" />
</p>

# TopiQ: Topic Modeling and Graph Analytics on Research Paper Abstracts

This repository contains a Jupyter Notebook that demonstrates **Topic Modeling** on research paper abstracts using **Large Language Models (LLMs)**. The project goes beyond basic topic modeling by incorporating **advanced graph analytics**, offering deep insights into the relationships between extracted topics. The notebook also provides comprehensive visualizations of topic clustering, topic networks, and their respective structures.

---

## Dataset

The dataset used in this project is sourced from Kaggle:

- **[Research Abstracts Dataset](https://www.kaggle.com/datasets/saqlain22/research-abstracts)**

This dataset consists of research paper abstracts, which are analyzed to uncover latent topics and their relationships. Please download the dataset from the link above and place it in the working directory before running the notebook.

---

## Dependencies

The project requires the following Python libraries:

### Core Libraries:
- **`pandas`**: For data manipulation and analysis.
- **`numpy`**: For numerical computations.
- **`matplotlib`**: For visualizing clustering, topics, and graphs.

### Clustering and Dimensionality Reduction:
- **`umap-learn`**: For reducing high-dimensional embeddings to lower dimensions.
- **`hdbscan`**: For hierarchical density-based clustering of data.

### Machine Learning Models:
- **`sentence-transformers`**: For generating embeddings of text data.
- **`transformers`**: To use the **Llama2** model for topic extraction.

### Topic Modeling Techniques:
- **`KeyBERT`**: For extracting representative keywords of a topic.
- **`UMAP`**: For dimensionality reduction.
- **`HDBSCAN`**: For identifying meaningful clusters.
- **`MMR (Maximal Marginal Relevance)`**: For selecting diverse and representative topics.

### Graph Analytics:
- **`networkx`**: For creating and analyzing topic graphs.

---

## Notebook Features

### 1. **Data Exploration**
   - Thorough exploration of the **Research Abstracts Dataset** to understand its structure and content. This step prepares the data for further analysis and modeling.

### 2. **Text Embedding**
   - Utilizes **`sentence-transformers`** to convert research abstracts into high-dimensional embeddings for more effective topic modeling.

### 3. **Dimensionality Reduction**
   - Uses **UMAP (Uniform Manifold Approximation and Projection)** to reduce the high-dimensional embeddings to a 2D space, making it easier to visualize and interpret the data.

### 4. **Clustering**
   - **HDBSCAN** (Hierarchical Density-Based Spatial Clustering of Applications with Noise) is employed to identify clusters of research abstracts, each representing a distinct topic.

### 5. **Topic Extraction**
   - Extracts representative topics using multiple techniques:
     - **`KeyBERT`** for extracting keywords.
     - **`Llama2`** (LLM) for advanced topic extraction.
     - **`MMR (Maximal Marginal Relevance)`** for selecting the most diverse and representative topics.

### 6. **Graph Construction and Analytics**
   - Constructs a graph from the extracted topics based on similarity.
   - Performs advanced graph analytics:
     - **Betweenness Centrality**: Identifies influential nodes in the topic network.
     - **Community Detection**: Groups related topics into communities.
     - **K-Cores**: Finds dense subgraphs within the topic network.
     - **Subgraph Generation**: Creates subgraphs for specific topics to analyze their local structure.

### 7. **Visualization**
   - Visualizes clustering, topic distributions, and graph structures for better understanding and interpretation.

---

## Team

This project was developed by:

- **[Mohammed Saqlain](https://github.com/saqlain2204)**
- **[Nishaan Padanthaya](https://github.com/nishaanpadanthaya)**
