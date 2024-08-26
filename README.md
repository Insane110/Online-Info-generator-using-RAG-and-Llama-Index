# RAG Implementation Project
This project implements a Retrieval-Augmented Generation (RAG) system using a variety of tools and frameworks to achieve efficient and accurate text extraction, processing, and retrieval.
## Overview
This RAG implementation is built using the LlamaIndex framework, which was chosen over Langchain due to its superior performance in online data extraction tasks. The project leverages several technologies for web scraping, text extraction, and data processing:

### Web Scraping:
**DuckDuckGo**: Used as the search engine for gathering web pages.

**OpenCV and Tesseract**: Utilized for extracting text from images found on web pages.

**Table Extraction**: Extracted data from tables on web pages, converting them into documents for further processing.

### Document Processing:
Converted scraped data into documents.
Removed empty documents, retaining only those with meaningful content.

### Language Model:
**Hugging Face**: Integrated the Meta-Llama-3.1-8B-Instruct model as the primary LLM.

**Embedding Model**: Used sentence-transformers/all-MiniLM-L6-v2 for generating embeddings.

### Vector Database:
Used FAISS for vector indexing to optimize search and retrieval performance, replacing the default VectorStoreIndex.

### Bot Interface:
Built an interactive bot interface using Gradio.

### Features
**Efficient Data Retrieval**: Leverages FAISS for fast and accurate retrieval of relevant documents.

**Versatile Text Extraction**: Supports text scraping from various sources, including images and tables.

**Scalable Framework**: Built on top of LlamaIndex, allowing for easy integration and scaling.
