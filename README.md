# 🧠 Cognitive-Agent-Simulator

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-brightgreen.svg)](https://www.python.org/downloads/)
[![Autonomous Intelligence](https://img.shields.io/badge/AI-Cognitive-orange.svg)]()
[![Research Focused](https://img.shields.io/badge/Field-Research-red.svg)]()

**Cognitive-Agent-Simulator** is a research-focused framework for simulating agent reasoning, multi-step planning, and long-term memory management. It provides a standardized environment to experiment with autonomous deliberation loops and agentic self-reflection architectures.

---

## 🚀 Key Features

- **🎯 Chain-of-Thought (CoT) Simulation:** Detailed tracking of an agent's internal monologue and deliberation steps.
- **🔄 Multi-Step Planning:** Dynamic decomposition of complex objectives into executable cognitive steps.
- **🧠 Hybrid Memory Architecture:** Simulated management of short-term (contextual) and long-term (vectorized) memory.
- **🔍 Self-Reflection Loop:** Integrated feedback mechanism for agents to evaluate and adjust their own reasoning paths.
- **📊 Detailed Tracing:** High-granularity logs of the agent's internal cognitive state transitions.

---

## 🏗️ Architecture

`mermaid
graph TD
    Objective([User Objective]) --> Perception[Input Perception]
    Perception --> Loop{Cognitive Loop}
    Loop --> Thought[Reasoning / Thought Generation]
    Thought --> Action[Action Planning]
    Action --> Reflect[Self-Reflection]
    Reflect -- Re-Plan --> Thought
    Reflect -- Finish --> Final[Final Decision]
    Loop <--> Memory[(Cognitive Memory)]
`

---

## 🛠️ Project Structure

`	ext
Cognitive-Agent-Simulator/
├── src/
│   ├── cognitive/      # Core reasoning and deliberation engine
│   ├── memory/         # Short-term and Long-term memory simulations
│   ├── planners/       # Task decomposition and planning logic
│   └── utils/          # Shared helper functions
├── notebooks/          # Research and analysis notebooks
├── tests/              # Comprehensive test suite
└── requirements.txt    # Project dependencies
`

---

## 📖 Quick Start

`python
from src.cognitive.engine import ReasoningEngine

# 1. Initialize the Reasoning Engine
engine = ReasoningEngine("Socrates-AI")

# 2. Define a complex objective
objective = "Optimize global logistics for a retail supply chain."

# 3. Start the deliberation process
result = engine.deliberate(objective)

# 4. Inspect the reasoning history
for step in engine.get_history():
    print(f"Thought: {step.thought} -> Action: {step.action}")
`

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
<p align="center">Built with ❤️ by <a href="https://github.com/peeyushpashine23">Peeyush Pashine</a></p>