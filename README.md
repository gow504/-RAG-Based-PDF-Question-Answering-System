# RAG-Based PDF Question Answering System

## Project Overview
This project is a Retrieval-Augmented Generation (RAG) application that allows users to ask questions about PDF documents and receive context-based answers using Large Language Models (LLMs).

It uses LangChain to manage the RAG pipeline, Hugging Face embeddings to convert text into numerical vectors, ChromaDB to store and retrieve document embeddings, and Groq to generate responses using an LLM.

## Technologies Used
- Python
- LangChain
- Hugging Face Embeddings
- ChromaDB
- Groq API
- LLaMA / GPT-OSS models
- PyPDFLoader
- CharacterTextSplitter

## Project Workflow
1. Load PDF documents using PyPDFLoader.
2. Split the extracted text into smaller chunks.
3. Convert text chunks into numerical embeddings using Hugging Face.
4. Store embeddings in the ChromaDB vector database.
5. Retrieve relevant document chunks based on user questions.
6. Pass retrieved context to the LLM through LangChain.
7. Generate answers based on the provided document context.

## Key Features
- PDF document loading and processing.
- Semantic search using vector embeddings.
- Context-based question answering.
- Persistent vector database storage.
- LLM-powered response generation.
- Basic error handling.

## Installation

Install the required packages:

```bash
pip install langchain langchain-classic langchain-community langchain-chroma langchain-huggingface langchain-groq langchain-text-splitters chromadb sentence-transformers pypdf
```

## API Configuration

Create a Groq API key and store it securely as an environment variable.

```python
import os

os.environ["GROQ_API_KEY"] = "YOUR_GROQ_API_KEY"
```

Never upload your actual API key to GitHub.

## Run the Project

1. Install the required dependencies.
2. Configure your Groq API key.
3. Provide a PDF document.
4. Run the notebook or application.
5. Enter questions related to the uploaded PDF.
6. Receive answers based on retrieved document information.

## Learning Outcomes
- Understanding Retrieval-Augmented Generation (RAG).
- Working with Large Language Models.
- Implementing text embeddings.
- Using vector databases for semantic search.
- Building document-based AI applications.
- Integrating LLMs using LangChain.
