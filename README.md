# 📚 Research Paper Recommendation System

## 🌟 Overview
This repository contains the code and resources for the **Research Paper Recommendation System**. The system utilizes various Natural Language Processing (NLP) models to generate embeddings and recommend research papers based on the semantic similarity of their abstracts. Below are the key steps, experiments, and functionalities implemented.

---

## 🔑 Key Notebooks and Their Functions

### 1. 🛠️ **TF-IDF Approach (Notebook 1)**
- **Purpose**: Baseline model to compute abstract similarity using TF-IDF vectors.
- **Key Steps**:
  - Data cleaning and preprocessing (lowercasing, lemmatization, punctuation removal).
  - Generation of TF-IDF vectors for abstracts.
  - Storage and retrieval of TF-IDF vectors using LanceDB.
  - Evaluation using ground truth measures.

### 2. 🧠 **SBERT Pre-trained Model: all-MiniLM-L6-v2 (Notebook 2)**
- **Purpose**: Leveraging Sentence-BERT for dense semantic embeddings.
- **Key Steps**:
  - Data preparation with stratified sampling.
  - Embedding generation using the pre-trained all-MiniLM-L6-v2 model.
  - Storage of embeddings in LanceDB for efficient retrieval.
  - Batch testing using various evaluation metrics.

### 3. 📊 **SBERT Pre-trained Model: allenai-specter (Notebook 3)**
- **Purpose**: Using AllenAI-Specter embeddings optimized for citation-based relationships.
- **Key Steps**:
  - Preprocessing and cleaning data.
  - Generating high-dimensional embeddings for academic abstracts.
  - Efficient embedding storage in LanceDB.
  - Model evaluation for abstract similarity.

### 4. 🔍 **SBERT Fine-Tuning: all-MiniLM-L6-v2 (Notebook 4)**
- **Purpose**: Fine-tuning the all-MiniLM-L6-v2 model for domain-specific tasks.
- **Key Steps**:
  - Fine-tuning using pairs of abstracts (positive/negative pairs).
  - Generating fine-tuned embeddings.
  - Storage and evaluation of fine-tuned embeddings in LanceDB.

### 5. 🌐 **Streamlit Application (Notebook 5)**
- **Purpose**: Deploying a user-friendly interface for abstract-based recommendations.
- **Key Steps**:
  - Generating embeddings using pre-trained and fine-tuned models.
  - Embedding storage and management.
  - Real-time recommendations with optional metadata filtering.
  - Retrieval-Augmented Generation (RAG) for explainability.

---

## 🧪 Results

Here are the key findings and metrics from the experiments:

- **TF-IDF Baseline**: Achieved acceptable results but lacked semantic depth.
- **SBERT Pre-trained (all-MiniLM-L6-v2)**: Significant improvement in capturing semantic similarity.
- **SBERT Fine-Tuned**: Delivered domain-specific enhancements with an accuracy of **78.9%** and an F1 Score of **79.64%**.
- **AllenAI-Specter**: Outperformed other models, achieving the highest relevance scores for scientific abstracts.

🚀 *"AllenAI-Specter embeddings provided the most contextually rich and accurate recommendations."*

---

## 🛠️ Installation and Setup

1. Clone the repository:
   ```bash
   https://github.com/arpannookala12/Research-Paper-Recommendation-based-on-Abstract-Similarity.git
