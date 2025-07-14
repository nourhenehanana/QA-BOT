# 📚🔍 RAG-PDF QA System

A retrieval‑augmented generation (RAG) system built with **FastAPI** that ingests user‑uploaded PDFs and answers user questions with high precision.

## ✨ Features
- **PDF Ingestion**: Upload PDFs via a simple API; text is extracted and processed.
- **Token‑Level Chunking**: Splits long documents into context‑aware segments optimized for LLM input limits.
- **Vector Search**: Uses FAISS to index document embeddings and enable fast semantic retrieval.
- **Answer Generation**: Combines retrieved text with a Gemini LLM to provide concise, context‑relevant answers.
- **Modular RAG Pipeline**: Built with LangChain for orchestration of ingestion, retrieval, and generation.

## ⚙️ Tech Stack
- **FastAPI** — High-performance web framework for building APIs
- **LangChain** — RAG pipeline orchestration
- **FAISS** — Efficient similarity search in large vector spaces
- **Gemini LLM** — Large language model for answer generation
- **Python** — Core language for processing and orchestration

## 🚀 Getting Started

Create and activate a virtual environment:

bash
Copier le code
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
Install dependencies:

bash
Copier le code
pip install -r requirements.txt
📦 Running the API
Start the FastAPI server:

bash
Copier le code
uvicorn app:app --reload
Once running, navigate to:

Upload PDFs

Ask questions

View answers in real time

# 🧠 How it Works
Text Extraction: Extracts text from uploaded PDFs.

Chunking: Splits text into overlapping chunks to preserve context.

Embedding: Converts text chunks into vectors using an embedding model.

Indexing: Stores vectors in a FAISS database for efficient semantic search.

Retrieval & Generation: On question input, retrieves relevant chunks and uses Gemini to generate an answer.

# 📌 Roadmap
Add user authentication

Enable support for other file types (Word, HTML)

Deploy to production (Docker & cloud)
