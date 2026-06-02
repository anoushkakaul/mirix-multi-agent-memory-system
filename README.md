# MIRIX: Multi-Agent Memory System for LLM-Based Agents

A MIRIX-inspired memory architecture that simulates how intelligent AI agents can store, organize, retrieve, and reason over different categories of memory using LangGraph, Large Language Models (LLMs), and semantic retrieval techniques.

## Overview

Modern AI agents require more than simple conversation history. They need structured memory systems capable of storing personal preferences, experiences, facts, procedures, resources, and sensitive information in dedicated memory modules.

This project implements a MIRIX-inspired Multi-Agent Memory System that routes incoming user information into specialized memory stores and enables intelligent retrieval using semantic similarity search and LLM-based reasoning.

The system combines memory routing, embedding-based retrieval, and agent orchestration to create a more realistic long-term memory framework for AI agents.

---

## Key Features

* Multi-Memory Architecture
* LangGraph-Based Agent Workflow
* LLM Integration via OpenRouter
* Semantic Memory Retrieval
* Sentence Transformer Embeddings
* Memory Classification and Routing
* Similarity-Based Search
* Gradio User Interface
* Automated Evaluation Framework
* Synthetic Benchmark Dataset Generation

---

## Memory Types

The system supports six specialized memory categories:

### Core Memory

Stores stable user attributes and long-term preferences.

Examples:

```text
My name is Ria.
I like pizza.
I enjoy swimming.
```

### Episodic Memory

Stores user experiences and events.

Examples:

```text
Today I went to the gym.
I did laundry today.
Last week I visited Delhi.
```

### Semantic Memory

Stores factual and conceptual knowledge.

Examples:

```text
AI means Artificial Intelligence.
Gravity is the force that attracts objects.
MIRIX is a multi-agent memory system.
```

### Procedural Memory

Stores instructions and task-oriented knowledge.

Examples:

```text
How to train a model in Python?
Steps to bake a cake.
How to reset a password?
```

### Resource Memory

Stores references to documents and external resources.

Examples:

```text
Check the PDF linked in the email.
This document contains the syllabus.
The presentation is in the document.
```

### Vault Memory

Stores sensitive information requiring protected storage.

Examples:

```text
API Key
Email Address
Passwords
Credentials
```

---

## System Architecture

```text
                    User Input
                          │
                          ▼
                Meta Memory Router
                          │
     ┌──────────┬──────────┬──────────┐
     ▼          ▼          ▼          ▼
   Core     Episodic   Semantic   Procedural
     │          │          │          │
     └──────────┴──────────┴──────────┘
                          │
               Resource & Vault Memory
                          │
                          ▼
              Embedding-Based Retrieval
                          │
                          ▼
                  LLM Reasoning Layer
                          │
                          ▼
                    Final Response
```

---

## Technology Stack

### AI & LLMs

* OpenRouter
* GPT Models
* LangChain
* LangGraph

### Embeddings

* Sentence Transformers
* all-MiniLM-L6-v2

### Development

* Python
* Gradio
* JSON
* CSV

### Retrieval

* Cosine Similarity Search
* Semantic Matching
* Embedding-Based Retrieval

---

## Workflow

### Memory Storage

1. User enters information.
2. Meta Router analyzes input.
3. Appropriate memory type is selected.
4. Information is stored in the corresponding memory store.

### Memory Retrieval

1. User submits a retrieval query.
2. Query is converted into embeddings.
3. Semantic similarity search is performed.
4. Relevant memories are retrieved.
5. LLM generates contextual reasoning.

---

## Evaluation Dataset

The project includes a synthetic benchmark dataset containing examples across multiple memory categories:

* Core Memory
* Episodic Memory
* Semantic Memory
* Procedural Memory
* Resource Memory
* Vault Memory
* Noise / Irrelevant Inputs

The benchmark is used to evaluate memory routing and retrieval performance across different memory types.

---

## Gradio Interface

The system includes an interactive Gradio application that allows users to:

* Store memories
* Retrieve memories
* Test routing behavior
* Evaluate memory classification

Example:

```text
Input:
I like pizza.

Output:
Stored in Core Memory
```

```text
Input:
get:pizza

Output:
Retrieved matching memories from Core Memory
```

---

## Repository Structure

```text
mirix-multi-agent-memory-system/
│
├── main.py
├── mirix_prompts_sampled.json
├── mirix_outputs_v2_sampled.json
├── requirements.txt
└── README.md
```

---

## Applications

* Agentic AI Systems
* Long-Term Memory for LLMs
* Personal AI Assistants
* Multi-Agent Architectures
* Conversational Memory Systems
* AI Research Prototypes
* Memory-Augmented Agents

---

## Future Improvements

* Vector Database Integration
* Persistent Memory Storage
* Hybrid Retrieval Systems
* Memory Importance Scoring
* Memory Consolidation
* Reflection and Self-Learning Agents
* Multi-Agent Memory Sharing
* RAG + Memory Hybrid Architecture

---

## Skills Demonstrated

* Agentic AI
* LangGraph
* LangChain
* LLM Integration
* Prompt Engineering
* Memory Architectures
* Semantic Search
* Embeddings
* Retrieval Systems
* Gradio
* Python
* AI Evaluation Frameworks

---

## Author

Anoushka Kaul

B.Tech Computer Science (AI/ML & Data Science)

Interests: Agentic AI, Generative AI, Memory Systems, Multi-Agent Architectures, and LLM Engineering.
