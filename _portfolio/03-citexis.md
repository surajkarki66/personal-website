---
title: "Citexis"
excerpt: "A hybrid academic paper discovery platform combining semantic search, keyword search, and recommendations."
collection: portfolio
permalink: /portfolio/citexis/
header:
  teaser: portfolio/citexis.png
---

![Citexis](/images/portfolio/citexis.png)

Citexis is a hybrid academic paper discovery platform. Paper metadata lives in **MongoDB**, semantic search runs on **Pinecone**, and keyword search on **Elasticsearch**, with a **React** frontend and **Celery + Redis** for background bulk imports.

**Features**

* **Hybrid search:** BM25 keyword results from Elasticsearch and semantic results from Pinecone (with optional reranking) are merged using reciprocal rank fusion, then hydrated from MongoDB.
* **Recommendations:** related papers from content similarity, citation edges, and collaborative signals from user interactions, combined with weighted rank fusion.
* **Ingestion:** import papers from OpenAlex, Crossref DOIs, arXiv search, or JSON files, with optional CORE full-text enrichment; bulk imports run asynchronously as Celery tasks.
* **Explore:** topic clusters, citation neighbours, author pages, saved papers, and ratings, with JWT-based authentication and admin-only import.

**Tech stack:** Python · FastAPI · MongoDB · Pinecone · Elasticsearch · Celery · Redis · React · TypeScript · Tailwind CSS

[Source code](https://github.com/surajkarki66/citexis)
