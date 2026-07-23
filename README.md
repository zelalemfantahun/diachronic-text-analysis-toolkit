# Diachronic Text Analysis Toolkit

A research-oriented Natural Language Processing (NLP) toolkit for extracting, preprocessing, analyzing, and clustering large text corpora from multiple sources, including **Reddit** and **Newsweek**. The project focuses on **diachronic text analysis**—studying how language, topics, and semantic relationships evolve over time using statistical and semantic NLP techniques.

---

## Project Overview

This project was developed as part of graduate research in **Computational Linguistics**. It contains a collection of Python scripts that perform different stages of a text mining workflow, from corpus extraction and preprocessing to phrase extraction, semantic analysis, clustering, and visualization.

Unlike a traditional software package, this repository evolved through research experiments. Each script performs a specific task within the overall workflow, allowing researchers to analyze textual data across different time periods and discover changes in vocabulary, concepts, and semantic relationships.

---

## Research Objectives

- Extract textual data from Reddit archives and news sources
- Clean and normalize large text corpora
- Perform linguistic preprocessing
- Extract noun phrases and meaningful collocations
- Generate statistically significant bigrams
- Build document-term matrices
- Learn semantic representations of words
- Cluster related documents and phrases
- Visualize semantic relationships
- Study language evolution over time

---

# Workflow

```text
                Reddit Archives
               News Articles
                      │
                      ▼
             Corpus Extraction
                      │
                      ▼
         Cleaning & Normalization
                      │
                      ▼
          Phrase Extraction
                      │
                      ▼
      Bigram / Co-occurrence Analysis
                      │
                      ▼
    Document-Term Matrix Construction
                      │
                      ▼
        Word Embeddings (Word2Vec)
                      │
                      ▼
       Clustering & Semantic Analysis
                      │
                      ▼
             Data Visualization
```

---

# Features

- Reddit corpus extraction
- News article processing
- Text cleaning and normalization
- Stopword removal
- WordNet lemmatization
- Porter stemming
- Stanford POS tagging
- Noun phrase extraction
- Phrase extraction
- Bigram generation
- Mutual Information analysis
- Document-Term Matrix generation
- TF-IDF vectorization
- Word embeddings
- Hierarchical clustering
- K-Means clustering
- Semantic similarity analysis
- Word Sense Disambiguation (Lesk Algorithm)
- Synonym analysis
- t-SNE visualization
- Dendrogram visualization

---

# Repository Structure

```
Diachronic-Text-Analysis-Toolkit/

├── Corpus Extraction
│   ├── reddit_extractor.py
│   ├── reddit_pre_process.py
│   ├── Reddit_csv_creator.py
│   ├── csv-year.py
│   ├── csv-4month.py
│   └── ...
│
├── Text Cleaning
│   ├── cleansing.py
│   ├── text_cleaner.py
│   ├── porter_dictionary.py
│   └── ...
│
├── Phrase Extraction
│   ├── phrase_extractor.py
│   ├── phrase_extractor_newsweek.py
│   ├── Noun_Phrase_extractor.py
│   └── ...
│
├── Text Mining
│   ├── Matrix-Builder.py
│   ├── Reddit_bigram_generator.py
│   ├── bigram_generator_MI.py
│   ├── term_document_matrix.py
│   └── ...
│
├── Semantic Analysis
│   ├── word2vec.py
│   ├── Synonyms.py
│   ├── lesk-algorithm.py
│   └── ...
│
├── Clustering & Visualization
│   ├── clustering.py
│   ├── cluster_one.py
│   ├── tf.py
│   ├── tsne.png
│   └── scipy-dendrogram.png
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

# Repository Components

## Corpus Extraction

Scripts for extracting Reddit comments and organizing corpora by day, month, and year.

Examples:

- reddit_extractor.py
- Reddit_csv_creator.py
- csv_creator.py
- csv-year.py
- csv-4month.py

---

## Text Preprocessing

Utilities for cleaning and preparing text.

Includes:

- Stopword removal
- WordNet lemmatization
- Porter stemming
- Text normalization

---

## Phrase Extraction

Extracts noun phrases and linguistic patterns using the Stanford POS Tagger.

Includes:

- Phrase extraction
- Noun phrase extraction
- Corpus-specific extraction

---

## Bigram & Statistical Analysis

Generates:

- Bigram frequencies
- Pointwise Mutual Information (PMI)
- Term frequencies

---

## Semantic Analysis

Implements:

- Word embeddings
- Synonym discovery
- Word Sense Disambiguation
- Semantic similarity

---

## Clustering & Visualization

Provides:

- Hierarchical clustering
- Agglomerative clustering
- K-Means clustering
- t-SNE visualization
- Dendrogram generation

---

# Technology Stack

### Programming Language

- Python

### NLP Libraries

- NLTK
- Stanford POS Tagger
- WordNet
- pywsd
- stemming

### Machine Learning

- Scikit-learn
- Gensim
- fastcluster

### Data Processing

- Pandas
- NumPy
- PyTables (HDF5)

### Visualization

- Matplotlib
- SciPy

---

# Skills Demonstrated

- Natural Language Processing (NLP)
- Computational Linguistics
- Text Mining
- Corpus Linguistics
- Information Retrieval
- Machine Learning
- Statistical Language Processing
- Word Embeddings
- Text Clustering
- Semantic Analysis
- Data Visualization
- Python Programming

---

# Example Applications

This toolkit can be applied to:

- Social Media Analytics
- News Analytics
- Topic Discovery
- Information Retrieval
- Computational Linguistics Research
- Corpus Analysis
- Semantic Search
- Trend Analysis
- Language Evolution Studies

---

# Setup

This repository was originally developed for research and contains scripts written over multiple stages of the project.

To run individual scripts:

1. Install Python and the required libraries.
2. Install project dependencies.

```bash
pip install nltk pandas numpy scipy matplotlib scikit-learn gensim tables fastcluster pywsd stemming
```

3. Download required NLTK datasets.

```python
import nltk

nltk.download("punkt")
nltk.download("wordnet")
nltk.download("stopwords")
```

4. Download the Stanford POS Tagger separately and update local paths where required.

5. Modify file paths to match your local dataset locations.

---

# Known Limitations

This repository reflects an academic research workflow rather than a packaged software library.

Current limitations include:

- No unified pipeline script
- Scripts executed independently
- Hardcoded local file paths
- Mixed Python 2 and Python 3 syntax
- No dependency management in the original project
- Duplicate experimental scripts
- Limited automated testing
- External Stanford POS Tagger dependency

These limitations have been intentionally documented to preserve transparency regarding the original implementation.

---

# Future Improvements

Planned enhancements include:

- Full migration to Python 3
- Modular project structure
- Configuration-based file paths
- Command-line interface (CLI)
- Automated testing
- Complete documentation
- Unified processing pipeline
- Docker support
- Jupyter notebook demonstrations

---

# About the Project

This repository represents graduate-level research in **Computational Linguistics** and demonstrates practical applications of Natural Language Processing, corpus linguistics, semantic analysis, and machine learning for large-scale textual data.

Rather than serving as a standalone application, it provides a collection of research tools that can be adapted for corpus analysis, information retrieval, and language evolution studies.

---

# Author

**Zelalem Abate**

**M.Sc. Computational Linguistics**

Python Developer | Data Analyst | NLP Engineer

GitHub: https://github.com/zelalemfantahun

---

# License

This project is licensed under the MIT License. See the LICENSE file for details.
