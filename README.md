# LangGraph Fundamentals

This repository contains my first hands-on exploration of LangGraph and its core concepts.

The goal of this notebook was to understand how LangGraph manages state, executes nodes, and orchestrates workflows while integrating with OpenAI models.

## What I Implemented

### State Management

Created a shared state using Pydantic to store:

* User question
* LLM-generated response

### Graph Construction

Built a simple LangGraph workflow consisting of:

```text
START
   │
   ▼
generate_answer
   │
   ▼
 END
```

### LLM Integration

Integrated OpenAI's GPT model using LangChain's `ChatOpenAI` interface.

The workflow:

1. Receives a user query.
2. Passes it to an OpenAI model.
3. Updates the graph state with the generated response.
4. Returns the final state.

### Graph Compilation

Compiled the workflow into an executable graph and visualized its structure.

### Gradio Interface

Created a basic Gradio chat interface to interact with the LangGraph application.

---

## Key Concepts Explored

* LangGraph State
* StateGraph
* Nodes
* Edges
* Graph Compilation
* State Updates
* OpenAI Integration
* Gradio Chat Interface

---

## Files

```text
basic_langgraph.ipynb
```

Contains the complete implementation along with explanations of each LangGraph component.

---

## Learnings

Through this exercise, I gained practical understanding of:

* How LangGraph differs from traditional chains
* Managing application state across nodes
* Building graph-based AI workflows
* Integrating LLM calls inside LangGraph nodes
* Executing and debugging LangGraph applications

---

## Next Steps

Future explorations may include:

* Multi-node workflows
* Conditional edges
* Tool calling
* Memory management
* Retrieval-Augmented Generation (RAG)
* Multi-agent systems
* Human-in-the-loop workflows

---

This notebook serves as a foundation for my LangGraph learning journey and future agentic AI projects.
