# 🧠 AI Backend Portfolio — Jeff Ellis

### A production-grade, Go-based AI backend ecosystem focused on **Retrieval-Augmented Generation (RAG)** with reusable AI microservices and a lightweight orchestration layer.

This organization contains a cohesive set of **AI backend microservices** designed to mirror real-world backend and AI engineering systems.

The core focus is **RAG architecture**, supported by:

* embeddings (vector search building blocks)
* summarization (task-specific transformation)
* **generative text** (prompt-driven LLM output)
* optional orchestration (service coordination + evaluation)

All services are containerized, deployed, documented, and built with production patterns in mind.

---

## 🌐 System Architecture Overview

```mermaid
flowchart LR

    Client --> RAG
    RAG --> GenAI
    RAG --> Summary
    RAG --> Client

    Embeddings
    Orchestrator
```

> Notes: **Embeddings** and **Summary** are standalone microservices. **GenAI** is a standalone, prompt-driven generation service. **Orchestrator** is included as a supporting workflow layer.

---

## 📦 Repositories

### **1. Notes Memory Core — RAG Extension (Flagship)**

A production-ready **Retrieval-Augmented Generation backend** built with Go, Postgres, and pgvector.
Implements semantic search, top-K retrieval, and context preparation for downstream AI tasks.

📌 [https://github.com/ai-backend-course/notes-memory-core-rag](https://github.com/ai-backend-course/notes-memory-core-rag)

---

### **2. Notes Memory Core**

The foundational CRUD backend for storing and retrieving notes.
Demonstrates clean service layout, Postgres integration, logging, and metrics.

📌 [https://github.com/ai-backend-course/notes-memory-core](https://github.com/ai-backend-course/notes-memory-core)

---

### **3. Generative AI Service**

A production-deployed **prompt-driven** Generative AI microservice built in Go.
Exposes a clean `/generate` endpoint for text generation and acts as a reusable LLM capability for other backend services.

📌 [https://github.com/ai-backend-course/ai-generative-service](https://github.com/ai-backend-course/ai-generative-service)

---

### **4. AI Summary Service**

An LLM-powered summarization microservice used to condense retrieved context or other text inputs.
Designed as a task-specific service (summarization) rather than a general generation API.

📌 [https://github.com/ai-backend-course/ai-summary-service](https://github.com/ai-backend-course/ai-summary-service)

---

### **5. AI Embedding Microservice**

A dedicated embedding service supporting mock and real OpenAI embeddings, with validation, rate limiting, and observability.

📌 [https://github.com/ai-backend-course/ai-embedding-microservice](https://github.com/ai-backend-course/ai-embedding-microservice)

---

### **6. Workflow / Orchestration Service (Supporting Project)**

A lightweight orchestration layer that coordinates retrieval + summarization, applies evaluation, and produces structured responses.

This service is **not the core focus** of the portfolio, but demonstrates how multiple AI backend services can be coordinated in a controlled workflow.

📌 [https://github.com/ai-backend-course/agentic-workflow-service](https://github.com/ai-backend-course/agentic-workflow-service)
🌐 [https://agentic-workflow-service.fly.dev](https://agentic-workflow-service.fly.dev)

---

## 🚀 Skills Demonstrated

* Go (Golang) backend development
* Fiber v2: routing, middleware, handlers
* Retrieval-Augmented Generation (RAG) architecture
* Embeddings and vector search (pgvector)
* Service-to-service AI backend design
* Postgres 16 + pgxpool
* Semantic search and top-K retrieval
* **Prompt-driven generative text APIs**
* AI summarization pipelines
* Docker + multi-stage builds
* Fly.io production deployment
* TLS and container runtime configuration
* Logging, tracing, and observability
* Clean, production-oriented API design

---

## 🏆 About This Portfolio

This portfolio is centered on **RAG-first AI backend systems**, reflecting how many real-world AI applications are built today.

The projects emphasize:

* clear API boundaries
* production-ready backend patterns
* deployable services
* explainable AI pipelines
* incremental system design

The orchestration layer is included to show **service coordination and workflow control**, while the primary strength remains **retrieval, data grounding, and backend reliability**.

This work aligns with **AI Backend Engineer**, **Backend Engineer (AI-enabled systems)**, and **RAG-focused roles**.

---

## 📬 Contact

```
Jeff Ellis
AI Backend Developer
Email: jellis777@gmail.com
GitHub: https://github.com/jellis777
```
