# 📚 Mini RAG – Document Question Answering

This is a simple **Retrieval-Augmented Generation (RAG)** application that lets you upload a PDF and ask questions about its content.

Instead of sending the entire document to an AI model, the application breaks the PDF into smaller chunks, converts those chunks into embeddings, stores them in ChromaDB, and retrieves the most relevant parts when you ask a question.

The retrieved information is then passed to an Ollama model to generate the answer.

## ✨ What it does

- Upload a text-based PDF
- Extract text from the PDF
- Split the document into smaller chunks
- Create embeddings using Sentence Transformers
- Store the embeddings in ChromaDB
- Search for relevant chunks based on your question
- Generate answers using Ollama
- Display the retrieved context along with the answer

## 🛠️ Technologies Used

- **Python** – Main programming language
- **Streamlit** – Web interface
- **PyPDF** – Extracts text from PDF files
- **Sentence Transformers** – Creates text embeddings
- **ChromaDB** – Stores and retrieves document embeddings
- **Ollama** – Runs the local AI model

## 🔄 How it works

The application follows a simple RAG pipeline:

```text
PDF
 ↓
Text Extraction
 ↓
Chunking
 ↓
Embeddings
 ↓
ChromaDB
 ↓
Question
 ↓
Relevant Chunks
 ↓
Ollama
 ↓
Answer
