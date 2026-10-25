---
title: "RAG Researcher"
excerpt: "A fully local retrieval-augmented generation (RAG) assistant for analyzing and chatting with research papers."
collection: portfolio
permalink: /portfolio/rag-researcher/
header:
  teaser: portfolio/rag-researcher.png
---

![RAG Researcher](/images/portfolio/rag-researcher.png)

RAG Researcher is a retrieval-augmented generation system for analyzing and understanding research papers, running entirely on local models so no data leaves your machine.

**Features**

* **Local AI:** Llama 3 via Ollama for generation and `nomic-embed-text` for embeddings, fully offline.
* **Multi-query retrieval:** generates several variations of each question to retrieve better-matching document chunks.
* **PDF processing:** robust loading and configurable text chunking, stored in a **ChromaDB** vector database.
* **Interactive chat:** terminal interface with streaming answers and the option to inspect the retrieved source chunks.

**Tech stack:** Python · LangChain · Ollama · Llama 3 · ChromaDB · RAG

[Source code](https://github.com/surajkarki66/RAG-Research-Assistant)
