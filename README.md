# Multi-PDF Chat Intelligence Agent

## Project Overview
This repository contains a professional-grade Document Intelligence Agent built using the Retrieval-Augmented Generation (RAG) framework. The system allows users to upload multiple PDF documents and engage in a contextual dialogue with the content. It leverages state-of-the-art Large Language Models (LLMs) and vector search technology to provide precise, grounded answers based on the provided documents.

## Technical Architecture
The application follows a structured RAG pipeline:
1. **Data Ingestion:** Extracts raw text data from multi-page PDF files using the PyPDF2 library.
2. **Text Processing:** Implements recursive character-based chunking to maintain semantic coherence and optimize token usage.
3. **Vector Embeddings:** Utilizes Google Generative AI Embeddings to transform text segments into high-dimensional vector representations.
4. **Vector Storage:** Indexes the generated embeddings in a local FAISS (Facebook AI Similarity Search) database for low-latency similarity searches.
5. **Contextual Retrieval:** Performs semantic search to retrieve the most relevant document segments based on the user's query.
6. **Response Generation:** Orchestrates the retrieved context into a prompt for the Gemini 2.5 Flash model to produce accurate and context-aware responses.

## Key Features
* Simultaneous processing of multiple PDF files.
* Local vector store management using FAISS for persistent and fast retrieval.
* Dynamic conversational interface with real-time response generation.
* Robust error handling for API versioning and model deprecation.

## Tech Stack
* **Language:** Python 3.10+
* **LLM:** Google Gemini 2.5 Flash
* **Embeddings:** Google Generative AI (gemini-embedding-001 / text-embedding-004)
* **Framework:** LangChain
* **Frontend:** Streamlit
* **Vector Store:** FAISS
* **Environment Management:** Python-dotenv

## Installation and Setup

1. **Clone the Repository:**
   ```bash
   git clone <https://github.com/RudraanshGupta/Chat-with-PDF/tree/main>
   cd <https://github.com/RudraanshGupta/Chat-with-PDF>
