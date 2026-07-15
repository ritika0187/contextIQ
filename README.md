# ContextIQ

<div align="center">

### AI-Powered Semantic Search & Retrieval-Augmented Generation (RAG) Engine in Modern C++

Explore how vector search, semantic retrieval, and local language models work together through an interactive C++ implementation.

</div>

---

## Overview

ContextIQ is an educational project that demonstrates the core concepts behind modern vector databases and Retrieval-Augmented Generation (RAG). It combines multiple nearest-neighbor search algorithms with local AI models to enable semantic document search and context-aware question answering.

The project provides a practical way to understand how vector embeddings are indexed, searched, and used to retrieve relevant information before generating AI responses.

---

## Key Features

- **Multiple Search Algorithms**
  - Hierarchical Navigable Small World (HNSW)
  - KD-Tree
  - Brute Force Search

- **Distance Metrics**
  - Cosine Similarity
  - Euclidean Distance
  - Manhattan Distance

- **Semantic Document Search**
  - Generate vector embeddings using Ollama
  - Index and retrieve documents efficiently
  - Automatic document chunking

- **Retrieval-Augmented Generation**
  - Context-aware AI responses
  - Local inference using Ollama
  - Semantic retrieval before generation

- **Interactive Visualization**
  - PCA-based 2D vector projection
  - Compare search algorithms
  - Visualize semantic clusters

- **REST API**
  - Vector insertion
  - Vector deletion
  - Similarity search
  - Benchmarking
  - Document management
  - AI-powered question answering

---

## Tech Stack

| Category | Technologies |
|----------|--------------|
| Language | C++17 |
| AI Models | Ollama |
| Embeddings | nomic-embed-text |
| LLM | llama3.2 |
| Algorithms | HNSW, KD-Tree, Brute Force |
| HTTP Library | cpp-httplib |
| Frontend | HTML, CSS, JavaScript |

---

## Project Workflow

```
User Query
      │
      ▼
Generate Embedding
      │
      ▼
Vector Search
(HNSW / KD-Tree / Brute Force)
      │
      ▼
Retrieve Relevant Context
      │
      ▼
Generate AI Response
      │
      ▼
Return Results
```

---

## Project Structure

```
ContextIQ/
├── main.cpp
├── httplib.h
├── index.html
└── README.md
```

---

## Getting Started

### Prerequisites

- Git
- C++17 Compiler
- Ollama

Download the required models:

```bash
ollama pull nomic-embed-text
ollama pull llama3.2
```

---

### Clone the Repository

```bash
git clone https://github.com/<your-github-username>/ContextIQ.git

cd ContextIQ
```

---

### Build

#### Windows

```bash
g++ -std=c++17 -O2 main.cpp -o db -lws2_32
```

#### macOS / Linux

```bash
g++ -std=c++17 -O2 main.cpp -o db
```

---

### Run

Start Ollama:

```bash
ollama serve
```

Run the application:

```bash
./db
```

Open your browser:

```
http://localhost:8080
```

---

## API Highlights

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | `/search` | Semantic vector search |
| POST | `/insert` | Insert vector |
| DELETE | `/delete/:id` | Delete vector |
| GET | `/benchmark` | Compare search algorithms |
| POST | `/doc/insert` | Store document embeddings |
| POST | `/doc/ask` | Retrieve context and generate AI response |

---

## Learning Outcomes

This project demonstrates practical concepts in:

- Vector Databases
- Semantic Search
- Approximate Nearest Neighbor Search
- Retrieval-Augmented Generation (RAG)
- Information Retrieval
- Local Large Language Models
- REST API Development in C++

---

## Future Enhancements

- Persistent vector storage
- PDF and DOCX document support
- Authentication and user management
- Docker deployment
- Hybrid keyword + semantic search
- GPU acceleration
- Streaming AI responses

---
