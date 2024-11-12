# ResearchRec: Academic Paper Recommender and Domain Classifier

ResearchRec is an advanced Natural Language Processing (NLP) project that combines a domain classifier for academic papers and a recommendation system for related research. This project aims to assist researchers in categorizing papers and discovering relevant literature in their field of study.

## Features

1. **Domain Classification**: Automatically categorize academic papers into relevant research domains using a deep learning model.
2. **Paper Recommendation**: Suggest similar academic papers based on the title of a given paper using sentence embeddings.

## Model Training

### Domain Classifier

The domain classifier is trained using a deep learning model with the following architecture:

- Input: TF-IDF vectorized abstract
- Hidden layers: Dense layers with ReLU activation and dropout
- Output: Multi-label classification using sigmoid activation


The model is trained on a dataset of arXiv papers, using binary cross-entropy loss and Adam optimizer.

### Recommendation System

The recommendation system uses the `all-MiniLM-L6-v2` model from the `sentence-transformers` library to generate embeddings for paper titles. Cosine similarity is then used to find the most similar papers.


