# 🧩 Component Explanation

This document breaks down each module in the system.

---

## 1. 📚 Knowledge Graph

- Stores textbook concepts and relationships.
- Built using Neo4j or RDF.
- NLP (spaCy/BERT) extracts entities from user queries.

---

## 2. 🤖 AI Slide & Script Generator

- Uses GPT-4 or similar LLM.
- Prompt engineering tailors output to education level.
- Generates structured slides and narration.

---

## 3. 🧾 Slide & Script Formatter

- Converts AI output into Markdown or JSON.
- Prepares content for Manim rendering.
- Uses Python templating (e.g., Jinja2).

---

## 4. 🎞️ Manim Automation

- Manim CE renders animations from formatted scripts.
- Each slide becomes a scene.
- Final video is stitched together.

---

## 5. ⚙️ Backend Orchestration

- FastAPI handles user requests.
- Celery manages asynchronous tasks.
- Docker ensures portability and scalability.

---

## 6. 🗃️ Storage & Retrieval

- AWS S3 or Azure Blob stores videos.
- PostgreSQL stores metadata.
- Redis caches frequent queries.
