# VC and Startup Recommendation Engine

This project provides a recommendation engine to match venture capital (VC) firms with startups based on their descriptions, funding history, and other relevant attributes. It leverages text embeddings and similarity search to recommend the best VC firms for a given startup.

## Overview

The recommendation engine works as follows:
1. **Data Preparation**: VC and startup data are loaded and transformed into structured text documents.
2. **Text Embeddings**: Text embeddings are generated using the `sentence-transformers/all-MiniLM-L6-v2` model.
3. **Vector Store**: A Chroma vector store is created to enable similarity-based search.
4. **Recommendation**: For a given startup, the top-k most similar VC firms are recommended based on the embeddings.

## Key Features
- **Flexible Text Creation**: Customizable functions to format VC and startup data into structured text.
- **Advanced Embedding Model**: Uses the `sentence-transformers/all-MiniLM-L6-v2` model for high-quality embeddings.
- **Efficient Search**: Chroma vector store enables fast and scalable similarity search.
- **Customizable Recommendations**: Adjustable number of top-k results.

## Installation

Install the required Python packages:

```bash
pip install langchain chromadb sentence-transformers streamlit
pip install -U langchain-community
