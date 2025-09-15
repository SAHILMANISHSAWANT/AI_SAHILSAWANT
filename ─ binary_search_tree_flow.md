# 🌳 Binary Search Tree – End-to-End Flow Example

This example demonstrates how the system transforms a user query into an animated educational video using the AI-powered pipeline.

---

## 🧑‍🎓 User Query

> "Explain Binary Search Tree with examples and animations."

---

## 📚 Concept Retrieval

- **Entities Extracted**: "Binary Search Tree", "examples", "animations"
- **Graph DB Node Matched**: `BST`
- **Content Retrieved**:
  - Definition: A binary tree where each node has at most two children.
  - Property: Left child < parent < right child.
  - Applications: Searching, sorting, hierarchical data.

---

## 🤖 AI Slide & Script Generation

**Prompt Sent to LLM**:

**Generated Slides**:
1. **Slide 1**: What is a Binary Search Tree?
   - Definition and structure
2. **Slide 2**: Insertion Logic
   - Step-by-step example
3. **Slide 3**: Search Operation
   - How to find a value
4. **Slide 4**: Traversal Techniques
   - Inorder, Preorder, Postorder
5. **Slide 5**: Real-World Applications
   - File systems, databases, autocomplete

---

## 🧾 Slide & Script Formatting

**Formatted Output**:
```json
[
  {
    "scene_title": "What is a Binary Search Tree?",
    "scene_content": "A BST is a tree where each node has two children. Left < Root < Right."
  },
  {
    "scene_title": "Insertion Logic",
    "scene_content": "Start at root. Compare value. Go left or right. Insert at null."
  },
  ...
]
sample scene
class BSTIntro(Scene):
    def construct(self):
        title = Text("Binary Search Tree")
        definition = Text("Left < Root < Right")
        self.play(Write(title))
        self.wait(1)
        self.play(Transform(title, definition))
