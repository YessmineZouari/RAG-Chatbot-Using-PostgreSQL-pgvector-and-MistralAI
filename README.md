
# RAG Chatbot Using PostgreSQL, pgvector, and MistralAI

This project demonstrates a **Retrieval-Augmented Generation (RAG) chatbot** that combines **vector embeddings** with a **large language model (LLM)** to answer questions based on a PDF document. It leverages **PostgreSQL** with the **pgvector** extension for efficient vector storage and similarity search, and **MistralAI** models for both embeddings and chat generation.

## Features
- Convert PDF text into embeddings (one vector per line) using **MistralAIEmbeddings**.  
- Store embeddings in **PostgreSQL 13** with **pgvector** extension (VECTOR(1024)).  
- Retrieve the most relevant information for a user query using vector similarity search.  
- Generate structured answers using **ChatMistralAI**.  
- Built with **LangChain** for easy integration of embeddings and chat models.

## Workflow
1. Extract text lines from PDF.  
2. Convert each line into a 1024-dimensional embedding using **MistralAI**.  
3. Store embeddings in PostgreSQL with **pgvector**.  
4. Retrieve relevant lines based on similarity to the user query.  
5. Generate answers with **MistralAI chat model**.

## Requirements
- Python 3.10+  
- PostgreSQL 13 with pgvector extension  
- `langchain-mistralai` Python package  
- Other dependencies in `requirements.txt`  


