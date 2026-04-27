# AI Document Q&A using RAG

## Overview
This project implements a Retrieval-Augmented Generation (RAG) system that enables users to query PDF documents and receive accurate, context-aware answers using LLMs.

## Structure
ai-rag-document-qa/
 ├── RAG_pdf_bot.ipynb
 ├── README.md        
 ├── screenshot.png
 ├── IKS_4001_MII_Lecture_0.pdf (used as sample.pdf)
 
## Features
- 📄 PDF document ingestion
- ✂️ Text chunking for efficient processing
- 🔍 Semantic search using FAISS vector database
- 🤖 LLM-based answer generation (HuggingFace)
- ⚡ Fast and context-aware responses

## Tech Stack
- Python
- LangChain
- FAISS (Vector Database)
- HuggingFace Transformers
- Google Colab

## How it Works
1. Load PDF document
2. Split into smaller chunks
3. Convert chunks into embeddings
4. Store embeddings in FAISS
5. Retrieve relevant chunks based on query
6. Generate answer using LLM

## Architecture
PDF → Chunking → Embeddings → FAISS → Retrieval → LLM → Answer

## Key Concepts
- Retrieval-Augmented Generation (RAG)
- Semantic Search
- Vector Embeddings
- Context-aware Answer Generation

## Example Query
### Query
Summarize this document

### Answer
The document describes the Indus Valley Civilisation as an advanced urban society known for its organized city planning, sanitation systems, and strong trade networks. The economy was based on agriculture and trade, with standardized weights and measures ensuring consistency. The people were skilled in crafts such as pottery, metallurgy, and bead-making. Social life appears peaceful and well-structured, with no clear evidence of large palaces or temples. Although the script remains undeciphered, findings suggest nature and animal worship. Overall, the civilisation demonstrated strong practical knowledge and laid the foundation for later cultures in the Indian subcontinent.

## Output Screenshot
![RAG Output](screenshot.png)

## Future Improvements
- FastAPI backend for API access
- Deployment on AWS / cloud platform
- Frontend interface (React)
- Support for multiple documents
- Performance optimization

## Author
Developed as part of learning AI + Backend integration using RAG pipelines.
