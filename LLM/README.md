# LLM-Powered Chatbot with Retrieval-Augmented Generation (RAG)

## Overview

This project demonstrates how to build a large language model (LLM) powered chatbot that combines open-domain generation with domain-specific context using retrieval-augmented generation (RAG). The pipeline integrates a quantized LLaMA model, Elasticsearch as a vector database, and the Haystack framework to create a scalable, modular chatbot system.

## Business Relevance

Businesses across industries are seeking ways to:
- Reduce customer support costs
- Improve employee knowledge access
- Enhance user experience with natural language tools

This chatbot pipeline shows how to deploy a lightweight LLM capable of domain-specific responses using real-time document retrieval — a critical feature for building trust and precision in high-stakes industries like finance, legal, or healthcare.

## Tools & Technologies Used

- Hugging Face Transformers & Hub API
- 4-bit quantized **LLaMA 3.2B Instruct** model
- **Haystack framework** for RAG
- **Elasticsearch** (BM25) for document storage and retrieval
- Sentence Transformers for embedding generation
- Streamlit (optional for deployment/UI)

## Problem Statement

How can we create a lightweight but powerful LLM chatbot that:
- Understands user queries in natural language
- Pulls in real, up-to-date content from a business’s document corpus
- Returns concise, human-like answers with references

## Approach

1. **Model Setup**
   - Loaded LLaMA 3.2B in 4-bit quantized format to reduce memory use
   - Connected to Hugging Face Hub with token authentication

2. **Data Indexing**
   - Used Haystack components to convert, chunk, and embed documents
   - Stored them in an Elasticsearch document store using BM25 retriever

3. **Prompt Construction & Generation**
   - Built custom prompt templates for task-specific generation
   - Integrated HuggingFaceAPIGenerator with retrieval pipeline

4. **Evaluation & Debugging**
   - Performed local testing via notebook and REST queries to Elasticsearch
   - Validated relevance of answers using sample document sets

## Results

- Chatbot can answer questions grounded in indexed business documents
- Fast query resolution with context-aware responses
- Modular system allows you to switch out model, retriever, or prompt logic easily
