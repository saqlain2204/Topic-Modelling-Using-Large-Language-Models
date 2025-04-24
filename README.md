<p align="center">
  <img src="assets/github banner.png" alt="TopiQ Logo" width="100%" />
</p>

This repository contains a Jupyter Notebook that demonstrates topic modeling on research paper abstracts using Large Language Models (LLMs). The project extends beyond topic modeling to include advanced graph analytics, providing deep insights into the relationships between extracted topics.

---

## Dataset

The dataset used in this project is sourced from Kaggle:  
- [Research Abstracts Dataset](https://www.kaggle.com/datasets/saqlain22/research-abstracts)

This dataset consists of research paper abstracts, which are analyzed to uncover latent topics and their relationships. Please download the dataset from the link above and place it in the working directory before running the notebook.

---

## Dependencies

The project requires the following Python libraries:

### Core Libraries:
- **`pandas`**: For data manipulation and analysis.
- **`numpy`**: For numerical computations.
- **`matplotlib`**: For visualization of clustering, topics, and graphs.

### Clustering and Dimensionality Reduction:
- **`umap-learn`**: For reducing high-dimensional embeddings to lower dimensions.
- **`hdbscan`**: For hierarchical density-based clustering of data.

### Machine Learning Models:
- **`sentence-transformers`**: For generating embeddings of text data.
- **`transformers`**: To use the Llama2 model for topic extraction.

### Topic Modeling Techniques:
- **`KeyBERT`**: For extracting representative keywords of a topic.
- **`UMAP`**: For dimensionality reduction.
- **`HDBSCAN`**: For identifying meaningful clusters.
- **`MMR (Maximal Marginal Relevance)`**: For selecting diverse and representative topics.

### Graph Analytics:
- **`networkx`**: For creating and analyzing topic graphs.

---

## Notebook Features

1. **Data Exploration**:
   - Detailed exploration of the Kaggle dataset to understand its structure and content.

2. **Text Embedding**:
   - Utilizes `sentence-transformers` to embed abstracts into high-dimensional vectors.

3. **Dimensionality Reduction**:
   - UMAP reduces embeddings to 2D for better interpretability and visualization.

4. **Clustering**:
   - HDBSCAN identifies clusters of abstracts representing different topics.

5. **Topic Extraction**:
   - Extracts meaningful topics using `KeyBERT`, `Llama2`, and `MMR`.

6. **Graph Construction and Analytics**:
   - Constructs a graph from the extracted topics based on similarity.
   - Performs advanced graph analytics:
     - **Betweenness Centrality**: Identifies influential nodes in the topic network.
     - **Community Detection**: Groups related topics into communities.
     - **K-Cores**: Finds dense subgraphs within the topic network.
     - **Subgraph Generation**: Creates subgraphs for specific topics to analyze their local structure.

7. **Visualization**:
   - Visualizes clustering, topic distributions, and graph structures.

---

## Team

This project was developed by:

- **[Mohammed Saqlain](https://github.com/saqlain2204)**
- **[Nishaan Padanthaya](https://github.com/nishaanpadanthaya)**
