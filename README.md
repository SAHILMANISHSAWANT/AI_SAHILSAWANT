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

Certainly! Here’s the **description of the system architecture flow** in plain words based on the diagram you provided:

---

### System Architecture Flow Description

1. **User Interface**
   The user interacts with the system by inputting a concept query and later views the generated educational video.

2. **Backend Orchestrator**
   This component controls the entire process, managing the flow of data and coordinating between different modules.

3. **Knowledge Graph Database and API**
   The backend queries the knowledge graph database through an API that performs semantic search and retrieves relevant concepts and related information.

4. **AI Content Module**
   Using the retrieved data from the knowledge graph, this module employs a large language model (LLM) to generate detailed slide content and narration scripts explaining the concept.

5. **Slide & Script Formatter**
   This component structures and organizes the AI-generated content into well-formatted slides along with synchronized narration scripts, ready for presentation.

6. **Manim Animation Engine**
   The formatted slides and scripts are passed to the Manim animation engine, which programmatically creates animated educational videos illustrating the concepts.

7. **Storage & Content Delivery Network (CDN)**
   The generated videos, scripts, and related metadata are stored securely and cached for faster retrieval. The CDN ensures smooth and efficient streaming of the videos to users.

8. **User Interface (Output)**
   Finally, the system streams the animated educational video back to the user interface, where the user can watch and learn from the generated content.

---

If you want, I can help rephrase it or write it for a specific section like documentation or a presentation!

# Prerequisites
**1.Python 3.10+**

**2.Docker**

**3.Neo4j (local or cloud)**

**4.OpenAI API key**

# 1. Clone the repo
git clone https://github.com/your-username/edugraph.git
cd edugraph
# 2. Setup backend
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
# 3. Setup Manim automation
cd ../manim_engine
pip install -r requirements.txt
Render a sample animation:
python render_bst.py
# 📂 Folder Structure
| Folder/File                          | Description                                      |
|-------------------------------------|--------------------------------------------------|
| `README.md`                         | Project overview and setup instructions          |
| `docs/`                             | System documentation and architecture            |
| ├── `architecture.md`              | High-level system design and flow                |
| ├── `flow_diagram.png`             | Visual diagram of the pipeline                   |
| ├── `component_explanation.md`     | Detailed breakdown of each module                |
| └── `sector_extensions.md`         | Customization for GIS, Space Tech, DSA, etc.     |
| `pseudo_code/`                      | Pseudo-code for core modules                     |
| ├── `concept_retrieval.py`         | Retrieves concept from knowledge graph           |
| ├── `ai_slide_generator.py`        | Generates slides and scripts using AI            |
| ├── `formatter.py`                 | Formats content for Manim                        |
| ├── `manim_automation.py`          | Automates Manim rendering                        |
| └── `backend_orchestration.py`     | Coordinates the full pipeline                    |
| `assets/`                           | Visuals and examples                             |
| ├── `diagrams/system_architecture.png` | PNG version of architecture diagram          |
| └── `examples/binary_search_tree_flow.md` | Sample concept-to-video flow               |
| `ideas/`                            | Design decisions and prompt strategies           |
| ├── `tradeoffs.md`                 | Key trade-offs in system design                  |
| ├── `tech_stack_choices.md`        | Justification for chosen technologies            |
| └── `prompt_templates.md`          | Reusable prompts for different domains           |

# 📌 Upcoming Features
### 🗣️ Voice-over narration using TTS

### 🌐 Multilingual support for global learners

### 📊 Dashboard for tracking generated content

### 🧪 Sector-specific templates (GIS, Space Tech, DSA)

# 🤝 Contributing
We welcome contributions! Please check out the ideas/ folder for open design discussions and submit pull requests with clear documentation.
