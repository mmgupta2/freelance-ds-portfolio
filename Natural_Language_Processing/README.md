# Topic Modeling & Text Analysis with LDA and BERTopic

## Overview

This project applies both classical and transformer-based natural language processing techniques to extract topics and themes from financial news articles. We use LDA for traditional probabilistic topic modeling and BERTopic to leverage contextual embeddings for more nuanced insights.

## Business Relevance

Companies, think tanks, and financial analysts deal with overwhelming volumes of text — from news feeds to internal reports. This project shows how automated topic modeling can help:

- Track narratives about key economic actors (e.g., OPEC)
- Detect emerging themes in financial reporting
- Enhance competitive intelligence and market sentiment analysis

This pipeline could easily be adapted for investment firms, media monitoring, or internal knowledge discovery.

## Tools & Technologies Used

- Python, pandas, seaborn, matplotlib
- NLTK for preprocessing and lemmatization
- Gensim (LDA + Coherence Scoring)
- BERTopic + Sentence Transformers
- pyLDAvis for visual topic exploration

## Problem Statement

Given a dataset of news articles (Factiva-sourced), how can we extract and label dominant topics or themes without manually reading every article?

## Approach

1. **Data Preparation**

   - Loaded and cleaned a collection of financial news articles.
   - Applied lemmatization, stopword removal, and tokenization.

2. **LDA Topic Modeling**

   - Built a Gensim-based LDA model on cleaned tokens.
   - Tuned number of topics using coherence score.
   - Visualized output with pyLDAvis.

3. **BERTopic (Transformer-Based)**

   - Used sentence-transformers (e.g., `all-MiniLM-L6-v2`) to generate document embeddings.
   - Applied UMAP + HDBSCAN for clustering.
   - Extracted and labeled topic keywords using BERTopic's built-in pipeline.

4. **Comparison**

   - Contra

