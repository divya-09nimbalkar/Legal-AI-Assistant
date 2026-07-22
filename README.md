
```markdown
#  Legal AI Assistant

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://python.org)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini-2.5--flash-blueviolet.svg)](https://aistudio.google.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Production_Ready-brightgreen.svg)]()

>  An interactive contract compliance and auditing application that leverages **Google Gemini 2.5-Flash JSON enforcement models** to parse raw legal text pools, isolate asymmetric liabilities, output counter-negotiation redlines, and run context-aware legal chats.

---

##  Table of Contents
- [Overview](#overview)
- [System Architecture](#system-architecture)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [Jupyter Cell Sequence Blueprint](#jupyter-cell-sequence-blueprint)
- [Installation & Environment Setup](#installation--environment-setup)
- [Project Directory Architecture](#project-directory-architecture)
- [License](#license)

---

##  Overview

Commercial agreements frequently hide asymmetrical liabilities within complex boilerplate text. The **Legal AI Assistant** simplifies contract reviews by systematically isolating high-risk terms (such as extreme indemnification or unlimited liability), mapping out counter-negotiation redlines, and evaluating overall document compliance against institutional standards.

---

##  System Architecture


```

Raw Unstructured Contract Document Input
│
▼
┌────────────────────────────────────────────────────────┐
│         Gemini 2.5-Flash Auditing Engine               │
│  ┌───────────────────────┐ ┌────────────────────────┐  │
│  │ Clause Classifier     │ │ Structural Risk Scorer │  │
│  └───────────────────────┘ └────────────────────────┘  │
│  ┌───────────────────────┐ ┌────────────────────────┐  │
│  │ Executive Summarizer  │ │ Redline Strategy Gen   │  │
│  └───────────────────────┘ └────────────────────────┘  │
└──────────────────────────┬─────────────────────────────┘
│
▼
┌────────────────────────────────────────────────────────┐
│         Interactive UI Layout Outputs (Gradio)         │
│  ┌───────────────────────┐ ┌────────────────────────┐  │
│  │ Executive Legal Brief │ │ Matplotlib Risk Bars   │  │
│  └───────────────────────┘ └────────────────────────┘  │
│  ┌───────────────────────┐ ┌────────────────────────┐  │
│  │ Counter Redlines List │ │ Chat Query Advisor     │  │
│  └───────────────────────┘ └────────────────────────┘  │
└────────────────────────────────────────────────────────┘

```

---

##  Key Features

* **JSON-Forced Legal Parser:** Extracts exact clause text, assigns a standardized threat matrix tier, and suggests targeted changes based on 12 key legal criteria.
* **Regex Hybrid Watchdog:** Combines pattern-matching rules with generative AI to spot high-liability indicators like unlimited liability or one-sided waivers.
* **Algorithmic Safety Scoring:** Deducts points dynamically from a base score of 100 based on the volume and severity of critical legal threats found.
* **Negotiation Strategy Architect:** Auto-generates practical counter-arguments and redline suggestions to balance unfair, one-sided terms.
* **Context-Aware Legal Advisor:** Provides interactive chat capabilities backed by conversational memory to answer questions regarding active clauses.

---

##  Tech Stack

* **AI Processing Framework:** Google Gemini 2.5-Flash (`google-generativeai`)
* **Visual Interface Engine:** Gradio Blocks Dashboard Grid (Gradio 6.0+ compatible)
* **Graphical Representation Layer:** Matplotlib Plotting Components
* **Data Processing Models:** Pandas DataFrames & NumPy Matrix Fields
* **Document Extraction Tooling:** Local PDF parsing engines via `pdfplumber`

---

##  Jupyter Cell Sequence Blueprint

| Cell # | Type | Target Context Module | Operational Analytical Purpose |
| :--- | :--- | :--- | :--- |
| **Cell 1** |  Markdown | **Documentation Cover** | System summary badges, feature indices, and structural maps. |
| **Cell 2** |  Code | **Package Downloads** | Installs AI libraries, pdfplumber, and core dependencies. |
| **Cell 3** |  Code | **Global Setup** | Imports libraries, sets global configurations, and initializes data class schemas. |
| **Cell 4** |  Code | **Contract Parser** | Implements the `ContractParser` module to extract structured clauses. |
| **Cell 5** |  Code | **Risk Assessment** | Defines `LegalRiskAnalyzer` for scoring and rendering risk profiles. |
| **Cell 6** |  Code | **Orchestrator Pipeline** | Builds `LegalAIAssistant` to coordinate chat histories and summarization. |
| **Cell 7** |  Code | **Verification Test Run** | Tests the pipeline end-to-end against sample commercial agreement texts. |
| **Cell 8** |  Code | **Gradio App Layout** | Launches the complete web application interface directly inside your browser. |

---

##  Installation & Environment Setup

### 1. Build Local Workspace Directory
```bash
git clone [https://github.com/yourusername/Legal_AI_Assistant.git](https://github.com/yourusername/Legal_AI_Assistant.git)
cd Legal_AI_Assistant
python -m venv venv
source venv/bin/activate # Windows Terminal: .\venv\Scripts\activate

```

### 2. Deploy Dependencies Manifest

```bash
pip install -r requirements.txt

```

### 3. Setup Gemini Access Token

Get a free API access key directly from [Google AI Studio](https://aistudio.google.com/). Paste your secret key parameter inside **Cell 3** configuration rows:

```python
os.environ["GEMINI_API_KEY"] = "AIzaSyYourSecretKeyStringHere"

```

---

## 📁 Project Directory Architecture

```text
Legal_AI_Assistant/
├── notebooks/
│   └── Legal_AI_Assistant.ipynb   # Main interactive development notebook workspace
├── output/
│   └── risk_analysis.png          # Rendered horizontal clause distribution pie charts
├── .gitignore                     # Git configuration element tracking blocks
├── README.md                      # Comprehensive system documentation (This file)
└── requirements.txt               # Pinned application dependencies manifest

```

---

## ⚠️ Disclaimer & Safety Guidelines

> 🚨 **IMPORTANT NOTICE:** This platform is designed strictly as an educational proof-of-concept and a contract-auditing research assistant tool. It **does not** provide official legal advice and should never replace professional legal counsel or formal review by a qualified attorney.

---

## 👤 Author

**Divya** — AI/ML Developer | B.Tech Electronics & Telecom

```

```
