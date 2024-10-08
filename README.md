# [DeepLearning.AI] Buildings Applications with Vector Databases course

Personal notes and code for the **DeepLearning.AI** course [Building Applications with Vector Databases](https://www.deeplearning.ai/short-courses/building-applications-vector-databases/).

## Requirements

* Python 3.10+
* Poetry
* Pinecone API Key
* OpenAI API Key

### Getting Started

1. **Install dependencies:**
```bash
poetry install
```

2. **Set up environment variables:**

Create a .env file in the root directory of the project.
Add the following environment variables to the .env file:
```
PINECONE_API_KEY=<Pinecone API Key>
OPENAI_API_KEY=<OpenAI API Key>
```

3. Run the desired notebook.

# Lesson 1: Semantic Search

Semantic search is a type of search that focuses on the meaning of the content being searched, as opposed to lexical search, which looks for literal matches or pattern-matched strings.

This is an extremely powerful concept that underlies much of what we see in text-oriented generative AI applications.

![Semantic Search](./images/semantic_search.png)

📝 **Notebook:** [01_semantic_search.ipynb](./notebooks/01_semantic_search.ipynb)

## Lesson 2: Retrieval Augmented Generation (RAG)

The RAG (Retrieval-Augmented Generation) system is a method that combines retrieval of relevant documents or data from an external source with the generation of natural language responses, usually via a generative model. Here’s a simplified breakdown:

* **Retrieval:** The system first searches a database or document corpus to fetch relevant pieces of information based on a user's query.
* **Augmented Generation:** It then uses a generative model to generate a response, but instead of purely relying on what it has been trained on, it incorporates the retrieved information to create a more accurate and contextually relevant answer.

This system is particularly useful for enhancing the accuracy and specificity of AI-generated responses, as it can access up-to-date or domain-specific information from external sources.

![RAG](/images/rag.png)

📝 **Notebook:** [02_rag.ipynb](./notebooks/02_rag.ipynb)

## Lesson 3: Recommender Systems

In the context of vector databases, **recommender systems** leverage high-dimensional vectors to capture the semantic similarity between items (such as products, news, or users) by embedding them into a shared vector space. The system then uses the vector representations to perform similarity searches, allowing for efficient and accurate recommendations based on proximity between vectors, which represents likeness in preferences, behavior, or content attributes. This approach is particularly useful for large-scale recommendation tasks due to its scalability and speed.

![Recommender System](/images/recommender_system.png)

📝 **Notebook:** [03_recommender.ipynb](./notebooks/03_recommender.ipynb)

## Lesson 4: Hybrid Search

Pinecone supports vectors with sparse and dense values, which allows you to perform hybrid search on your Pinecone index. Hybrid search combines semantic and keyword search in one query for more relevant results. Semantic search results for out-of-domain queries can be less relevant; combining these with keyword search results can improve relevance.

![Hybrid Search](/images/hybrid_search.png)

📝 **Notebook:** [04_hybrid_search.ipynb](./notebooks/04_hybrid_search.ipynb)

## Lesson 5: Facial Similarity Search

Technique used to find faces that look similar to a given face within a dataset. The process involves converting facial images into numerical representations (embeddings) and then comparing these embeddings to determine the degree of similarity.

![Facial Similarity Search](/images/facial_similarity_search.png)

### Reducing dimension of the data

![pca-tsne](/images/pca_tsne.png)
![PCA](/images/pca.png)
![T-SNE](/images/tsne.png)


📝 **Notebook:** [05_facial_similarity_search.ipynb](./notebooks/05_facial_similarity_search.ipynb)

## Lesson 6: Anomaly Detection

![Anomaly Detection](/images/anomaly_detection.png)


📝 **Notebook:** [06_anomaly_detection.ipynb](./notebooks/06_anomaly_detection.ipynb)

### Contributions

This repository is created to be used as a companion for the DeepLearning.AI course [Building Applications with Vector Databases](https://www.deeplearning.ai/short-courses/building-applications-vector-databases/). Feel free to use it to learn about the course content and as a reference for future projects.