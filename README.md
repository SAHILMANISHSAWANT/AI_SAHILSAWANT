# 🎓 EduGraph – AI-Powered Concept-to-Animation Pipeline

EduGraph is a modular AI system that transforms textbook concepts into animated educational videos using a knowledge graph, large language models, and the Manim animation engine. Whether you're a student exploring Binary Search Trees or a teacher explaining Kepler’s Laws, EduGraph automates the entire journey from query to visual learning.

---

## 🌟 Features

- 🔍 **Concept Retrieval**: Extracts and matches textbook concepts using NLP and a semantic knowledge graph.
- 🧠 **AI Slide Generation**: Automatically creates educational slides and narration scripts using LLMs.
- 🧾 **Script Formatting**: Converts AI output into structured templates for animation.
- 🎞️ **Manim Automation**: Renders animated video scenes from formatted scripts.
- ⚙️ **Backend Orchestration**: Coordinates the entire pipeline from input to output.
- 📦 **Storage & Retrieval**: Saves generated videos and metadata for future access.

---

## 🧑‍💻 Tech Stack

- **Knowledge Graph**: Neo4j, spaCy, BERT
- **AI Generation**: GPT-4 / OpenAI API
- **Animation Engine**: Manim CE (Python)
- **Backend**: FastAPI, Celery, Docker
- **Storage**: AWS S3, PostgreSQL, Redis

---

## 🔄 Project Flow


graph TD
    A[🧑‍🎓 User Query] --> B[NLP Entity Extraction]
    B --> C[📚 Knowledge Graph Retrieval]
    C --> D[🤖 AI Slide & Script Generator]
    D --> E[🧾 Slide & Script Formatter]
    E --> F[🎞️ Manim Animation Engine]
    F --> G[📦 Video Output]
    G --> H[🗃️ Storage & Retrieval System]
    H --> I[🔁 Retrieval API]
🛠️ Getting Started Locally
## Prerequisites
# 1.Python 3.10+

# 2.Docker

# 3.Neo4j (local or cloud)

# 4.OpenAI API key

## 1. Clone the repo
git clone https://github.com/your-username/edugraph.git
cd edugraph
## 2. Setup backend
cd backend
pip install -r requirements.txt
Create a .env file in /backend with:
OPENAI_API_KEY=your_openai_key
NEO4J_URI=bolt://localhost:7687
NEO4J_USER=neo4j
NEO4J_PASSWORD=your_password
S3_BUCKET=your_bucket_name
Run backend:
uvicorn main:app --reload
## 3. Setup Manim automation
cd ../manim_engine
pip install -r requirements.txt
Render a sample animation:
python render_bst.py
## 📂 Folder Structure
AI-KnowledgeGraph-Manim-Automation/
├── README.md
├── docs/
│   ├── architecture.md
│   ├── flow_diagram.png
│   ├── component_explanation.md
│   └── sector_extensions.md
├── pseudo_code/
│   ├── concept_retrieval.py
│   ├── ai_slide_generator.py
│   ├── formatter.py
│   ├── manim_automation.py
│   └── backend_orchestration.py
├── assets/
│   ├── diagrams/
│   │   └── system_architecture.png
│   └── examples/
│       └── binary_search_tree_flow.md
├── ideas/
│   ├── tradeoffs.md
│   ├── tech_stack_choices.md
│   └── prompt_templates.md
## 📌 Upcoming Features
# 🗣️ Voice-over narration using TTS

# 🌐 Multilingual support for global learners

# 📊 Dashboard for tracking generated content

# 🧪 Sector-specific templates (GIS, Space Tech, DSA)

##🤝 Contributing
We welcome contributions! Please check out the ideas/ folder for open design discussions and submit pull requests with clear documentation.
