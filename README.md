# Hyprland Lua RAG Framework

A semantic, structural RAG (Retrieval-Augmented Generation) infrastructure
designed for zero-hallucination AI-driven development and seamless migration to Hyprland 0.55.2+.

### 🛠️ Architecture Philosophy

Unlike traditional dotfile repositories that rely on raw text or ad-hoc prompting, this framework treats configuration specifications as an intelligent, semantic data layer, designed to function as a **Deterministic RAG** (Retrieval-Augmented Generation) infrastructure.

- **Separation of Data and Logic**: Configuration specifications are modeled in semantic HTML (Data Layer), allowing LLMs to parse exact API boundaries and structural constraints without interference from runtime deployment scripts (Logic Layer).
    
- **Self-Documenting Topology**: Utilizes JSON-LD (`ItemList`) and structured metadata to inject an absolute frame of reference directly into the AI's inference context, effectively mapping the entire configuration landscape.
    
- **Cognitive Load Reduction**: Eliminates AI hallucination by establishing physical network entry points (`root-skill.html`), forcing the LLM to rely on provided structural data rather than its own unstable internal knowledge base.
    
- **Deterministic RAG Paradigm**: By treating the LLM as a strictly bounded compiler rather than a conversational assistant, this framework ensures that structural inputs yield predictable, error-free outputs, enabling flawless 1-shot refactoring and migration.
    
- **Infrastructure-as-Context**: Rather than refining prompts, this system optimizes the data infrastructure itself. It provides a stable, machine-readable topology that allows the AI to operate with 100% precision, transforming configuration management from a probabilistic task into a deterministic execution.

## 🚀 Usage Workflow

1. Feed `root-skill.html` as the root context into your LLM CLI (e.g., Antigravity CLI).
2. The AI automatically maps the entire configuration topology via the embedded JSON-LD.
3. Prompt the AI for your configuration needs. It will output 100% precise, verified Lua code on the first attempt.

## 📂 Repository Structure & Extensibility

The repository is structured as a generic framework with strict separation of concerns.

```text
.
├── Configuring
│   ├── Advanced-and-Cool/      # Empty (Ready for your custom specs)
│   ├── Basics
│   │   ├── Autostart
│   │   │   └── spec-skill.html # Provided
│   │   ├── Binds
│   │   │   └── spec-skill.html # Provided
│   │   ├── Dispatchers
│   │   │   └── spec-skill.html # Provided
│   │   ├── Monitors
│   │   │   └── spec-skill.html # Provided
│   │   ├── Variables
│   │   │   └── spec-skill.html # Provided
│   │   ├── Window-Rules
│   │   │   └── spec-skill.html # Provided
│   │   └── Workspace-Rules
│   │       └── spec-skill.html # Provided
│   ├── Example-configurations/ # Empty (Ready for your custom specs)
│   ├── Layouts/                # Empty (Ready for your custom specs)
│   └── Start/                  # Empty (Ready for your custom specs)
├── README.md
└── root-skill.html             # Physical network entry point (Index)

```



🛠️ Extensibility Notice (Bring Your Own Data)

    No Scraping Scripts Provided: The internal scraping and formatting script (lrag_format.py) is kept strictly private and is not included in this repository.

    Analyze and Extend: The folder structure is purposefully designed for complete modular scalability. For directories currently left empty (e.g., Advanced-and-Cool, Layouts), users are expected to analyze the rigorous semantic HTML schema, metadata tags, and JSON-LD topologies provided in the Basics directory, and reverse-engineer or manually craft their own spec-skill.html files.

🚀 Proven Success with Basics Layer

During actual deployment in the author's workstation environment, feeding only the provided Basics layer into the LLM context resulted in a 100% flawless, error-free refactoring and migration to the new Hyprland Lua API on the very first attempt.

(Note: While the code generation itself was achieved in a single shot, a full system/environment restart was required to apply and finalize the configuration changes correctly on the host machine).
