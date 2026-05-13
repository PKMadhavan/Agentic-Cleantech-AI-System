# Agentic Cleantech AI System

A Retrieval-Augmented Generation (RAG) agent for Cleantech news and data, combining semantic search over curated industry articles with real-time web retrieval.

## Overview

This project demonstrates an end-to-end RAG pipeline that delivers accurate, grounded answers on cleantech topics — both historical and current — using a hybrid agent architecture.

## Features

- **Data Ingestion & Indexing** — Loads and processes cleantech datasets, embedding them for efficient semantic search
- **Vector Database Retrieval** — Uses OpenAI embeddings and ChromaDB for context-aware document retrieval
- **Hybrid Agent Orchestration** — Custom ReAct agent prioritizes internal sources, falls back to Tavily web search for current events
- **Conversational Memory** — Tracks multi-turn interactions for grounded, context-rich responses
- **Rigorous Evaluation** — Validates retrieval and answer quality using LLM-as-a-judge scoring and reference-based precision

## Tech Stack

| Component | Technology |
|---|---|
| LLM | OpenAI GPT-4o-mini |
| Embeddings | OpenAI text-embedding-3-small |
| Vector Store | ChromaDB |
| Agent Framework | LangChain |
| Web Search | Tavily |
| Data | Pandas |

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/PKMadhavan/Agentic-Cleantech-AI-System.git
   cd Agentic-Cleantech-AI-System
   ```

2. Install dependencies:
   ```bash
   pip install langchain langchain-openai langchain-chroma chromadb openai tavily-python langchain-community pandas
   ```

3. Set environment variables:
   ```bash
   export OPENAI_API_KEY="your-openai-api-key"
   export TAVILY_API_KEY="your-tavily-api-key"
   ```

4. Open and run the notebook:
   ```bash
   jupyter notebook "Agentic-Cleantech-AI-System .ipynb"
   ```

## Evaluation Results

| Metric | Score |
|---|---|
| Retrieval Accuracy (Hit Rate) | 100% |
| Response Accuracy (LLM Judge) | 100% |

## Author

**Madhavan Panneerselvam Kumar**  
Course: CSC 583 — Natural Language Processing
