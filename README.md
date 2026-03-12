This repo provides the source code & data for RAG POCs

Overview 
A real-time RAG (Retrieval-Augmented Generation) system that allows users to upload documents (PDF, text) and ask questions. 
The system splits documents into chunks, generates embeddings, stores them in a vector database, and retrieves relevant information for answering user queries using an LLM.

## Project Structure

- `data/` – Store uploaded PDFs or text files.
- `ingestion/` – Scripts for loading and chunking documents.
- `embeddings/` – Scripts for generating vector embeddings.
- `vector_store/` – FAISS/Pinecone/Milvus integration.
- `retrieval/` – Query the vector database for relevant chunks.
- `llm/` – Send retrieved chunks to an LLM for answers.
- `app/` – FastAPI backend for real-time querying.
- `main.py` – Orchestrates the full RAG pipeline.
- `requirements.txt` – Python dependencies.
- `.env` – Environment variables like API keys.
