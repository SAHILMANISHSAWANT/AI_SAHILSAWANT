# ⚖️ Design Trade-offs

This document outlines key decisions made during the system design and the trade-offs considered.

---

## 1. Graph Database vs Relational Database

**Graph DB (Neo4j)**  
✅ Pros:
- Semantic relationships between concepts
- Efficient traversal for linked ideas

❌ Cons:
- Slower for flat queries
- Requires specialized query language (Cypher)

**Relational DB (PostgreSQL)**  
✅ Pros:
- Fast for tabular data
- Widely supported and understood

❌ Cons:
- Poor at representing hierarchical or semantic links

**Decision**: Chose Graph DB for its ability to model educational concepts and their relationships.

---

## 2. Markdown vs JSON for Slide Formatting

**Markdown**  
✅ Pros:
- Easy to read and edit
- Good for human collaboration

❌ Cons:
- Needs parsing for structured automation

**JSON**  
✅ Pros:
- Machine-friendly
- Easy to validate and transform

❌ Cons:
- Harder for manual editing

**Decision**: Use Markdown for initial formatting, convert to JSON for Manim automation.

---

## 3. FastAPI vs Flask for Backend

**FastAPI**  
✅ Pros:
- Asynchronous support
- Auto-generated docs
- Faster performance

❌ Cons:
- Slightly newer, smaller community

**Flask**  
✅ Pros:
- Mature and stable
- Large ecosystem

❌ Cons:
- Synchronous by default

**Decision**: Chose FastAPI for speed and async capabilities.

---

## 4. Manim vs Other Animation Tools

**Manim CE**  
✅ Pros:
- Precise mathematical animations
- Python-based and open-source

❌ Cons:
- Steep learning curve
- Requires scripting

**Other Tools (e.g., After Effects)**  
✅ Pros:
- GUI-based, easier for designers

❌ Cons:
- Not programmatically scalable
- Expensive licensing

**Decision**: Manim chosen for automation and educational precision.
