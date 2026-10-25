---
title: "Agentic Researcher"
excerpt: "A CrewAI multi-agent system that researches, writes, and edits a one-page scientific document on any topic."
collection: portfolio
permalink: /portfolio/agentic-researcher/
header:
  teaser: portfolio/thumbs/agentic-researcher.jpg
---

![Agentic Researcher](/images/portfolio/agentic-researcher.png)

Agentic Researcher is a CrewAI-powered multi-agent system that automatically generates a comprehensive, evidence-based one-page scientific document on any concrete scientific topic.

**How it works:** three specialized agents work in sequence.

1. **Scientific Researcher:** gathers information from academic literature via a custom arXiv search tool, plus web search and scraping.
2. **Scientific Writer:** turns the findings into a clear, structured 500–650 word document with inline citations.
3. **Editor:** reviews for accuracy, clarity, structure, and length to produce a publication-ready report.

**Tech stack:** Python · CrewAI · LLM Agents · arXiv API · Serper · LiteLLM · Ollama

[Source code](https://github.com/surajkarki66/agentic_researcher)
