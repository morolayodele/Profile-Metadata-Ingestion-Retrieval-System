# Profile Metadata Ingestion & Query System

This project processes structured `.docx` consultant profiles, extracts key metadata fields (e.g., roles, responsibilities, tech stacks), generates sentence embeddings using `SentenceTransformers`, and stores the results in a persistent ChromaDB vector store. A LangChain-powered agent enables querying those profiles via natural language, with an optional Streamlit UI.

---

## Overview

This system is structured in two parts:

1. **Ingestion (`profilechunks.py`)**  
   Parses `.docx` files, extracts structured metadata, and stores embedded summaries in ChromaDB.

2. **Query Interface (`streamlitprofilechunks.py`)**  
   Launches a Streamlit app that uses a LangChain agent to respond to user queries using the stored vector data.

---

## Prerequisites

- Python 3.10+
- Virtual environment (`chroma-env`) with required libraries installed
- `.docx` consultant profiles with a consistent structure

---

## Directory Structure

