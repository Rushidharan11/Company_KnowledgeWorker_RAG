# Company Knowledge Worker - RAG

An AI-powered Retrieval-Augmented Generation (RAG) assistant that answers questions using a company's internal knowledge base. The system retrieves the most relevant document chunks and uses LLM to generate grounded responses.

## Features

- Retrieval-Augmented Generation (RAG)
- Semantic search over company knowledge base
- Source chunk visualization
- Interactive Gradio chat interface
- RAG evaluation dashboard for retrieval and answer quality

## Tech Stack

- Python
- LangChain
- ChromaDB
- OpenAI / HuggingFace Embeddings
- Gradio
- LLM - OpenAI (`gpt-4.1-nano`)
- NumPy

## Demo

🎥 **Project Demo:** [Watch the demo](assets/pro.mp4)

## Setup

### 1. Initialize the project

```bash
uv sync
```

### 2. Create the vector database

Run the ingestion script to process the knowledge base and generate embeddings.

```bash
uv run ingest.py
```

### 3. Launch the RAG application

Start the Gradio chat interface.

```bash
uv run app.py
```

### 4. Evaluate the RAG system

Launch the evaluation interface to measure retrieval and answer quality.

```bash
uv run evaluator.py
```

> **Note:** Create a `.env` file with your OpenAI API key before running the project.