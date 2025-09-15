# 🧪 Tech Stack Justification

This document explains the rationale behind each technology used in the system.

---

## 📚 Knowledge Graph

**Neo4j**  
- Ideal for representing semantic relationships between concepts
- Supports Cypher queries for graph traversal

## 🧠 NLP & AI

**spaCy / BERT**  
- Used for entity extraction and concept identification from user queries

**GPT-4 / LLMs**  
- Generates educational slides and scripts
- Adaptable to different learning levels

## 🧾 Slide Formatting

**Markdown + JSON**  
- Markdown for readability
- JSON for structured automation

## 🎞️ Animation

**Manim CE**  
- Python-based animation engine
- Perfect for educational and mathematical visualizations

## ⚙️ Backend

**FastAPI**  
- Async support for fast performance
- Easy integration with Celery and Docker

**Celery**  
- Task queue for managing long-running jobs (e.g., video rendering)

**Docker**  
- Containerization for deployment and scalability

## 🗃️ Storage & Caching

**AWS S3 / Azure Blob**  
- Stores generated videos and assets

**PostgreSQL**  
- Stores metadata and user queries

**Redis**  
- Caches frequent queries and results
