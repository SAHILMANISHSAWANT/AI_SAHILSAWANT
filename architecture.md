# 📐 System Architecture

## 🎯 Overview

This system transforms textbook concepts into animated educational videos using AI and Manim. It is modular, scalable, and designed for automation.

---

## 🔄 Workflow Pipeline

1. **User Query**: Student asks for a concept (e.g., "Explain Binary Search Tree").
2. **Concept Retrieval**: NLP extracts entities; graph DB returns relevant content.
3. **AI Slide Generator**: LLM generates slides and narration script.
4. **Formatter**: Structures content into Manim-compatible format.
5. **Manim Automation**: Renders animated video scenes.
6. **Backend Orchestration**: Coordinates all modules.
7. **Storage & Retrieval**: Saves outputs and enables future access.

---

## 🧠 Architecture Diagram

See `flow_diagram.png` in the `diagrams/` folder for a visual representation.
